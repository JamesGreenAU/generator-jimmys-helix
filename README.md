# generator-jimmys-helix
> Yeoman generator for Sitecore Projects 

## Installation

First, install [Yeoman](http://yeoman.io) and generator-jimmys-helix.  As this is still a very early work-in-progress, it's not in NPM (we assume you have pre-installed [node.js](https://nodejs.org/)).

```bash
npm install -g yo
```

So use [NPM Link](https://docs.npmjs.com/cli/link) to install this generator by changing into the root of this repo and typing:

```bash
npm link 
```

## What is it?
The purpose of jimmys-helix is to reduce the time when creating Sitecore projects following [Helix] guidelines.

## Background

This generator is based on [generator-prodigious-helix], which is based on [kamsar] yeoman [habitat generator], with a couple of differences:

* Uses Unicorn for serialisation rather than TDS
* Uses a slightly different folder structure under App_Config to suit our installation. 

## Unicorn

The serialization config file created in the new module includes two predicate paths by default:
 * '/sitecore/templates/Feature/YourNewModule' and
 * '/sitecore/layout/Renderings/Feature/YourNewModule'

These are intended to be potentially useful safe defaults.  You should update as per the module's requirements.

[kamsar]: https://twitter.com/kamsar
[habitat generator]: https://github.com/kamsar/generator-habitat/
[Helix]: http://helix.sitecore.net/
[generator-prodigious-helix]: https://github.com/mrodriguezr/generator-prodigious-helix
