# Cohesive Research: A Stepping Stones Project

- [Cohesive Research: A Stepping Stones Project](#cohesive-research-a-stepping-stones-project)
    - [Overview](#overview)
    - [New Research Projects](#new-research-projects)
    - [Mod Patches](#mod-patches)
        - [Vanilla Expanded](#vanilla-expanded)
            - [VFE Classical](#vfe-classical)
            - [VFE Tribals](#vfe-tribals)
        - [Other](#other)
            - [Progression: Production](#progression-production)
        - [Transparent Substructure](#transparent-substructure)
    - [Planned Changes](#planned-changes)
        - [Dubs' Bad Hygiene](#dubs-bad-hygiene)
        - [VE Cooking](#ve-cooking)
        - [VCE - Carnivore/Vegetarian Meals Patch](#vce---carnivorevegetarian-meals-patch)
        - [Mods which will not be patched (for now)](#mods-which-will-not-be-patched-for-now)

## Overview
Cohesive Research is a collection of patches in the vein of [Research Reinvented: Stepping Stones](https://steamcommunity.com/sharedfiles/filedetails/?id=2868389782), increasing cohesiveness and compatibility with Stepping Stones' more individualized research projects.

## New Research Projects

Each new research project will only be added if it is required by a [Mod Patch](#mod-patches).

- Glass Blowing <- Smithing (Core)
- Simple Hygiene <- Simple Waterworks (Cohesive Research)
- Simple Waterworks <- Structures (RR: Stepping Stones), Simple Furniture (RR: Stepping Stones)
- Complex Hygiene <- Plumbing (Dubs Bad Hygiene)
- Complex Waterworks <- Plumbing (Dubs Bad Hygiene)

## Mod Patches

Key: Research Project(s)/Thing(s)/Recipe(s) <- New prerequisite Research Project (source mod)

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

Things:

- Transparent Fine Tile, Transparent Substructure, Sky Tile, Fine Sky Tile, Heavy Transparent Bridge <- Glass Blowing (Cohesive Research)

## Planned Changes

### Dubs' Bad Hygiene

Plumbing is split up into multiple chunks (pipes, waterworks, hygiene), with simple and complex levels. Simple Hygiene and Simple Waterworks are required for building basic latrines and wells (already unlocked in Neolithic starts and above).

Tweaks:

- Rename: Heating -> Water Heating
- Rename: Central Heating -> Plumbed Water Heating
- Rename: Geothermal Heating -> Geothermal Water Heating

Things:

- Latrine, Water Tub <- Simple Hygiene (Cohesive Research)
- Primitive Well <- Simple Waterworks (Cohesive Research)
- Water Trough <- Simple Waterworks (Cohesive Research)
    - If VE Tribals is installed: Water Trough <- Simple Waterworks (Cohesive Research), Animal Husbandry (VE Tribals)
- Basin, Bathtub <- Complex Hygiene (Cohesive Research)
- Water butt, Water Tower, Water Well, Wind Pump <- Complex Waterworks (Cohesive Research)

Research Projects:

- Plumbing <- Simple Waterworks (Cohesive Research), Smithing (Core)
- Water Heating <- Simple Waterworks (Cohesive Research), Fire (RR: Stepping Stones)

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
- Firefoam things: default researches (tied to Core's Firefoam and Gunsmithing) are pretty reasonable.