# Cohesive Research: A Stepping Stone Project

Cohesive Research is a collection of patches in the vein of [Research Reinvented: Stepping Stones](https://steamcommunity.com/sharedfiles/filedetails/?id=2868389782), increasing cohesiveness and compatibility with Stepping Stones' more individualized research projects.

## Changes

Key: Research Project/Thing/Recipe <- New prerequisite Research Project (source mod)

### Progression: Production

NOTE: This patch will soon not be recommended, as this mod will replace Progression: Production in and of itself.

Research Projects:

- Research Bench <- Basic Crafting Facilities (Research Reinvented:Stepping Stones)

### VFE Classical

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

### VFE Tribals

- Replaces all instances of `VFET_ResearchSpot` with `RR_ThinkingSpot`, to avoid any errors when using VFE Tribals and Research Reinvented: Stepping Stones together with any mod that is looking for `VFET_ResearchSpot` (such as Progression: Education)

## Planned Changes

### VE Cooking

- Simple Bake, Fine Bake <- Basic Baking
- Lavish Bake, Gourmet Bake <- Refined Baking
- Simple Dessert, Fine Dessert <- Basic Desserts
- Lavish Dessert, Gourmet Dessert <- Refined Desserts
- Similar for other meal types

### VCE - Carnivore/Vegetarian Meals Patch

Same as for VE Cooking, but for the VCE Carnivore and Vegetarian meals.

### Transparent Substructure

- Adds Glass Blowing (new) as a prerequisite for transparent foundations, substructures, and floors.

### Mods which will not be patched (for now)

- Hospitality (and Casino, Gastronomy, Spa, Storefront, Vending Machines): already well-served by Progression: Hospitality.