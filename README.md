# Framer.js Server
### A local development environment for Framer.js prototypes.
This is a simple gulp.js build designed to help make developing Framer.js prototypes a bit easier.

## Features
- `index.html` updates automatically in your browser whenever changes are saved to `app.js`
- Your prototypes are accessible to other devices on your local network (`ifconfig` to get the IP)
  * These devices are also updated when changes are made to `app.js`

## Installation
You'll need to have node & grunt.js installed ([this guide](http://travismaynard.com/writing/getting-started-with-gulp) is a good starting point).

1. `npm install` to grab the Node dependencies
2. `cd` into the project and type `gulp`
3. It's happening!

![](http://i.imgur.com/vv49C.gif)

## To do
- Add node-open