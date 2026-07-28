# Contributing to Cohesive Research

## Research Defs

Define all `ResearchProjectDef`s in `Conditional Defs/<Research Project Name>/Defs`, and then add a line in [LoadFolders.xml](LoadFolders.xml) with all mods whose patches require the research project.

Example:

[Glass Blowing.xml](Conditional%20Defs/Glass%20Blowing/Defs/Glass%20Blowing.xml)

```xml
<Defs>
    <ResearchProjectDef>
        <defName>KobeRiddle_GlassBlowing</defName>
        <label>glass blowing</label>
        <description>Creating and using glass</description>
        <baseCost>500</baseCost>
        <techLevel>Medieval</techLevel>
        <prerequisites>
            <li>Smithing</li>
        </prerequisites>
        <researchViewX>0</researchViewX>
        <researchViewY>0</researchViewY>
    </ResearchProjectDef>
</Defs>
```

[LoadFolders.xml](LoadFolders.xml)

```xml
...
<!-- Conditional Defs -->
<li IfModActive="Aelanna.TransparentSubstructure,Dubwise.DubsSkylights">Conditional Defs/Glass Blowing</li>
...
```

## Patches

Place all `PatchOperation`s in `Mod Patches/<Folder Name>/<Mod Name>/Patches`, and then add a line in [LoadFolders.xml](LoadFolders.xml) with the associated mod and the folder. Add the mod(s) to [About.xml](About/About.xml)'s `<loadAfter>` list as well.

Allowed Patch Operations:

- Patch Operations from Vanilla Rimworld
- Patch Operations provided by Research Reinvented: Stepping Stones

We are unable to define variable names, method names, etc. in RimWorld XML patches, so please use comments to explain what each operation does.

>! Do not use `<Success>Always</Success>` in your patches. This doesn't make your patches work, it makes them fail silently.

Example Patch

[Transparent Substructure Patches.xml](Mod%20Patches/Other/Transparent%20Substructure/Patches/Transparent%20Substructure%20Patches.xml)

```xml
<Patch>

    <!-- Add glass as a prerequisite for transparent foundations and floors -->

    <!-- Floors inheriting from TileMetalBase: override parent prerequisites -->
    <Operation Class="PatchOperationAdd">
        <xpath>Defs/TerrainDef[
            defName="TransparentFoundation_FineTile"
            or defName="TransparentFoundation_SkyTile"
            or defName="TransparentFoundation_FineSkyTile"
            or defName="TransparentFoundation_Substructure"
            ]
        </xpath>
        <value>
            <researchPrerequisites Inherit="False">
                <li>KobeRiddle_GlassBlowing</li>
            </researchPrerequisites>
        </value>
    </Operation>

    <!-- Bridge: append glass to existing prerequisites -->
    <Operation Class="PatchOperationAdd">
        <xpath>Defs/TerrainDef[
            defName="TransparentFoundation_HeavyBridge"
            ]/researchPrerequisites
        </xpath>
        <value>
            <li>KobeRiddle_GlassBlowing</li>
        </value>
    </Operation>

</Patch>
```

[LoadFolders.xml](LoadFolders.xml)

```xml
...

    <li IfModActive="Aelanna.TransparentSubstructure">Mod Patches/Other/Transparent Substructure</li>
...
```

## Ordering

LoadFolders and [About.xml](About/About.xml)'s `<loadAfter>` list are sorted first by folder (custom order), then alphabetically by mod name. Please add new entries in the correct order. Contributors should not create sorting folders (i.e VE, Other, etc.) without first asking permission.