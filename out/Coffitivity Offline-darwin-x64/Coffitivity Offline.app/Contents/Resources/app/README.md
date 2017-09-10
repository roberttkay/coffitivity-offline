# Coffitivity Offline 1.0.0
Coffitivity.com's unofficial desktop app which runs without internet. 🎧 🚀


### Development Setup

To clone and run this repository you'll need [Git](https://git-scm.com) and [Node.js](https://nodejs.org/en/download/) (which comes with [npm](http://npmjs.com)) installed on your computer. We will also be using [Electron Forge](https://electronforge.io/) for building our desktop native app.
Next open up Terminal or your favourite command line tool:

```bash
   # First go to the directory where you want to install Coffitivity Offline
   # Next we'll clone the repository
git clone https://github.com/siwalikm/coffitivity-offline.git
   # install Electron-Forge globally on your system
npm install -g electron-forge
   # Go into the repository
cd coffitivity-offline
   # Install all the dependencies of this project
npm install
   # Run the app
electron-forge start
```
#### Building native app for MacOS
```bash
   # Go into the repository
cd coffitivity-offline
   # Install all the dependencies of this project
npm install
   # Run Build Script
electron-forge make
```
> This creates a compiled dmg file in the folder "../out/make" in your application's root directory.

To edit specificities of the MacOS build, go to your package.json file and edit the following property.

```bash
"electronPackagerConfig": {
        "packageManager": "npm",
        "name": "Coffitivity Offline",
        "icon": "./assets/icon.png.icns"
      },
```