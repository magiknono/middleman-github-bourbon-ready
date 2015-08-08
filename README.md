# MIDDLEMAN Starter Kit
Middleman starter kit with custom basic features for ruby/html/css/js webdesign

see a basic-grid [demo](http://gentle-eyrie-4382.herokuapp.com/)

## Features

 - [Sass](http://sass-lang.com) ready with [Bourbon](http://github.com/thoughtbot/bourbon/) / [Neat](http://github.com/thoughtbot/neat) / [Bitters](http://github.com/thoughtbot/bitters)
 - A basic layout page & index page based on [Normalize](http://github.com/necolas/normalize.css/)
 - Livereload for development mode and Minify css/js for prod
 - [Jquery 2](https://jquery.com/)   (not for ie 6/7/8) or Jquery 1
 - [Google Fonts](https://www.google.com/fonts) with Open-sans
 - [Github pages](https://github.com/middleman-contrib/middleman-deploy) ready with middleman-deploy
 - ERB by default
 - [FontAwesome](http://fontawesome.io/) 4.3.0
 - [Google Analytics](http://github.com/danielbayerlein/middleman-google-analytics/)

## System requirements
 - Git and Github account
 - Ruby (you can set your own version in the Gemfile)(2.1.2 by default)

## Installation
Create a github repository with your username like username.github.io
*Setup*
```
mkdir your-folder
git clone git@github.com:magiknono/middleman-github-bourbon-ready.git your-folder
cd your-folder
git remote rm origin
git remote add origin your-git-url
```
*Install gems*
```
bundle install
```
current version is : Middleman 3.3.12 and all gems are fixed in Gemfile

##Start middleman
```
middleman server
```
**test in your browser : http://localhost:4567**
##Deploy to github pages
*First Commit*
```
git init
git add .
git commit -m "initialise custom middleman starter kit"
```
*Deploy to githubpages and test in browser*
```
middleman deploy
```

## How to start
see the demo at **http://localhost:4567**
```
set your own ruby version in Gemfile
override the grid to make your own in source/stylesheet/base/_grid_settings.scss
write your html index in source/index.html.erb and create new pages
write your own css in source/stylesheets/_custom.scss
customize your own scss variables in source/stylesheets/base/_variables.scss
write your own js in source/javascripts/_lib.js
replace the jquery you want in source/javascripts/all.js
your content can be in data/your-file.yml
Add your google analytics is in config.rb
```
#### **Enjoy!**

#### BUG
 - google fonts are only loaded in http, blocked in https
 - you need some more tweakings for ie, it's not made for ie6/7/8
#### Link for more info

 - start here : https://middlemanapp.com/
 - read the doc of neat and bourbon

#### TO DO

 - make one demo site with erb and maybe after migrating to slim
 - create a command line for configuration option
 - gem sitemap or manual set ?
 - add generate number for img  ?
 - activate pretty url

## License

Copyright (c) 2015 Arnaud Cormier. MIT Licensed, see [LICENSE](http://github.com/magiknono/middleman-heroku-bourbon-ready/blob/master/LICENSE.md) for details.
