# my-winget-packages

## Overview
This repository contains a collection of custom packages for the Windows Package Manager (winget). These packages can be used to install software on Windows systems using the winget command-line tool.

## How to Use
1. Clone this repository to your local machine:
    ```sh
    git clone https://github.com/yourusername/my-winget-packages.git
    cd my-winget-packages
    ```

2. Add the local repository to winget:
    ```sh
    winget source add -n my-packages <path-to-repo>
    ```

3. Update the winget sources:
    ```sh
    winget source update
    ```

4. Install a package from this repository:
    ```sh
    winget install <package-name>
    ```

## Packages
The following packages will be installed by the DSC configuration:
- Notepad++: A free source code editor.
- ShareX: A free and open-source screenshot tool.
- Notion: An all-in-one workspace for notes and tasks.
- Visual Studio Code: A source-code editor developed by Microsoft.
- 7zip: A file archiver with a high compression ratio.
- Blender: A free and open-source 3D creation suite.
- Calibre: An open-source e-book management tool.
- Google Chrome: A cross-platform web browser.
- Google Drive: A file storage and synchronization service.
- Handbrake: An open-source video transcoder.
- OBS Studio: Free and open-source software for video recording and live streaming.
- Slack: A messaging app for teams.
- TreeSize Free: A disk space analyzer.
- VLC: A free and open-source media player.
- Epic Games Launcher: A digital distribution platform for video games.
- EA App: A digital distribution platform for EA games.
- Battle.net: A digital distribution platform for Blizzard games.

## Using the DSC Configuration
The `configuration.dsc.yaml` file contains a list of packages to be installed using the Desired State Configuration (DSC) for winget.

1. Ensure you have the necessary DSC modules installed:
    ```sh
    Install-Module -Name Microsoft.WinGet.DSC
    ```

2. Apply the DSC configuration:
    ```sh
    Start-DscConfiguration -Path ./configuration.dsc.yaml -Wait -Verbose
    ```

## Contributing
Feel free to submit issues or pull requests if you have suggestions or improvements.

## License
This project is licensed under the MIT License.

