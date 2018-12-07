# Cordova Process d' Installation #

## Les Besoins :
* nodjs : https://nodejs.org/en/
* Java (au moins Jdk ) : https://www.oracle.com/technetwork/java/javase/downloads/jre8-downloads-2133155.html
* Android Studio :https://developer.android.com/studio/
* La Version 27 Android SDK via Android Studio: https://developer.android.com/studio/intro/update#sdk-manager
* npm : Le package manager installer par défaut avec Nodejs.

## Les Etapes :
Ouvrir un Terminal dans le dossier du Projet
On installe cordova grace au package manager npm:
### Pour MacOs Linux
    sudo npm install -g cordova
### Pour Windows :
    npm install -g cordova

### Creation D'une APP "hello"
    cordova create hello com.example.hello HelloWorld

## Ajouter une ou des Plateformes

pour ajouter la plateforme android :

    cordova platform add android

pour ajouter une plateforme type browser

    cordova platform add browser

pour voir les plateformes installées dans nôtre projet et celle disponible :

    cordova platform ls

renvoit une liste comme ci-dessous:

    Installed platforms:
    android 7.1.4
    browser 5.0.4
    ios 4.5.5
    Available platforms: 
    osx ~4.0.1
    windows ~6.0.0


## "CheckLister" les dépendences vitales au projet :

Il peut être intéressant de vérifier avant tout si toutes les dépendances utilisées par cordova sont bien installées.

    cordova requirements

Le terminale renverra une checklist:
    
     Requirements check results for android:
    Java JDK: installed .
    Android SDK: installed
    Android target: installed android-19,android-21,android-22,android-23,Google Inc.:Google APIs:19,Google Inc.:Google APIs (x86 System Image):19,Google Inc.:Google APIs:23
    Gradle: installed

    Requirements check results for ios:
    Apple OS X: not installed
    Cordova tooling for iOS requires Apple OS X
    Error: Some of requirements check failed


## Build de l'APP 

Pour "builder" l'app sous android par exemple :

    cordova build android

Pour le browser :
   
     cordova build browser

Pour toutes les plateformes en même temps :

    cordova build


## Run L'APP

Pour android 
 Penser a brancher un smartphone en mode dev. 

    cordova run android

pour le browser :
 
    cordova run browser

Pour toutes les plateformes en même temps :

    cordova run


Le code source se situe par défaut dans le fichier html index.html dans le dossier www.


  