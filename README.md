#NativeSettings plugin for Android and iOS 8 Cordova.

The plugin allows you to open Settings view from Android Cordova application and to open Native App settings view from iOS 8 Cordova application. Based on https://github.com/raulduran/VideoPlayer.

##Adding the Plugin to your project

###Example for iOS and Android

```js
if(typeof cordova.plugins.settings.openSetting != undefined){
    cordova.plugins.settings.open(function(){
            console.log("opened settings")
        },
        function(){
            console.log("failed to open settings")
        });
}
```

##Using the plugin for Android

```
cordova.plugins.settings.openSetting(settingName, success_callback, failure_callback);
```

###Example for Android

```js
if(typeof cordova.plugins.settings.openSetting != undefined){
    cordova.plugins.settings.openSetting("nfc_settings", function(){
            console.log("opened nfc settings")
        },
        function(){
            console.log("failed to open nfc settings")
        });
}
```