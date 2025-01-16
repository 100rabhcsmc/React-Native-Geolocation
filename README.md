# React Native Geolocation

**Prerequisites**
**Installation**
First, install the `react-native-geolocation-service` package by running:

```bash
npm install react-native-geolocation-service
```

After installation, for iOS, make sure to run:

```bash
npx pod-install
```

**Android Configuration**
To access the device's location on Android, you need to request permissions by updating the AndroidManifest.xml file.

Add the following permissions to the file:

```bash
<uses-permission android:name="android.permission.ACCESS_FINE_LOCATION" />
<uses-permission android:name="android.permission.ACCESS_COARSE_LOCATION" />
<uses-permission android:name="android.permission.ACCESS_BACKGROUND_LOCATION"/>
```

**iOS Configuration**
For iOS, permissions need to be added to the Info.plist file to access the device's location.

Add the following keys to your Info.plist:

```bash
<key>NSLocationWhenInUseUsageDescription</key>
<string>We need access to your location to provide personalized services.</string>

<key>NSLocationAlwaysUsageDescription</key>
<string>We need access to your location even when the app is in the background.</string>

<key>NSLocationAlwaysAndWhenInUseUsageDescription</key>
<string>We need your location at all times to offer seamless services.</string>
```

By following these steps, you’ll be able to access the user's `latitude` and `longitude` efficiently.
