# Clone
1. Clone and setup the repo (for Ubuntu, more info at [info](https://docs.qgroundcontrol.com/master/en/qgc-dev-guide/getting_started/))
   ```bash
    git clone https://github.com/UAV-Design-Team-2024/qgroundcontrol.git --recursive;
    cd qgroundcontrol;
    git submodule update --recursive;
   ```
# Setup
2. Run setup script, if errors see [info](https://docs.qgroundcontrol.com/master/en/qgc-dev-guide/getting_started/). This must be run in the `qgroundcontrol` directory.
   ```bash
   sudo bash ./tools/setup/install-dependencies-debian.sh;
   ```

# Build
3. Run configure script, do this if you reinstall QT.
    ```bash
    ./configure_auto_build
    ```
    - If you get an error running the script, run the command
        ```bash
        chmod a+x configure_auto_build; ./configure_auto_build;
        ```
4. Run this command to build qgroundcontrol.
   ```bash
   ./build.sh
   ```