# Cohesive Research: A Stepping Stones Project

- [Cohesive Research: A Stepping Stones Project](#cohesive-research-a-stepping-stones-project)
    - [Overview](#overview)
    - [Changes](#changes)
        - [Vanilla Expanded](#vanilla-expanded)
            - [VFE Classical](#vfe-classical)
            - [VFE Tribals](#vfe-tribals)
        - [Other](#other)
            - [Progression: Production](#progression-production)
        - [Transparent Substructure](#transparent-substructure)
    - [Planned Changes](#planned-changes)
        - [VE Cooking](#ve-cooking)
        - [VCE - Carnivore/Vegetarian Meals Patch](#vce---carnivorevegetarian-meals-patch)
        - [Mods which will not be patched (for now)](#mods-which-will-not-be-patched-for-now)

## Overview
Cohesive Research is a collection of patches in the vein of [Research Reinvented: Stepping Stones](https://steamcommunity.com/sharedfiles/filedetails/?id=2868389782), increasing cohesiveness and compatibility with Stepping Stones' more individualized research projects.

## Changes

Key: Research Project(s)/Thing(s)/Recipe(s) <- New prerequisite Research Project (source mod)

### Combat Extended

#### Core
Note: Currently, only the generic ammo types are supported, and it is higly recomneded to use The Generic Ammo Experience for Combat Extended (a mod by Turkler) when using this patch. This may change in the future. The research requirements from this patch (and the other CE patches in this mod) are in addition to the original requirements, not a repleacement. Also note, if you are using YART it currently will show the non-generic ammo types in the research tree despite the generic ammo types option in CE being enabled, this has been reported to YARTs developer and hopefully will be fixed in the future. 

Research Projects:

- Incendiary Launcher <- Incendiary Weapons (Research Reinvented:Stepping Stones)
- Flare Gun <- Incendiary Weapons (Research Reinvented:Stepping Stones)
- EMP Grenades <- EMP Weapons (Research Reinvented:Stepping Stones)
- Anti-Materiel Incendiary Ammo <- Incendiary Weapons (Research Reinvented:Stepping Stones)
- Incendiary Mortar Shells <- Incendiary Weapons (Research Reinvented:Stepping Stones)
- Incendiary Rifle Ammo <- Incendiary Weapons (Research Reinvented:Stepping Stones)
- Incendiary Intermediate Rifle Ammo <- Incendiary Weapons (Research Reinvented:Stepping Stones)
- Incendiary Magnum Rifle Ammo <- Incendiary Weapons (Research Reinvented:Stepping Stones)
- Fire Arrows <- Incendiary Weapons (Research Reinvented:Stepping Stones)
- Flare Cartridges <- Incendiary Weapons (Research Reinvented:Stepping Stones)
- EMP Launcher Grenades <- EMP Weapons (Research Reinvented:Stepping Stones)
- EMP Autocannon Grenades <- EMP Weapons (Research Reinvented:Stepping Stones)
- EMP Mortar Shells <- EMP Weapons (Research Reinvented:Stepping Stones)
- 155mm EMP Howitzer Shells <- EMP Weapons (Research Reinvented:Stepping Stones)
- Heavy Cannon EMP Shells <- EMP Weapons (Research Reinvented:Stepping Stones)
- Napalm Flamethrower Fuel <- Incendiary Weapons (Research Reinvented:Stepping Stones)
- Prometheum Flamethrower Fuel <- Incendiary Weapons (Research Reinvented:Stepping Stones)

Research Projects (Only active when *The Generic Ammo Experience for Combat Extended* is NOT installed):

- Incendiary Launcher Grenades <- Incendiary Weapons (Research Reinvented:Stepping Stones)
- Incendiary Autocannon Shells <- Incendiary Weapons (Research Reinvented:Stepping Stones)
- Incendiary Artillery Shells <- Incendiary Weapons (Research Reinvented:Stepping Stones)
- Electro Slug Shotgun Ammo <- EMP Weapons (Research Reinvented:Stepping Stones)
- EMP Artillery Shells <- EMP Weapons (Research Reinvented:Stepping Stones)

#### Combat Extended Guns

Research Projects:

- Flamethrower <- Incendiary Weapons (Research Reinvented:Stepping Stones)

#### The Generic Ammo Expeience for Comabt Extended

Research Projects:

- EMP Missiles <- EMP Weapons (Research Reinvented:Stepping Stones)
- EMP Rocket Grenades <- EMP Weapons (Research Reinvented:Stepping Stones)
- Incendiary Missiles <- Incendiary Weapons (Research Reinvented:Stepping Stones)
- Incendiary Fuel Ammo <- Incendiary Weapons (Research Reinvented:Stepping Stones)
- Incendiary Autocannon Shells <- Incendiary Weapons (Research Reinvented:Stepping Stones)
- EMP Shotgun Shells <- EMP Weapons (Research Reinvented:Stepping Stones)
- Mounted Flamethrower Turret <- Incendiary Weapons (Research Reinvented:Stepping Stones)
- Flamethrower AutoTurret <- Incendiary Weapons (Research Reinvented:Stepping Stones)
- Smoke Bombs <- Basic Explosives (The Generic Ammo Experience for Combat Extended)

### Vanilla Expanded

#### VFE Classical

Research Projects:

- Togas <- Basic Apparel (Research Reinvented:Stepping Stones)
    - If VFE Tribals is installed: Togas <- Tribalwear (VFE Tribals)
- Tyrian Production <- Basic Apparel (Research Reinvented:Stepping Stones)
    - If VFE Tribals is installed: Tyrian Production <- Tribalwear (VFE Tribals)
- Temperature control research project <- Passive Cooler (Core)
- Mosaics <- Stonecutting (Core)
- Thermaebath <- Stonecutting (Core)
- Drama and Comedy <- Stonecutting (Core)
- Bronze Working <- Smithing (Core)
- Crafting Bench <- Basic Crafting Facilities (Research Reinvented:Stepping Stones)
- Cement Making <- Stonecutting (Core)
- Wood-fired Crematorium <- Stonecutting (Core)
- Road building <- Stonecutting (Core)
- Heavy Shield Making <- Smithing (Core)
- Legionary Armaments <- Smithing (Core)
- Legionnaire Armor <- Smithing (Core)
- Centurion Armor <- Smithing (Core)
- Scorpion <- Smithing (Core), Recurve Bow (Core)
- Beacons <- Smithing (Core)

#### VFE Tribals

- Replaces all instances of `VFET_ResearchSpot` with `RR_ThinkingSpot`, to avoid any errors when using VFE Tribals and Research Reinvented: Stepping Stones together with any mod that is looking for `VFET_ResearchSpot` (such as Progression: Education)

### Other

#### Progression: Production

NOTE: This patch will soon not be recommended, as this mod will replace Progression: Production in and of itself.

Research Projects:

- Research Bench <- Basic Crafting Facilities (Research Reinvented:Stepping Stones)

### Transparent Substructure

- Transparent Fine Tile, Transparent Substructure, Sky Tile, Fine Sky Tile, Heavy Transparent Bridge <- Glass Blowing (new) <- Smithing (Core)

## Planned Changes

### VE Cooking

- Simple Bake, Fine Bake <- Basic Baking
- Lavish Bake, Gourmet Bake <- Refined Baking
- Simple Dessert, Fine Dessert <- Basic Desserts
- Lavish Dessert, Gourmet Dessert <- Refined Desserts
- Similar for other meal types

### VCE - Carnivore/Vegetarian Meals Patch

Same as for VE Cooking, but for the VCE Carnivore and Vegetarian meals.

### Mods which will not be patched (for now)

- Hospitality (and Casino, Gastronomy, Spa, Storefront, Vending Machines): already well-served by Progression: Hospitality.