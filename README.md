# MIDDLEMAN Starter Kit 
Middleman starter kit with custom basic features for futures ruby/html/css/js dev

## Features

 - [Sass](http://sass-lang.com) ready with [Bourbon](http://github.com/thoughtbot/bourbon/) / [Neat](http://github.com/thoughtbot/neat) / [Bitters](http://github.com/thoughtbot/bitters)
 - A basic layout page & index page based on [Normalize](http://github.com/necolas/normalize.css/)
 - Livereload for development mode
 - [Jquery 2 min](https://jquery.com/)   (not for ie 6/7/8)
 - [Google Fonts](https://www.google.com/fonts) with Open-sans
 - [Google analytics](http://www.google.com/analytics/) ready snippet for build in Layout
 - [Heroku](http://www.heroku.com) ready with [puma](http://github.com/puma/puma/)
 - ERB by default (optionnal : [Slim](http://slim-lang.com/) templating *Uncomment the Gemfile)

## System requirements
 - [Heroku Toolbelt](https://toolbelt.heroku.com/) and a heroku account.
 - Ruby (you can set your own version in the Gemfile)(2.1.2 by default)

## Installation
*Setup*
```
mkdir your-folder
git clone git@github.com:magiknono/middleman-heroku-bourbon-ready.git your-folder
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
###Deploy to heroku
*First Commit*
```
git init
git add .
git commit -m "initialise custom middleman starter kit"
```
*Deploy to heroku and test in browser*
```
heroku create
heroku push origin master
heroku open
```

**Enjoy!**

####1 BUG
 - google fonts are only loaded in http, blocked in https 

#### Link for more info on using middleman

 - start here : https://middlemanapp.com/

#### TO DO
 - using jquery cdn
 - normalize.css v3.0.3 instead of v2
 - make basic starting partial/nav/footer/header with neat-basic-center-grid
 - set google analytics in config.rb and layout for easy config
