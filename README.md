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

4. Edit `build`: Update this file to specify a file name for your XPI, as well which version of Firefox you want to use to test the XPI file.

5. Run `./build`: This creates an XPI in your source directory and pushes it to your device. You must have [adb](http://developer.android.com/tools/help/adb.html) installed for the push step to work.

## Using volo

You can use [volo](http://volojs.org/) to quickly bootstrap your add-on from this template.

volo requires [node](http://nodejs.org/) to run. To install volo:

    npm install -g volo

After installing volo, to create a new directory for your add-on, run:

    volo create youraddon https://github.com/leibovic/hub-boilerplate/archive/master.zip

This will create a new directory `youraddon`, which holds all the files for your add-on.

