# Hub Boilerplate

This code is a template for building Firefox Hub add-ons for Firefox for Android.

For more information about building Hub add-ons, see:
https://developer.mozilla.org/en-US/Add-ons/Firefox_for_Android/Firefox_Hub_Walkthrough

For more information about building mobile add-ons, please see:
https://developer.mozilla.org/en/Extensions/Firefox_on_Android

## Using the Hub Boilerplate

1. Edit `install.rdf`: Please change the ALL CAPS areas with text specific to your add-on.

2. Edit `bootstrap.js`: The current code includes an example of how to add a panel and refresh its data.

3. Edit `chrome.manifest`: Optionally use this to include additional files, including localization files.

4. Edit `config_build.sh`: If you add any additional files, make sure you add them to `config_build.sh`. See `build.sh` for more details.

5. Run `./build.sh`: This creates the XPI and pushes it to your device if you have adb installed.
