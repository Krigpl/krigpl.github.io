Application **Wifi Time Tracker** collects and stores the history of your connections to Wifi networks.
All that data and the other data that the user creates in the application (like labels) is stored on the device only and is not send to any remote servers.

The following two permissions are required for the application to function correctly: `ACCESS_FINE_LOCATION` and `ACCESS_BACKGROUND_LOCATION`.

`ACCESS_FINE_LOCATION` permission is required in order to obtain the SSID (network name) of the Wifi network as described in the Android Developer documention [here](https://developer.android.com/reference/android/net/wifi/WifiInfo). Without it the app will show "unknown ssid" instead of the network name. 

`ACCESS_BACKGROUND_LOCATION` is required to start tracking the network changes automatically after the phone powers on ([Android Developer documentation](https://developer.android.com/guide/components/foreground-services#bg-access-restrictions)). Without it the app will again show only "unknown ssid" until the user opens it for the first time after boot. 

Both permissions are required to provide the best user experience, however it's possible to use the app without the latter, if the user will always remember to open the app after each phone boot.
At the same time, the application doesn't access/collect the user's location in any other way (e.g. GPS coordinates), permissions are required only for the purpose of obtaining the wifi network name. 

The application uses Google Firebase Analytics SDK for storing basic events about the app usage (event like "app opened", "app uninstalled", "app crashed", etc). That data is collected in an anynymised fashion.

If you installed this application from Google Play, then Google Play does collect some personal data. Please see the privacy policy for Google Play Services here: https://policies.google.com/privacy
