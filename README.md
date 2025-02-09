# PlatformIO build any
Small script that converts a PlatformIO project into an Arduino sketch, builds it and uploads it using arduino-cli.\
This was made because the board we are using (Realtek AMB82) is not compatible with PlatformIO, only Arduino IDE.\
This should allow you to use the basic features of PlatformIO with any board compatible with Arduino IDE.\
Just change `board_fqdn`, `board_pid` and `board_vid` in `build-upload.py`. (run `arduino-cli board list --json` for `board_pid` and `board_vid`, `arduino-cli board listall` for `board_fqdn`).\
To use it, put this repo content in your `.vscode` folder, alongside with [arduino-cli](https://github.com/arduino/arduino-cli/releases).