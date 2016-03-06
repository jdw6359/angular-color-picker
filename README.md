# angularjs-color-picker


AngularJS Color Picker Directive

## Installation

#### Bower

```shell
bower install angularjs-color-picker --save
```

#### Npm
```shell
npm install angularjs-color-picker --save
```

#### Usage

* Include tinycolor2.js, angularjs-color-picker.js and angularjs-color-picker.css
```html
<link rel="stylesheet" href="bower_components/angular-color-picker/dist/angularjs-color-picker.min.css" />
<!-- only include if you use bootstrap -->
<link rel="stylesheet" href="bower_components/angular-color-picker/dist/themes/angularjs-color-picker-bootstrap.min.css" />
<script src="bower_components/tinycolor2/dist/tinycolor2-min.js"></script>
<script src="bower_components/angular-color-picker/dist/angularjs-color-picker.min.js"></script>
```


* Add the module to your app
```javascript
angular.module('app', ['color.picker']);
```

* Include in your view
```html
<color-picker ng-model="myColor"></color-picker>
```

## Options

If a list is given then choose one of the items. The first item in the list will be the default.
```html
<color-picker
    ng-model="" <!-- only required field -->
    color-picker-format="'hsl', 'hsv', 'rgb', 'hex', 'hex8'"
    color-picker-alpha="true, false"
    color-picker-swatch="true, false"
    color-picker-swatch-pos="'left', 'right'"
    color-picker-swatch-bootstrap="true, false"
    color-picker-swatch-only="true, false"
    color-picker-pos="'bottom left', 'bottom right', 'top left', 'top right'"
    color-picker-case="'upper', 'lower'"
    color-picker-on-change="onColorChange($event, color)"
></color-picker>
```

## Requirements

* angularjs (v1.3 and higher)
* tinycolor2.js (18.8 KB minified)

NO requirement for jQuery!

## Inspiration

Inspiration and code taken from projects like
* http://kaihenzler.github.io/angular-minicolors/
* http://mjolnic.github.io/bootstrap-colorpicker/
* https://github.com/buberdds/angular-bootstrap-colorpicker/
