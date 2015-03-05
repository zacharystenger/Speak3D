## Speak3D

Web app that creates 3D stuff when you speak to your browser. 
Created using [three.js](http://threejs.org) and [annyang.](https://www.talater.com/annyang/) 
Built off of the Text3D example in Lee Stemkoski's
[Three.js examples](http://stemkoski.github.io/Three.js/index.html)

[Try the Demo on Google Drive](http://googledrive.com/host/0B5KjNubMIcDvSnNtVnhNemsxd2M/index.html) (only works with Chrome)

## List of Commands & Examples

  - say 'create cube' w/ optional parameters
  - say 'create sphere' w/ optional parameters
  - say 'create ring' w/ optional parameters
  - say 'create knot' w/ optional parameters
  - say 'create cylinder' w/ optional parameters
  - say 'create floor' w/ optional parameters (only has y coordinate right now)
  - say 'create wall' w/ optional parameters (only has x,y coordinate right now)
  - say 'create many cubes/spheres/rings/knots/cylinders' w/ optional parameters, provide amount param and two params on atleast one axis(x,y, or z) or two size params ex: 'create many spheres amount 5 z 0 and 250' or 'create many cubes amount 5 size 10 and 110 transparent true'
  - say 'create text' then say whatever you want
  - say 'undo' or press ctrl+z
  - say 'test everything' to see a bunch of stuff at once
  - optional parameters are x (number), y (number), z (number), size (number), color (color name), transparent (true or false)
  - examples: say 'create cube x 50 y 100 z 100 size 75' or 'create ball size 100 y 150'

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

## List of Color Names

  -antique
  -aqua
  -aquamarine
  -azure
  -beige
  -bisque
  -black
  -blue
  -brown
  -burlywood
  -chartreuse
  -chocolate
  -coral
  -crimson
  -cyan
  -fire
  -forest
  -fuchsia
  -gainsboro
  -ghost
  -gold
  -goldenrod
  -gray
  -grey
  -green
  -honeydew
  -indigo
  -ivory
  -khaki
  -lavender
  -lawn
  -lemon
  -lime
  -linen
  -magenta
  -maroon
  -midnight
  -mint
  -navy
  -olive
  -orange
  -orchid
  -pink
  -plum
  -purple
  -red
  -salmon
  -seashell
  -sienna
  -silver
  -sky
  -snow
  -tan
  -teal
  -thistle
  -tomato
  -turquoise
  -violet
  -wheat
  -white
  -yellow

## To Do

  - a lot
  - export function so users can save whatever they create
  - cli alternative to send commands
  - ability to manipulate & remove existing geometries
  - have start/pause screen that has usage & commands & examples
  - ctrl+z is buggy
  - use updated version of three.js
  - create self command, for third person view
  - better controls to navigate in 3D space
  - textures
  - add parameters for dimensions, rotation, etc.
  - problems with people talking fast
  - geometries in motion
  - more geometries
  - more colors
  - ability to set default parameters for specific geometries 
  - spin(command would be spin x, spin y, spin z)
  - lights, fog, skyBox, etc.
  - built-in models and user uploaded models
  - better debugging
  - usage & list of commands
  - display message when browser does not support speech recognition
  - refactor

## Authors

* Zachary Stenger

## License

MIT

* [http://www.opensource.org/licenses/mit-license.php](http://www.opensource.org/licenses/mit-license.php)