### [OpenSCAD](https://openscad.org/)

#### Install using Git

1.  Clone the [`OpenSCAD` repository](https://github.com/dracula/openscad):

    ```sh
    git clone https://github.com/dracula/openscad.git
    ```

2.  Move into the cloned repository:

    Linux & Mac:

    ```bash
    cd ./openscad
    ```

    Windows

    ```PowerShell
    Set-Location -Path ".\openscad"
    ```

3.  Create the directories `OpenSCAD/color-schemes/editor` and `OpenSCAD/color-schemes/render` in the application's config directory if they do not exist.

    Linux:

    ```bash
    mkdir -p $HOME/.config/OpenSCAD/color-schemes/editor $HOME/.config/OpenSCAD/color-schemes/render
    ```

    Mac:

    ```bash
    mkdir -p "$HOME/Library/Application Support/OpenSCAD/color-schemes/editor" "$HOME/Library/Application Support/OpenSCAD/color-schemes/render"
    ```

    Windows:

    ```PowerShell
    New-Item -Path "C:\Documents and Settings\$env:username\Local Settings\Application Data\OpenSCAD\color-schemes\editor" -ItemType Directory
    New-Item -Path "C:\Documents and Settings\$env:username\Local Settings\Application Data\OpenSCAD\color-schemes\render" -ItemType Directory
    ```

4.  Finally, create two symbolic links from the local repository to [OpenSCAD](https://openscad.org/)’s editor and render folders:

    Linux:

    ```bash
    ln -s $PWD/dracula.json $HOME/.config/OpenSCAD/color-schemes/editor
    ln -s $PWD/transylvania.json $HOME/.config/OpenSCAD/color-schemes/render
    ```

    Mac:

    ```bash
    ln -s "$PWD/dracula.json" "$HOME/Library/Application Support/OpenSCAD/color-schemes/editor"
    ln -s "$PWD/transylvania.json" "$HOME/Library/Application Support/OpenSCAD/color-schemes/render"
    ```

    Windows:

    ```PowerShell
    New-Item -Path "$pwd\dracula.json" -ItemType SymbolicLink -Value "C:\Documents and Settings\$env:username\Local Settings\Application Data\OpenSCAD\color-schemes\editor"
    New-Item -Path "$pwd\transylvania.json" -ItemType SymbolicLink -Value "C:\Documents and Settings\$env:username\Local Settings\Application Data\OpenSCAD\color-schemes\render"
    ```

#### Install manually

1.  Download the [`OpenSCAD` archive](https://github.com/dracula/openscad/archive/main.zip) and extract it.

2.  Linux:
    Create the directories `OpenSCAD/color-schemes/editor` and `OpenSCAD/color-schemes/render` if it does not exist in `$HOME/.config/`.

    Mac:
    Create the directories `OpenSCAD/color-schemes/editor` and `OpenSCAD/color-schemes/render` if it does not exist in `$HOME/Library/Application Support/`.

    Windows:
    Create the directories `OpenSCAD/color-schemes/editor` and `OpenSCAD/color-schemes/render` if it does not exist in `C:\Documents and Settings\$env:username\Local Settings\Application Data\`.

3.  Move the `dracula.json` file from the extracted archive to [OpenSCAD](https://github.com/dracula/openscad/archive/main.zip)’s `editor` folder, and `transylvania.json` to [OpenSCAD](https://github.com/dracula/openscad/archive/main.zip)’s `render` folder.

#### Activating theme

1. Navigate to `OpenSCAD -> Edit -> Preferences`.
2. Select `3D View -> Color scheme -> Transylvania` as the render theme.
3. Select `Editor -> Color syntax highlighting -> Dracula` as the editor theme.
