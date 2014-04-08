# Framer.js Server
### A local development environment for Framer.js prototypes.
This is a simple gulp.js build designed to help make developing Framer.js prototypes a bit easier.

## Features
- Opens a new browser window pointed at `index.html` (localhost:4000 by default)
- `index.html` automatically refreshes whenever changes are saved to `app.js`
- Prototypes are accessible to other devices on your local network (`ifconfig` to get the IP)
  * These devices are also automatically refreshed when changes are made to `app.js`

## Installation
You'll need to have node & grunt.js installed ([this guide](http://travismaynard.com/writing/getting-started-with-gulp) is a good starting point).

1. `npm install` to grab the Node dependencies
2. `cd` into the project and run the `gulp` command
3. It's happening!

![](http://i.imgur.com/vv49C.gif)

## To do
- ~~Add node-open~~
