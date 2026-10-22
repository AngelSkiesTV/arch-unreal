# DAZ -> Unreal pipeline

Dropbox currently has no DAZ exports (only shortcuts to DAZ Studio / Install Manager). Drop new exports in Dropbox at **/AngelSkies/DAZ_Exports/<CharacterName>/** and they get organized here.

## Export from DAZ Studio 4.21
Easiest: install **DAZ to Unreal Bridge** (free, via DAZ Install Manager) > File > Send To > Daz to Unreal. It sends straight into Content/ARCH/Characters.

Manual FBX:
1. File > Export > FBX, version **FBX 2014 Binary**
2. Tick: Figures, Props, Morphs (only needed ones), Collapse UV Tiles. Untick: Lights, Cameras
3. Save to DAZ_Exports/<CharacterName>/<CharacterName>.fbx with its textures/ folder beside it

## Import into Unreal
Drag the .fbx into Content/ARCH/Characters/<CharacterName>. Skeletal Mesh on, Import Morph Targets on, Import Uniform Scale 1.0, Convert Scene on.
For Quest: reduce textures to 2K, use LODs, keep characters under ~50k triangles.

## Folder layout
DAZ_Exports/
  <CharacterName>/
    <CharacterName>.fbx
    textures/
