# photos-sharing-final

# stepts to setup this project

download the project from github (github is a code repository website)

starter project
https://github.com/xdagee/photos-sharing-master

final project
https://github.com/xdagee/photos-sharing-final

extract and import to the project to VS Code
download the project packages and run the app.

configuring the project for firebase ()
create an account if don't have one already
https://console.firebase.google.com

give it a project name
my-photo-sharing-app

add the following package name
com.google.codelab.photos.sharing

add the SHA-1 certificate fingerprint from your debug.keystore

get the SHA-1 certificate fingerprint from your debug.keystore file using keytool from the cli (command line interface)

keytool -alias androiddebugkey -keystore debug.keystore -list -v -storepass android

(if keytool is not recognised, add it to user path)
C:\Program Files\Android\Android Studio\jre\bin

click register app to complete creating your project on firebase developer console

download the google-services.json file and copy it to your project
project-name\android\app\

configure your project to use google services in your app

add google services dependencies to the build.gradle file in project level
project-name\android\ 

classpath 'com.google.gms:google-services:4.2.0'

add firebase dependencies to the build.gradle file in app level
project-name\android\app\
implementation 'com.google.firebase:firebase-core:16.0.9'

finally add gradle plugin to the build.grade file in app level
project-name\android\app\

enable the Google Photos Library API in your project
https://console.developers.google.com/apis/library/photoslibrary.googleapis.com

select your project and enable Google Photos Library API

add OAuth to the Google Photos Library API scope
enter the application name - My Photo Sharing App

select and add the following scopes
https://www.googleapis.com/auth/photoslibrary
https://www.googleapis.com/auth/photoslibrary.sharing

add a support email address and save to complete the process

congrats; you have now successfully added google servies to your app.
google-sign-in
google-photos-library-api