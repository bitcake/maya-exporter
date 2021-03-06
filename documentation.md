# Install Instructions

1. Copy the downloaded `maya/` folder into your preferences folder:
    - Windows: `Documents/maya/`
    - MacOS: `Library/Preferences/Autodesk/maya/`
1. Open up the script editor in Maya and type (on the mel tab):
    ```
    source "bitcake_exporter";
    bitcake_exporter_install;
    ```
1. Two buttons will be automatically created on your current shelf with the correct Icons.


# The Shelf Buttons

![BitCake Exporter Shelf Buttons](images/shelfbuttons.png)

The first button will open a window with options for you to choose from when exporting your animation.
Don't forget to choose your `character` and `animation` names! The `export directory` can be inside your engine's project folder.
Once you choose the export options, click the `Export` button at the end and a `.fbx` file will be saved to the `Export Directory`.

The second button is a "quick export" button. Once pressed, it will export the `.fbx` with your saved export preferences.


# The Exporter UI

![BitCake Exporter Screenshot](images/screenshot.png)

## Main

Field | Description
--- | ---
Character | The character part of the exported fbx filename
Animation | The animation part of the exported fbx filename
Export Directory | The directory where the exported fbx file will be saved on

*The resulting filename will be `<character>@<animation>.fbx`

## Options

### Frames

Field | Description
--- | ---
Use timeline range | All frames in the entire timeline will be used when exporting
Set start and end frames | Only frames inside `Start Frame` and `End Frame` frames will be used when exporting

### Meshes

Field | Description
--- | ---
No mesh | Only joints and animation data will be exported
All meshes | All meshes in the scene will be included in the export
Selected meshes | Only selected meshes will be included in the export
Only skinned meshes | Only skinned meshes will be included in the export
Except skinned meshes | All meshes except skinned meshes will be included in the export

### Joints

Field | Description
--- | ---
Delete | All joints that include these tags (separated by `,`) will be deleted on export
Ignore Bake | All joints that include these tags (separated by `,`) won't be baked to the exported animation

---

*All these fields are saved to the scene file. By doing so, it is not needed to retype them everytime the exporter is opened.*
