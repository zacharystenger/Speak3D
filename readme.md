## Speak3D

Web app that creates 3D stuff when you speak to your browser. 
Created using [three.js](http://threejs.org) and [annyang.](https://www.talater.com/annyang/) 
Built off of the Text3D example in Lee Stemkoski's
[Three.js examples](http://stemkoski.github.io/Three.js/index.html)

[Try the Demo on Google Drive](http://googledrive.com/host/0B5KjNubMIcDvSnNtVnhNemsxd2M/index.html) (works with Chrome)

## List of Commands & Examples

  - say 'create cube' or 'create bubble cube' w/ optional parameters
  - say 'create sphere' or 'create bubble' w/ optional parameters
  - say 'create ring' w/ optional parameters
  - say 'create knot' or 'create bubble knot' w/ optional parameters
  - say 'create cylinder' or 'create cone' w/ optional parameters
  - say 'create floor' w/ optional parameters (only has x,y,size right now)
  - say 'create wall' or 'create back wall' w/ optional parameters (only has x,y,size right now)
  - say 'create many cubes/spheres/rings/knots/cylinders/floors/walls' w/ optional parameters, provide amount param and two params on atleast one axis(x,y, or z) or two size params ex: 'create many spheres amount 5 z 0 until 250' or 'create many cubes amount 5 size 10 until 110 transparent true'
  - say 'create text' then say whatever you want
  - say 'set default' w/ parameters ex: 'set default transparent true color blue' or 'set default amount 10 size 20 x 0 until 200'
  - say 'undo' or press ctrl+z
  - say 'open console' or press 'o' to submit typed out commands in the top right corner(submit with enter); say 'close console' to close it
  - say 'test' or 'test everything' to see a bunch of stuff at once

## Parameters

  - 'x','y', or 'z' followed by a number
  - 'size' or 'width' followed by a number
  - 'color' or 'ambient' followed by a color name
  - 'texture' followed by a texture name
  - 'transparent' followed by a 'true' or 'false'
  - 'spin' followed by 'x', 'y', or 'z'
  - 'move' followed by a range of 'x', 'y', or 'z', ex: move x 0 until 250
  - you can set a parameter range by using the keyword until, ex: create many cubes x 0 until 100

## Examples

  - say 'create cube color blue'
  - say 'create knot width 9 texture cloud'
  - say 'create cube x 50 y 100 z 100' 
  - say 'set default transparent true size 50 until 100', then 'create many spheres color magenta'
  - say 'set default texture random', then 'create floor', then 'create many walls x -500 until 500'


##Usage

  - enunciate all your words clearly
  - leave a pause between commands
  - wait a few seconds to see if anything renders before retrying a command
  - you can look at the console log (ctrl+shift+c) to see if your Speak3D commands and parameters are being picked up properly
  - leave a slight pause between words
  - to use negative numbers you can say 'negative' or 'minus' followed a number, do not pause between these words
  - example (.. represents a slight pause): say 'create cube .. size .. one hundred fifty .. x .. minus twenty five'

## If you want to run on your server 

You'll need [nodejs](http://nodejs.org/) installed
  - Clone to your machine
  - run npm install from your CLI
  - run node server.js command
  - Open localhost:9000 in a Chrome browser
  - Allow microphone access
  - Speak to your browser

## [List of Color Names](https://github.com/zacharystenger/Speak3D/blob/master/current_color_list.md)

## List of Texture Names
  
  -alloy
  -brick
  -carving
  -checkers
  -chipped
  -chrome
  -cloud
  -crate
  -dirt
  -electric
  -glow
  -grass
  -hearts
  -lava
  -moon
  -paper
  -rock
  -rocky
  -rope
  -sand
  -snow
  -water
  -wood

## To Do


  - add dat.GUI, for default params
  - ability to reset/clear default params
  - GUI for user uploaded textures and models
  - add parameters for dimensions, rotation, etc.
  - improve cli's auto-complete
  - improve cli w/ list of recently submitted commands
  - ability to manipulate & remove existing geometries, incl. voice command to stop all motion
  - enhance start/pause screen
  - export function, add option that generates three js code
  - add random as an option, ex: color random, size & coordinates also
  - esc from pointer lock when mouse is in motion can cause camera to be angled somewhere else
  - ctrl+z is buggy
  - use updated version of three.js
  - bug when loading more than one mirror from file
  - bug with create many w/ mirror material (cameras)
  - create self command, for third person view
  - when creating many geometries w/ one command, morph them into one geometry (maybe when amount >= a certian amount)
  - better controls to navigate in 3D space
  - problems with people talking fast
  - more geometries
  - more colors and textures
  - ability to set default parameters for specific geometries 
  - lights, fog, skyBox, etc.
  - built-in models and user uploaded models
  - better debugging
  - display message when browser does not support speech recognition
  - refactor

## Authors

* Zachary Stenger

## License

MIT

* [http://www.opensource.org/licenses/mit-license.php](http://www.opensource.org/licenses/mit-license.php)