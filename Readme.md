# Svelte Native

## Steps to create and run app

- `npm install -g nativescript`
- `npx degit halfnelson/svelte-native-template app-name`
- `cd app-name`
- `npm install`
- Edit `app/App_Resources/iOS/build.xcconfig`
- Uncomment the line that starts with "DEVELOPMENT_TEAM ="
  and set it to your team name (ex. "Mark Volkmann (Personal Team)")
- Edit `platforms/ios/Pods/Pods.xcodeproj/project.pbxproj`
- Change all the lines that set `IPHONEOS_DEPLOYMENT_TARGET`
  to use a newer version than 8.0 such as 14.0.
- To see a list of available device simulators, enter
  ``.
- To run the app as iOS, enter `ns run ios --device "{device-name}"`.
  For example, `device-name` can be `iPhone 13`.
- To run the app as Android, enter `ns run android`.

Other commands include `ns preview` and `ns build`.

## Modifying the app

Start by editing `app/App.svelte`.
When changes are saved, Webpack builds and re-bundles the entire app
and copies it to the simulator, and re-renders the app.
This takes about four seconds.
