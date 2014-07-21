---
title: Developing Less
---

Thanks for thinking about contributing. Please read the [contributing instructions]({{ less.master }}/CONTRIBUTING.md) carefully to avoid wasted work.

## Install these tools

* **node** - <http://nodejs.org/>
* **phantomjs** - <http://phantomjs.org/download.html>

make sure the paths are setup. If you start your favourite command line and type `node -v` you should see the node compiler. If you run `phantomjs -v` you should see the phantomjs version number.

* clone your less.js repository locally
* navigate to your local less.js repository and run `npm install` this installs less' npm dependencies.
* If you haven't used grunt before, run `npm install grunt-cli -g` - this allows you to use the "grunt" command anywhere

## Usage

If you go to the root of the less repository you should be able to do `grunt test` - this should run all the tests. For the browser specific only, run `grunt browsertest` If you want to try out the current version of less against a file, from here do `node bin/lessc path/to/file.less`

To debug the browser tests, run `grunt browsertest-server` then go to http://localhost:8088/tmp/browser/ to see the test runner pages.

Optional: To get the current version of the less compiler do `npm -g install less` - npm is the node package manager and "-g" installs it to be available globally.

You should now be able to do `lessc file.less` and if there is an appropriate file.less then it will be compiled and output to the stdout. You can then compare it to running localy (`node bin/lessc file.less`).

Other grunt commands

* `grunt benchmark` - run our benchmark tests to get some numbers on performance
* `grunt stable` to create a new release
* `grunt readme` to generate a new readme.md in the root directory (after each release)

## Guide

If you look at [http://www.gliffy.com/go/publish/4784259](http://www.gliffy.com/go/publish/4784259),  This is an overview diagram of how less works.

## Books

* [Less Web Development Essentials](http://www.packtpub.com/less-web-development-essentials/book), by Bass Jobsen, Foreword by Alexis Sellier
