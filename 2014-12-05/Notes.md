# Front end initiative 2014-12-15
## Notes
### Introduction

  * Boilerplate merges
    * [ ] merged: no drupal branch [pull/32](https://github.com/Crosscheck/drupal-theme-boilerplate/pull/32)
    * [ ] merged: postinstall, sourcemaps, force, theme specify [pull/38](https://github.com/Crosscheck/drupal-theme-boilerplate/pull/38)

  * Boilerplate issues
    * see list agenda

  * bower integration with auto edits on info file
  * yeoman generator

### Firebase - Build Realtime Apps - By Dries
 * Firebase is a realtime backend as a service that allows you to create incredible apps. Save, Store and Update Data in realtime directly from the browser or mobile client using only javascript or native iOS or Android code.
 * You can import your own JSON data file, or export the by GUI made JSON data structure.
 * [github](https://github.com/firebase)
 * [docs](https://www.firebase.com/docs/)

### Headless drupal - By Maarten

  * [drupal](https://groups.drupal.org/headless-drupal) 

### TypeScript & JS refactoring - By Algeron

  * [github](https://github.com/Microsoft/TypeScript)

### Bower - A package manager for the web

  * [github](https://github.com/bower/bower)
  * more for front end [scripts](http://bower.io/search/)
  * install `npm install -g bower`
  * Bower.json (yet another package manager)
  * create bower.json `bower init`
  * dependencies `bower install jquery --save` save zorgt voor een edit op de bower.json voor team collaboratie
  * this installs all the deps in `bower_components` now they can be used in your app
  * but how to inject into your app with [build tools](http://bower.io/docs/tools/)
  * see which files will be used by the build tools `bower list --paths`
  * alfred integration
  
### Yeoman - The web's scaffolding tool for modern webapps
  
  * [github](https://github.com/bower/bower)
  * Yeoman helps you kickstart new projects, prescribing best practices and tools to help you stay productive.
  * it uses [generators](http://yeoman.io/generators/)
  * install the generator you want to use example `npm install -g generator-angular`
  * run generator by `yo generator_name app_name`
  * collaborates with `grunt gulp bower npm sass less`
  * Create a generator for the boilerplate [authoring](http://yeoman.io/authoring/)
    * yo xc-generator:nodrupal
    * yo xc-generator:drupaltheme
    * yo xc-generator:omega
        * no more gemset Setup the gemset to use
        * no more `bundle install` 
        * no more `npm install` 
        * no `bower install` 
        * no more renaming files in the beginning



### Pageres
  * take screenshots from the terminal
  * [github](https://github.com/sindresorhus/pageres)

### gh
  * All the power of GitHub in your terminal.
  * [github](https://github.com/node-gh/gh)

### Perfmap

  * A bookmarklet and Chrome extension to create a front-end performance heatmap of resources loaded in the browser using the Resource Timing API. A browser with support for the Resource Timing API is required.
  * [github](https://github.com/zeman/perfmap)

### Microjs.com

  * Fantastic Micro-Frameworks and Micro-Libraries for Fun and Profit!

