# monkii

This is a fork of [monk](https://github.com/Automattic/monk) with [mongoskin](https://github.com/kissjs/node-mongoskin) upgrade to v2, which use a more recent version of [mongodb](https://github.com/mongodb/node-mongodb-native).

There is a [pending pull request](https://github.com/Automattic/monk/pull/119) waiting to review, this package is for those who can't wait.

## Usage

Simply `npm install monkii` and replace `require('monk')` with `require('monkii')`.

`monkii` is designed to be a drop-in replacement, it has the same API as `monk`.

For documentation, please refer to [monk's README](https://github.com/Automattic/monk/blob/master/README.md).

## Issues

If you encounter any problems, please [file an issue](https://github.com/ratson/monkii/issues) along with a detailed description.

## Run Test Cases
- all tests `node_modules/.bin/mocha`

## Breaking Changes
- `collection.update()` and `collection.remove()` now return the number of documents affected by the operation.
- implements `collection.aggregate(stages, [options], fn)` 
