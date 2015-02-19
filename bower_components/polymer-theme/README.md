# Polymer Theme

Polymer theme using [Sass](http://sass-lang.com) and
[Material Design](http://www.google.com/design/spec/material-design/introduction.html) language.

For scaffolding Polymer apps use [Polymer Base Template](https://github.com/StartPolymer/polymer-base-template)
or [Yeoman generator](https://github.com/yeoman/generator-polymer).

## Installation

### Bower Component

```sh
bower install polymer-theme --save
```

## Usage

### main.scss

```scss
@import '../bower_components/polymer-theme/sass/modules/all';

// Roboto Font Combinations
$heading-font-name:     'roboto-slab';
$font-lang:             'en';
$heading-font:          roboto-font($heading-font-name, 'heading');
$body-font:             roboto-font($heading-font-name, 'body');
@import url(roboto-font($heading-font-name, 'url') + '&lang=' + $font-lang);

.polymer-theme {
  // Make copy of ../bower_components/polymer-theme/sass/_variables.scss to styles dir
  @import 'variables';

  @import '../bower_components/polymer-theme/sass/base';

  /deep/ {
    @import '../bower_components/polymer-theme/sass/elements/all';
  }
}
```

### index.html

```html
<body class="polymer-theme">
```

See the [Polymer Base Template](https://github.com/StartPolymer/polymer-base-template)

## [Variables](https://github.com/StartPolymer/polymer-theme/blob/master/sass/_variables.scss)

### [Material Design Colors](http://www.google.com/design/spec/style/color.html#color-color-palette)

- [Link to module](https://github.com/StartPolymer/polymer-theme/blob/master/sass/modules/_material-colors.scss)

```scss
$primary-color-name:    'indigo';
$accent-color-name:     'pink';
```

### [Roboto Font Combinations](https://gist.github.com/8faa215aca23696a3e3c)

- [Link to module](https://github.com/StartPolymer/polymer-theme/blob/master/sass/modules/_roboto-fonts.scss)

```scss
$heading-font-name:     'roboto-slab';
$font-lang:             'en';
```
