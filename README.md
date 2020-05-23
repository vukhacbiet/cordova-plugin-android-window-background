# :snowflake: cordova-plugin-android-window-background :art: :lollipop:

This is a simple plugin for Android which will set the window background color for you app's MainActivity to a color of your choice.
This allows you to avoid the standard dark grey background which will flash for a second before your splash screen appears. Set the color to the same background as your splash screen for a smoother start-up effect.

## My Update
Update To Default Android Theme.

## Installation

You'll need to set your desired window background color while installing the plugin by supplying the `WINDOW_BACKGROUND_COLOR` variable. Set it to whatever you want, preferrably the same color as your splash screen.

    cordova plugin add https://github.com/vukhacbiet/cordova-plugin-android-window-background.git --variable WINDOW_BACKGROUND_COLOR=#ffffff --save

	
## Supported Platforms

- Android (cordova-android 7.0.0+)

## Configuration

A custom `WINDOW_BACKGROUND_COLOR` variable will be added to your app's config.xml after installation with the value you selected (provided you included the `--save` flag).
You can change it whenever you want, but you'll need to remove and re-add the Android platform from your project in order for the change to go through.

    <plugin name="cordova-plugin-window-background">
        <variable name="WINDOW_BACKGROUND_COLOR" value="#B4D455" />
    </plugin>

To re-add the Android platform:

	cordova platform remove android
	cordova platform add android
	
