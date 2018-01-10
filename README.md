# Blank Theme For Wordpress Using Gulp


This is just empty theme for starting your Wordpress projects, with
built in support for **Sass**, **Susy** and **Gulp.js**.

## Requirements:

1. [Node.js](https://nodejs.org/)
2. [Gulp.js](http://gulpjs.com/)

## Installation

* The theme folder needs to be the root folder to run gulp
* Replace all the your-theme with the name of your theme
* npm install


When you are done just run `glup watch`

## Features

Most of the features are in gulp. This theme has almost no styling. You only have `clearfix` defined and `_reset.scss` from Eric Mayer as a partial and some empty scss partials.

### Gulp features

* Image optimization
* Sass compilation
* Auto prefixing
* Source maps for css file
* Uglifying and concatinating all js files
* LiveReload

All of these features are run when starting `gulp watch` except for image optimization, you have to run that task separatley.


### CSS and JavaScript

All the of css can be found and should be written in partials. So that you end up with just one css file (style.css).

JavaScript has two folders `lib` and `js` you should never touch `js` folder, this is where the uglifyed and concatinated files go. Put your jQuery plugins and other JS files in lib folder and gulp will do the rest for you. There is no need to call those added scripts from header.php or footer.php, all your scripts will be concatinated in one file.

### Some mixins and functions

You have several mixins and functions in the `_mixins.scss` file along with comments on how to use them. These mixins and functions include:

* Automatic calculation of percentages from pixels
* Automatic calculations of rems from pixels
* Easy to use Media Queries in your normal css flow
