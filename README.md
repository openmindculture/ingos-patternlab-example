# Ingo's PatternLab Example

- as atomic design PoC for frontend development
- based on the grunt edition, as the pure patternlab-node failed to install
- using Twig as template engine, which is already known and popular from Symfony

## Requirements / Installation Overview

- install node, npm, grunt-cli
- cloned the base setup

```
npm install @pattern-lab/starterkit-twig-demo
grunt patternlab:loadstarterkit --kit=@pattern-lab/starterkit-twig-demo
```

This setup was based on: Pattern Lab Node - Grunt Edition

## Pattern Lab Node - Grunt Edition

The Grunt wrapper around [Pattern Lab Node Core](https://github.com/pattern-lab/patternlab-node), providing tasks to interact with the core library and move supporting frontend assets.

## Packaged Components

The Grunt Edition comes with the following components:

- `patternlab-node`: [GitHub](https://github.com/pattern-lab/patternlab-node), [npm](https://www.npmjs.com/package/patternlab-node)
- `patternengine-node-mustache`: [GitHub](https://github.com/pattern-lab/patternengine-node-mustache), [npm](https://www.npmjs.com/package/patternengine-node-mustache)
- `pattern-lab/styleguidekit-assets-default`: [GitHub](https://github.com/pattern-lab/styleguidekit-assets-default)
- `pattern-lab/styleguidekit-mustache-default`: [GitHub](https://github.com/pattern-lab/styleguidekit-mustache-default)

## Prerequisites

The Pattern Lab Node - Grunt Edition uses [Node](https://nodejs.org) for core processing, [npm](https://www.npmjs.com/) to manage project dependencies, and [grunt.js](http://gruntjs.com/) to run tasks and interface with the core library. Node version 4 or higher suffices. You can follow the directions for [installing Node](https://nodejs.org/en/download/) on the Node website if you haven't done so already. Installation of Node will include npm.

It's also highly recommended that you [install grunt](http://gruntjs.com/getting-started) globally.

## Installing

There are two methods for downloading and installing the Grunt Edition:

- [Download a pre-built package](#download-a-pre-built-package)
- [Use npm](#use-npm)

### Download a pre-built package

The fastest way to get started with the Grunt Edition is to [download the pre-built version](https://github.com/pattern-lab/edition-node-grunt/releases) from the [releases page](https://github.com/pattern-lab/edition-node-grunt/releases). The pre-built project comes with the [Base Starterkit for Mustache](https://github.com/pattern-lab/starterkit-mustache-base) installed by default.

**Please note:** Pattern Lab Node uses [npm](https://www.npmjs.com/) to manage project dependencies. To upgrade the Grunt Edition or to install plug-ins you'll need to be familiar with npm.

### Use npm

`npm` is a dependency management and package system which can pull in all of the Grunt Edition's dependencies for you. To accomplish this:

- download or `git clone` this repository to an install location.

- run the following

  ```
  cd install/location
  npm install
  ```

Running `npm install` from a directory containing a `package.json` file will download all dependencies defined within.

#### Install the Grunt Edition of Pattern Lab Node as a Dependency

Most people want to run Pattern Lab Node standalone and not as a dependency. If you wish to install as a dependency you can do the following:

Use npm's [`install` command](https://docs.npmjs.com/cli/install) with an argument to install the Grunt Edition into a location of your choosing. In Terminal type:

    cd install/location/
    npm install edition-node-grunt

This will install the Grunt Edition into a directory called `node_modules` in `install/location/`.

## Getting started

The Pattern Lab Node - Grunt Edition ships with a [base experience](https://github.com/pattern-lab/starterkit-mustache-base) which serves as clean place to start from scratch with Pattern Lab. But if you want to get rolling with a starterkit of your own, or use the [demo starterkit](https://github.com/pattern-lab/starterkit-mustache-demo) like the one on [demo.patternlab.io](http://demo.patternlab.io), you can do so automatically at time of `npm install` by adding your starterkit to the `package.json` file.

You can also [work with starterkits using the command line](https://github.com/pattern-lab/patternlab-node/wiki/Importing-Starterkits).

## Updating Pattern Lab

To update Pattern Lab please refer to each component's GitHub repository, and the [master instructions for core](https://github.com/pattern-lab/patternlab-node/wiki/Upgrading). The components are listed at the top of the README.

## Helpful Commands

These are some helpful commands you can use on the command line for working with Pattern Lab.

### List all of the available commands

To list all available commands type:

    grunt patternlab:help

### Generate Pattern Lab

To generate the front-end for Pattern Lab type:

    grunt

### Watch for changes and re-generate Pattern Lab

To watch for changes, re-generate the front-end, and server it via a BrowserSync server, type:

    grunt patternlab:serve

BrowserSync should open [http://localhost:3000](http://localhost:3000) in your browser.

### Install a StarterKit

To install a specific StarterKit from GitHub type:

    npm install [starterkit-vendor/starterkit-name]

    grunt patternlab:loadstarterkit --kit=[starterkit-name]
