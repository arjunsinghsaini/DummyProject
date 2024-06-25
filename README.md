# cooking_genie
nt for a Flutter application.

A few resources to get you started if this is your first Flutter project:

- [Lab: Write your first Flutter app](https://flutter.dev/docs/get-started/codelab)
- [Cookbook: Useful Flutter samples](https://flutter.dev/docs/cookbook)

For help getting started with Flutter, view our
[online documentation](https://flutter.dev/docs), which offers tutorials,
samples, guidance on mobile development, and a full API reference.

For enable background service in android

/*For background location service in Genie app,
  1. comment flutter_background_geolocation in pubspec.yaml
  2. Comment in CookinGenie app file for initIosLocationService method and imported library for flutter_background_geolocation
  3. Comment in LocationUtil methods - updateFirebaseDatabase, startIosLocationService and backgroundLoc.BackgroundGeolocation.stop(); line*/

//External Libraries -> Flutter background service ->
<service
            android:enabled="true"
            android:exported="true"
            android:name=".BackgroundService"
            android:foregroundServiceType="location"
            />
