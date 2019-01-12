[![Build Status](http://img.shields.io/travis/stefanjudis/credits-cli.svg?style=flat)](https://travis-ci.org/stefanjudis/credits-cli) [![npm version](http://img.shields.io/npm/v/credits-cli.svg?style=flat)](https://www.npmjs.org/package/credits-cli) [![npm downloads](http://img.shields.io/npm/dm/credits-cli.svg?style=flat)](https://www.npmjs.org/package/credits-cli) [![Coverage Status](http://img.shields.io/coveralls/stefanjudis/credits-cli.svg?style=flat)](https://coveralls.io/r/stefanjudis/credits-cli?branch=master) [![Uses greenkeeper.io](https://img.shields.io/badge/Uses-greenkeeper.io-green.svg)](http://greenkeeper.io/)
[![All Contributors](https://img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)](#contributors)

# credits-cli
> Find out on whose work your project is based on

![Screenshot](./screenshot.png)

We all use a lot of open source projects. Really often we don't even know who is responsible for all the well done projects. You want to see who to thank for hard work?

**Use `credits` and find out on whose work your projects are based on.**

## Install

```
npm install -g credits-cli
```

Also you can use `credits` without global installation, using [`npx`](https://blog.npmjs.org/post/162869356040/introducing-npx-an-npm-package-runner):

```
npx credits-cli
```

## Basic usage

`credits` will check all `node_modules` recursively and evaluate the **Author** and **Maintainers** of the **installed** dependencies included in the set path.

```
Usage
  $ credits <path>

Options
  -r, --reporter Choose reporter to format output [ minimal, extended, markdown ]

Examples
  $ credits /projects/foo
  $ credits /projects/foo --reporter extended
  $ credits /projects/foo --reporter markdown > THANKS.md
```

### Examples

You can use `credits` to generate a `THANKS.md` files easily by running:

```
$ credits . --reporter markdown > THANKS.md
```

***************

#### I want to thank all these [people](./THANKS.md) for their great work!!!

## Contributors

Thanks goes to these wonderful people ([emoji key](https://github.com/kentcdodds/all-contributors#emoji-key)):

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
| [<img src="https://avatars.githubusercontent.com/u/509946?v=3" width="75px;"/><br /><sub>Jayson Harshbarger</sub>](http://www.hypercubed.com)<br />[📖](https://github.com/stefanjudis/credits-cli/commits?author=Hypercubed) [💻](https://github.com/stefanjudis/credits-cli/commits?author=Hypercubed) | [<img src="https://avatars.githubusercontent.com/u/170270?v=3" width="75px;"/><br /><sub>Sindre Sorhus</sub>](https://twitter.com/sindresorhus)<br />[💻](https://github.com/stefanjudis/credits-cli/commits?author=sindresorhus) |
| :---: | :---: |
<!-- ALL-CONTRIBUTORS-LIST:END -->

This project follows the [all-contributors](https://github.com/kentcdodds/all-contributors) specification. Contributions of any kind welcome!
