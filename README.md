<<<<<<< HEAD
# init-package-json

A node module to get your node module started.

[![Build Status](https://secure.travis-ci.org/npm/init-package-json.svg)](http://travis-ci.org/npm/init-package-json)

## Usage

```javascript
var init = require('init-package-json')
var path = require('path')

// a path to a promzard module.  In the event that this file is
// not found, one will be provided for you.
var initFile = path.resolve(process.env.HOME, '.npm-init')

// the dir where we're doin stuff.
var dir = process.cwd()

// extra stuff that gets put into the PromZard module's context.
// In npm, this is the resolved config object.  Exposed as 'config'
// Optional.
var configData = { some: 'extra stuff' }

// Any existing stuff from the package.json file is also exposed in the
// PromZard module as the `package` object.  There will also be free
// vars for:
// * `filename` path to the package.json file
// * `basename` the tip of the package dir
// * `dirname` the parent of the package dir

init(dir, initFile, configData, function (er, data) {
  // the data's already been written to {dir}/package.json
  // now you can do stuff with it
})
```

Or from the command line:

```
$ npm-init
```

See [PromZard](https://github.com/npm/promzard) for details about
what can go in the config file.
=======
# README #

This README would normally document whatever steps are necessary to get your application up and running.

### What is this repository for? ###

* Quick summary
* Version
* [Learn Markdown](https://bitbucket.org/tutorials/markdowndemo)

### How do I get set up? ###

* Summary of set up
* Configuration
* Dependencies
* Database configuration
* How to run tests
* Deployment instructions

### Contribution guidelines ###

* Writing tests
* Code review
* Other guidelines

### Who do I talk to? ###

* Repo owner or admin
* Other community or team contact
>>>>>>> 7bcc377f2a27b07c66cee0afa9023cc8ff80bd82
