# Changelog

## 1.92
### General

- **Zen UV now works** not only in Edit Mode but also **in Object mode**. The following functions are available in Object Mode: Advanced UV Maps, UV Coverage, Checker Map, Texel Density Checker.
- **Added Texel Density category.** Get, Set, and Check Texel Density of UV Islands.
- Updated **Checker Map category**. Add your own textures, filter existing textures by resolution, square and rectangular formats.
- Updated **UV Maps category**. Now you can work on UV Maps of the selected objects in sync.

### Operators
#### **Advanced UV Maps**

- Added **Sync UV Maps operator.** Now you can duplicate, remove, clean and rename UV Maps of the selected objects in sync.
- Added **Rename UV Map** operator with pattern UV_Channel_* to keep the right order of UV Maps during export.
  
#### **Unwrap**

- Fixed **Zen Unwrap** operator. Now it ignores Islands tagged as Finished.
- Updated **Quadrify Islands** operator. Islands with the same geometry get the same unfolding.

#### **Pack**

- Added **UV Coverage** operator. It helps to determine the percentage of UV Map coverage.

#### **Checker Map**

- Added **Filters** to filter existing textures by resolution, square and rectangular formats.
- Added the possibility to add custom Checker textures and texture libraries.


## 1.9
### General

- **Zen UV now works with multiple objects!**
- Added **Finished System.** It helps to control and manage the state of unwrapping UV Islands (Finished/Unfinished) by tags and visually. Nothing will be left not unwrapped!
- Updated **Checker System.** Now it is based on nodes and contains textures designed specifically for Zen UV. Custom textures can be added easily by the user at the node level.
- Added **UV Maps Properties Tab** to have quick access to UV Maps management.
- Updated **Quadrify** operator. Now it is based on the native **Follow Active Quad** operator and sets the base polygon size based on the average size of current islands.
- **Redesigned UI** to support current and all new updates.

### UI

#### **Main Menu**

- The interface has been completely redesigned and operators have been classified and divided into the following groups:

Operator | Function
:---|:---
    **UV Maps**  |          Selecting and managing UV maps. 
    **Unwrap**    |           Marking and unwrapping operations.
    **Select**   |               Edges/Islands selection operations.
    **Pack**      |               Pack operations.
    **Checker Map**   |   Display control of Checker textures.
    **Preferences**    |     Hotkeys and other general settings.
    **Help**            |        Documentation and support section.

<br>
- Operators options were hidden under the **Settings icons** to optimize space.

#### **Pie Menu:**

- Alternative **CTRL** operators **Pin/Unpin Islands** were replaced by **Tag Finished/Unfinished** from the new powerful **Finished System**. (Sector 4 and Sector 6).
- Added new alternative **CTRL** operator **Select Flipped Islands** to **Select Islands** (Sector 7).
- Added icons for **Quadrify Islands** and **Checker Texture (Toggle)** operators.

#### **Pop Up Menu:**

- All operator options were removed from the Pop Up menu, you can adjust them only in the Main menu. The order of operators is consistent with the Main menu.

### Operators

#### **UV Maps**

- Added **UV Maps Properties Tab** to have quick access to UV Maps management.

#### **Unwrap**

- Added **Tag Unwrapped** option for **Zen Unwrap** operator.
- Added **Sort Unwrapped** option for **Zen Unwrap** operator.
- Added **Auto UV Sync** option for **Zen Unwrap** operator.
- Added **Unwrap Method** option for choosing Unwrap algorithm.
- **Zen Unwrap** now is using the packing algorithm selected in **Pack Engine**.
- Added a warning for the **Marking System** when both **Mark Seams** and **Mark Sharp Edges** options are off.
- Fixed **Smooth by Sharp (Toggle)** operator**.** Now its use ****does not require re-switching.
- Added **Finished System**. It has absorbed **Pin System** and was made to control and manage the state of unwrapping UV Islands (Finished/Unfinished) by tags and visually. Tags can be assigned manually or automatically after unwrapping. Islands can be sorted and pinned by state in UV Editor. You can check the state of Islands in the viewport by using **Display Finished (Toggle)** operator. Nothing will be left not unwrapped!
- Updated **Quadrify** operator. Now it is based on the native **Follow Active Quad** operator and sets the base polygon size based on the average size of current islands.

#### **Select**

- Updated **Isolate Islands (Toggle)** operator. Isolation mode now is working for any selection mode — Vertex/Edge/Polygon. It no longer requires you to select at least one Vertex/Edge/Polygon in order to return back.
- Added **Select Flipped Islands** operator.
- Added **Select Sharp Edges** operator.
- Added **Select Seam Edges** operator.
- **Select Edge Loop** operator ****name ****was changed to **Select Interseam Loop**.

#### **Pack**

- Added **Rotate Islands** option for **Pack Islands** operator.

#### **Checker Map**

- Updated **Checker System**. Now it has 2 types of texture checker - color and monochrome. Each type has 4 sizes. Custom textures can be added easily by the user at the node level.. The **Reset Checker** operator will return the **Checker System** to its initial state.
- Added **Show Image In UV Editor** option. It allows you to turn off the display of texture in the UV Editor.
- Added **Remove Checker Nodes** operator. It removes all checker nodes from the scene to not interfere with the export.

#### **Preferences**

- **Reset Preferences** now returns Auto Mark operator angle settings to their default values.

#### **Help**

- Added information about the current Zen UV version number at the end of the section.

## 1.8
- Added Selected Only option to Zen Unwrap. It’s the separate workflow where only Selected Faces will be Unwrapped and Packed. It includes warnings and Unwrapping options if nothing is selected.
- Added Islands Offset option to Zen Unwrap. It’s available after activating Selected Only. Adds the ability to move inactive islands in the UV viewport to the left when working with Zen Unwrap operator.
- Auto Seams changed to Auto Mark. Zen UV now marks both Sharp Edges and Seam Edges. What exactly to mark can be configured in the panel using Mark Seams and Mark Sharp Edges checkboxes. In fact, this means that with Zen UV you can not only map, but also use it exclusively for the Sharp Edges marking.
- Auto Mark now has the possibility to change the angle. Works in interactive mode.
- Added Mark Seams by Sharp Edges option.
- Added Mark Sharp Edges by Seams option.
- Added Pack After Quadrify option which automatically Pack Islands after Quadrify Islands operation.
- Added Pack Islands option. Also can be found in the Pie menu as alternative command in sector 9 (Zen Unwrap).
- Added Margin option which allows to set space between Islands for Pack Islands operation.
- Added Average Islands Scale option which averages Islands scale before Pack Islands operation.
- Added the possibility to choose Pack Engine.
- Added option to use UVPackmaster 2 Pack Engine if it’s installed on the system.
- Added Select Edge Loop option which allows to select edge loops with Seams respect.
- Added Auto Fit UV View option which automatically Fit and Zoom UV viewport.
- Added Show Bevel Weight and Show Crease Edges options due to the probability of overlapping displayable edge types.
- Added Reset Preferences button to reset all the settings to default state.
- The addon preferences moved from the scene properties to the addon properties. This allows to remember settings between sessions.
- Fully reworked Main and Popup menus, structure and design.
- Fixed the loading icons bug that occurs on some systems.

## 1.7
- Bugfix

## 1.65
- Start!

## 1.64
- Bugfix
- UI Improve