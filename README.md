# photos-sharing-final

# steps to setup this project

# 1.0 download the project from github (github is a code repository website)

# starter project
# https://github.com/xdagee/photos-sharing-master

# final project (completed)
# https://github.com/xdagee/photos-sharing-final

# extract and import to the project to VS Code
# download the project packages and run the app

# 2.0 configuring the project for firebase (Firebase is platform for building web and mobile applications without any backend coding)
# create an account if don't have one already
# https://console.firebase.google.com

# give it a project name
# my-photo-sharing-app

# add the following package name
# com.google.codelab.photos.sharing

# add the SHA-1 certificate fingerprint from your debug.keystore

# get the SHA-1 certificate fingerprint from your debug.keystore file using keytool from the cli (command line interface)

# keytool -alias androiddebugkey -keystore debug.keystore -list -v -storepass android

# (if keytool is not recognised, add it to user path)
# C:\Program Files\Android\Android Studio\jre\bin

# click register app to complete creating your project on firebase developer console

# download the google-services.json file and copy it to your project
# project-name\android\app\

# 3.0 configure your project to use google services in your app

# add google services dependencies to the build.gradle file in project level
# project-name\android\ 

# [code] classpath 'com.google.gms:google-services:4.2.0' [/code] 

# add firebase dependencies to the build.gradle file in app level
# project-name\android\app\
# scrolldown to dependencies and add the following code
# [code] implementation 'com.google.firebase:firebase-core:17.0.0' [/code]

# finally add gradle plugin to the build.grade file in app level
# go down to the last level and add the following code
# project-name\android\app\
# [code] apply plugin: 'com.google.gms.google-services' [/code]

# 4.0 enable the Google Photos Library API in your project
# https://console.developers.google.com/apis/library/photoslibrary.googleapis.com
# ()
# select your project and enable Google Photos Library API

# add OAuth to the Google Photos Library API scope
# enter the application name - My Photo Sharing App

# select and add the following scopes
# [code] https://www.googleapis.com/auth/photoslibrary [/code]
# [code] https://www.googleapis.com/auth/photoslibrary.sharing [/code]

# add a support email address and save to complete the process

# congrats; you have now successfully added google servies to your app.
# google-sign-in
# google-photos-library-api
