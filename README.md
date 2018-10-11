# Post Pingeon – Ionic 4 messenger app for iOS and Android based on Angular 6 and Firebase

The Post Pingeon is Ionic 4 simple, light-weight messenger application based on Angular 6 and Firebase. You can use it on Android or iOS devices. It is easy to maintain project for your own targets. Project based on default Ionic styleguides.

## Firebase setup

1. Create a Firebase project in the [Firebase console](https://console.firebase.google.com).
2. From the project overview page in the Firebase console, click Add Firebase to your web app. If your project already has an app, select Add App from the project overview page. Change .read and .write values to true.
3. Copy and paste your project's customized code snippet available under Authentication tab then click on Web setup button and initialize your Firebase project with the 5 keys: apiKey, authDomain, databaseURL, projectId, storageBucket, messagingSenderId into src/app/app.module.ts.
4. Click on the Authentication tab and enable firebase password authentication or Google/Twitter/GitHub, Facebook as you like. 

## Start the project

The project is started with the regular ionic commands.

1. Run `npm install` to install all dependencies.
2. Run `ionic serve` to start the development environment.
3. To build the project run `ionic build android` or `ionic build ios`. In order for you to build an iOS app, you need to run on MacOS.

## Project Structure

### main directory
```
.
 ├── resources/                   # This folder contains build files on the specific platforms (iOS, Android) and app icon + splash
 ├── src/                         # This is where the app lives - *the main folder*
 ├── .editorconfig                # This file is a helper file to define and maintain coding styles across environments
 ├── .gitignore                   # This file contains specifies intentionally untracked files to ignore when using Git
 ├── config.xml                   # This file contains ionic config file
 ├── .ionic.config.json           # This file contains global configuration for your Ionic app
 ├── package.json                 # This file contains dependencies and build scripts
 ├── tsconfig.json                # This file contains TypeScript configurations
 └── tslint.json                  # This file contains TypeScript linting options
```

### src directory
```
├── ...
   ├── src                       
   │  ├── app/                    # This folder contains global modules and styling.
   │  ├── assets/                 # This folder contains images and icons.
   |  ├── pages/                  # This folder contains all the individual pages.
   |  ├── providers/              # This folder contains the firebase api services that retrieves data from the Realtime Database.
   |  ├── theme/                  # This folder contains the global SCSS variables to use throughout the app.
   |  ├── index.html              # This file contains the root index app file - This launches the app.
   |  ├── manifest.json           # This file contains metadata for the app.
   │  └── service-worker.js       # This file contains cache configurations.
   └── ...
```
