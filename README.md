# ESP-AT

[doc-latest]: https://img.shields.io/badge/docs-latest-blue
- [ESP-AT README](./README_EN.md)

For AT commands available to the host mcu, see the [AT Command Set (v3.4.0.0)](https://docs.espressif.com/projects/esp-at/en/release-v3.4.0.0/esp32/AT_Command_Set/index.html)

# To Build
Follow steps here [Compile ESP-AT Project Locally](https://docs.espressif.com/projects/esp-at/en/latest/esp32/Compile_and_Develop/How_to_clone_project_and_compile_it.html)

# Introduction 
To push changes to `bitbucket`: 
    
    git push bitbucket master

To update from original `repo` (`github`)

    git fetch upstream
    git merge upstream/master

# Tools
[esp_idf_5.2.2](https://videndumplc.sharepoint.com/:f:/r/sites/VitecProductionSolutionsEngineering/Shared%20Documents/General/Engineering%20Tools%20and%20Applications/esp32/esp_idf_5.2.2?csf=1&web=1&e=UZdDu2)

# Bin Generation

Once the changes are made, build the project from the `ESP-IDF`, using `python build.py build` or `python build.py all`
    
    Note: use ESP-IDF version >= 5.2

The combined application `bin` will be in the `.\build\factory` dir, `factory_WROOM-32.bin`.

    NOTE: factory_WROOM-32.bin is used for first time production programming.

The file used for `ota` will be in the `.\build\` dir, `esp-at.bin`. 
    
    NOTE: esp-at.bin is used for field updates via `ota` AT command.
