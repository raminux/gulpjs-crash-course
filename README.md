#gulpjs Crash Course

## What is gulpjs?

It is a toolkit to automate and enhance the workflow. It is a tool written in JavaScript to help developer get rid of slow,repetitive tasks by building an efficient pipelines. It is a replacement for webpack. It is commonly known as task-runner. We give a bunch of tasks to it and it executes them. In the upcomming commits, I will show you how to use gulpjs for various tasks. 

## How to install gulp?
Just run the following command:
```bash
$> npm install gulp-cli -g
```
## How to setup the directory structure?
Let's run the following commands:
```bash
$> mkdir supergulp
$> mkdir src
$> touch src/index.pug
$> mkdir src/img src/js src/scss src/partials src/templates
$> touch js/main.js js/util.js
$> touch scss/styles.scss scss/_variables.scss scss/_reset.scss
$> touch partials/header.pug partials/footer.pug
$> touch templates/layout.pug
```
Also add an image to the `img` directory. Now go to the `supergulp` directory and initialize the node project:
```bash
$> npm init
```
## Adding some content to the files
To fake a real project scenario, it is required to add some data to the project files. So lets's do it!

To use gulp, we need to create a `gulpfile.js`.

Also install the gulp package as:
```bash
$> npm install gulp
```

## How to create a task with gulp?
It is so easy! You have to just export a `const` in the gulpfile.js for each of the task you want. 
We're going to add some task for different tasks such transforming pug files to html ones. 

1. In this task, we want to change `.pug.` files into `.html' ones. First, we need to install a gulp plugin for this purpose:
```bash
$> npm install gulp-pug -D
```
> Sometimes, we need to clean the project to build fresh. To do so, we need to install the following package and use it inside our tasks:
```bash
$> npm i del -D
```
