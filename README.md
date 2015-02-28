# node-match-media

[![NPM version](https://img.shields.io/npm/v/grunt-match-media.svg)](https://www.npmjs.com/package/grunt-match-media) [![NPM Downloads](https://img.shields.io/npm/dm/grunt-match-media.svg)](https://www.npmjs.com/package/grunt-match-media) [![Dependencies](https://img.shields.io/david/mstrutt/grunt-match-media.svg)](https://david-dm.org/mstrutt/grunt-match-media#info=dependencies) [![Dev Dependencies](https://img.shields.io/david/dev/mstrutt/grunt-match-media.svg)](https://david-dm.org/mstrutt/grunt-match-media#info=devDependencies) [![Build Status](https://img.shields.io/travis/mstrutt/grunt-match-media/master.svg)](https://travis-ci.org/mstrutt/grunt-match-media)

> Node function to extract styles matching certain media conditions, and separate the styles out

## Usage

- [grunt-match-media](https://npmjs.org/package/grunt-match-media) - a [Grunt](http://gruntjs.com/) wrapper for this task, allowing you to use it as part of the build process.

### Future uses

- *gulp-match-media* - I plan on making a wrapper for the popular build-tool [Gulp](http://gulpjs.com/)
- *command line interface* - extending this package so it can be run directly from the command line, or as a task to run from npm

## Caveats / Todos

At the moment, functionality is limited to [`min-width`, `max-width`, `min-device-width`, `max-device-width`, `min-height`, `max-height`, `min-device-height`, `max-device-height`, `orientation`] media queries, chaining is supported with `,` and `and` to build complex statements. I have also recently added support for a binary check between `print` and all other media types. In the future I am looking to include:

* Possibility to include more queries such as `min-device-pixel-ratio` hopefully working through this list: https://developer.mozilla.org/en-US/docs/Web/Guide/CSS/Media_queries#Pseudo-BNF_(for_those_of_you_that_like_that_kind_of_thing)
* An exclude option to ignore a certain type of media query