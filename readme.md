# AngularJS for Rails generator

Maintainer: [Sheniff](https://github.com/sheniff)

Based on [generator-angular](https://github.com/yeoman/generator-angular)

## Important note

This project is completely based on [generator-angular](https://github.com/yeoman/generator-angular), just **in process to be** adapted to generate proper distributions to be used along with rails.

## Changes (regarding the original project)
* Modify javascript templates
* Add an extra service type: `resource`
* [WIP] Modify Coffeescript templates
* [WIP] Add more options in app creation
* Add a Rails builder task for Grunt so it generates a `distRails` folder ready to be included into the assets-pipeline
* [WIP] Add a HAML version of views

## Install

Install yo, grunt and bower
```
npm install -g yo grunt-cli bower
```
Clone this project locally and call npm link (and reset the console) to be able to do `yo angular-rails` easily
```
git clone git@github.com:sheniff/generator-angular-rails.git && cd generator-angular-rails
npm link
reset
```
Start your project using angular-rails
```
mkdir my-project && cd $_
yo angular-rails --minsafe
npm install
bower install
grunt
```
Build your rails-ready project running
```
grunt build-rails
```

## Usage

For more info about usage, please refer to [original project here](https://github.com/yeoman/generator-angular)
