<!-- @format -->

## NVD3 - A reusable D3 charting library

Inspired by the work of Mike Bostock's [Towards Reusable Charts](http://bost.ocks.org/mike/chart/), and supported by a combined effort of [Novus](http://www.novus.com) and the NVD3 community.

[View Examples](http://nvd3-community.github.io/nvd3/) | [NEW Documentation!](http://nvd3-community.github.io/nvd3/examples/documentation.html) | Development build status: [![Build Status](https://travis-ci.org/novus/nvd3.svg?branch=master)](https://travis-ci.org/novus/nvd3)

## Usage

add `nv.d3` assets to project & include them in the HTML

```
<link href="nv.d3.min.css" rel="stylesheet">
<script src="nv.d3.min.js"></script>
```

- `nv.d3.js` should appear after `d3.js` is included.
- Prefer minified assets (`.min`) for production.

### Dependencies

[ `pieChart`, `padAngle`, `cornerRadius` ]

## Supported Browsers: [ WebKit based ]

[ Google Chrome, Opera 15+, Safari, Firefox, Internet Explorer: 10+ ]

# Optional dependencies

[Fastdom](https://github.com/wilsonpage/fastdom) -> increase performance of the line chart

## A few rules for pull requests

If you want to test your changes using the example pages,
you'll have to run `grunt production` to build the items into the `build` directory.
You must do this before your changes show up in the examples, as they link to the build directory
in order to properly show off the finished product.
Please remember to NOT include the build files in your commit though,
only include the source files you changed!

### Tips for Testing

- Unit tests were written in Karma and Mocha. Follow instructions in **Building Latest** to get npm packages setup. This may not work on Windows machines.
- Run `bower install` to get bower dependencies.
- Run `grunt` to start the unit tests.
- Also visually inspect the HTML pages in the **examples/ and test/ folders**. Make sure there are no glaring errors.``
- Novus now uses Travis CI for continuous integration. Visit [our travis build page](https://travis-ci.org/novus/nvd3/) to see the latest status.

#### Meteor Tinytests

- Any Meteor-specific features can be tested from the command line using `tinytest` and [Spacejam](https://www.npmjs.com/package/spacejam)
- `spacejam` can be installed by running `npm install -g spacejam`.
- Tinytests can then be executed by running `spacejam test-packages ./` from this project's root.

---

## Building latest

1. First clone the repository and checkout the `master` branch
2. make sure `nodejs` is installed via your system's package manager.
3. Install `grunt`, `grunt-cli`, and `bower`: `npm install -g grunt grunt-cli bower`

> have node download nvd3's required modules with: `npm install`

> build with: `grunt production`

You should now have a `build` directory with the js and css files within.

---
