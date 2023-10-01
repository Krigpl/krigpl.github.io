Application **Wifi Time Tracker** collects and stores the history of your connections to Wifi networks.
All that data and the other data that the user creates in the application (like labels) is stored on the device only and is not send to any remote servers.

The following two permissions are required for the application to function correctly: `ACCESS_FINE_LOCATION` and `ACCESS_BACKGROUND_LOCATION`. Both access user sensitive information about their location at all times, however the application doesn't collect any data about the user's location. `ACCESS_FINE_LOCATION` permission is required in order to obtain the SSID (network name) of the Wifi network as described in the Android Developer documention [here](https://developer.android.com/reference/android/net/wifi/WifiInfo). `ACCESS_BACKGROUND_LOCATION` is required to track the Wifi network changes while the application is not in the foreground, which will be the case most of the time.
Hence, both permissions are required, but the application doesn't collect nor store the location data.

The application uses Google Firebase Analytics SDK for storing basic events about the app usage (event like "app opened", "app uninstalled", "app crashed", etc). That data is collected in an anynymised fashion.

If you installed this application from Google Play, then Google Play does collect some personal data. Please see the privacy policy for Google Play Services here: https://policies.google.com/privacy
