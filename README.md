# Rockicon
## Rocky Identicons

It is a fork of (jazzicon)[https://github.com/danfinlay/jazzicon] with ability to set colors palette from outside.

## Installation

```
npm install rockicon -S
```

## Usage

Takes a color palette, a pixel diameter and a javascript integer (seeds the shape), and gives you back a DOM element to use as you wish!

```javascript
var colors = [
	'#5bdd95',
  '#5bddcf',
  '#47b1ee',
  '#3677ee',
  '#7e27d0',
  '#631fa3',
  '#d025ce',
  '#f12498',
  '#f1611a',
  '#f8c013',
]
var rockicon = require('rockicon')
rockicon.setColorsPalette(colors)
var body = document.querySelector('body')
for(var i = 0; i < 60; i++) {
  var el = rockicon.generateIdenticon(100, Math.round(Math.random() * 10000000))
  body.appendChild(el)
}
```

## Example

You can run an example by installing beefy (`npm i -g beefy`) and then running `npm start`.
