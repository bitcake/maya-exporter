## BitCake's Maya Exporter

# Install Instructions

1. Copy the entire `/maya/` folder into your `/documents/maya/` folder
1. Open up the script editor in Maya and type (on the mel tab):
    - `source "bitcake_exporter"; bitcake_exporter_install;`
1. Two buttons will be automatically created on your current shelf with the correct Icons.

# How to use

The first button will open a window with options for you to choose from when exporting your animation.
Don't forget to choose your `character` and `animation` names! The `export directory` can be inside Unity's Asset folder.
Once you choose the export options, click the `Export` button at the end and a `.fbx` file will be saved to the `Export Directory`.

The second button is a "quick export" button. Once pressed, it will export the `.fbx` with your saved export preferences.
