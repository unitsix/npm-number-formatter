

[![Coverage Status](https://coveralls.io/repos/github/unitsix/npm-number-formatter/badge.svg?branch=master)](https://coveralls.io/github/unitsix/npm-number-formatter?branch=master) [![Build Status](https://travis-ci.org/unitsix/npm-number-formatter.svg?branch=master)](https://travis-ci.org/unitsix/npm-number-formatter)

Number Formatter
=========

A small library that adds commas to numbers

## Installation

  `npm install @unitsix/number-formatter`

## Usage

    var numFormatter = require('@unitsix/number-formatter');
    
    var formattedNum = numFormatter(35666);

  


  Output should be `35,666`

## Tests

  `npm test`
  or
  `make test`

## Deploy/Publish

### With Make

  `make publish-patch` 
  or
  `make publish-minor`
  or
  `make publish-major`

### Without Make

```
npm version patch -m "Version %s - add sweet badges"
```

**%s** = the new version number.

This command will bump the version number in **package.json**, add a new commit, and tag it with this release number.

**Note**: Your Git working directory has to be **clean** before you can run **npm version**.

After bumping the version number

```
git push && git push --tags (or git push origin master --tags)
npm publish
```

 https://codeburst.io/how-to-create-and-publish-your-first-node-js-module-444e7585b738