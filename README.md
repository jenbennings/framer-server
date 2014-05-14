# Framer.js Server
#### A local development environment for Framer.js prototypes.
This is a simple node/gulp.js build designed to help make developing Framer.js prototypes a bit easier. So far this only works with [Sketch Framer](https://github.com/bomberstudios/sketch-framer) output.

## Features
- `index.html` automatically refreshes whenever changes are saved to `app.js`
- Prototypes are accessible to other devices on your local network (use `ifconfig` to get the IP)
  * These devices are also automatically refreshed when changes are made to `app.js`

## Installation
You'll need to have node & grunt.js installed ([this guide](http://travismaynard.com/writing/getting-started-with-gulp) is a good starting point).

1. Clone this repo into the same folder as your Sketch Framer output
2. `npm install` to grab the node dependencies
3. Run the `gulp` command
4. It's happening!

![](http://i.imgur.com/vv49C.gif)
