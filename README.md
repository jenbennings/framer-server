# Framer.js Server
#### A local development environment for Framer.js prototypes.
This is a simple gulp.js build designed to help make developing Framer.js prototypes a bit easier.

## Features
- Opens a new browser window pointed at `index.html` (localhost:4000 by default)
- `index.html` automatically refreshes whenever changes are saved to `app.js`
- Prototypes are accessible to other devices on your local network (use `ifconfig` to get the IP)
  * These devices are also automatically refreshed when changes are made to `app.js`

## Installation
You'll need to have node & grunt.js installed ([this guide](http://travismaynard.com/writing/getting-started-with-gulp) is a good starting point).


1. `cd` to the folder your Sketch file is located and clone the repo
2. `npm install` to grab the node dependencies
3. Run the `gulp` command
4. It's happening!

![](http://i.imgur.com/vv49C.gif) 

### Bonus points: Add [FastClick](https://github.com/ftlabs/fastclick)

> ...mobile browsers will wait approximately 300ms from the time that you tap the button to fire the click event. The reason for this is that the browser is waiting to see if you are actually performing a double tap.

This sucks. Let's get rid of it.

[FastClick](https://github.com/ftlabs/fastclick) comes bundled `custom.js`, along with a function that attaches it to the body of `index.html`

To start using it, modify your `sketch-framer-config.js` (part of the [sketch-framer](https://github.com/bomberstudios/sketch-framer) plugin) to include a reference to `custom.js`.

```js
var FramerLibraryUrl = "custom.js";
var extra_script_line;
var FramerLibraryFileName;
 
if(FramerLibraryUrl) {
  FramerLibraryFileName = FramerLibraryUrl.replace(/^.*(\\|\/|\:)/, '');
  extra_script_line = "\n\t\t<script src=\"" + FramerLibraryFileName + "\"></script>"
}
```

Full Gist [here](https://gist.github.com/jenbennings/10083816).

## To do
- ~~Add node-open~~
- ~~Add fastclick~~
