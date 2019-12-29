## [2.0.0] - Major - 2019-12-29
* Switch to d3v5, this only means changing the way `d3.json` and `d3.csv` work.
* Rewritten the snippets using ES2015.
* New snippet for using `Promise.all` to load files. This is the way to do it now as d3-queue is no longer recommended.
* New snippet for `d3.max`.
* New snippet for `d3.min`.

## [1.2.1] - Path - 2017-11-01
* Change block snippet shorthand to `createblock` to prevent a collision with the CSS display property.

## [1.2.0] - Minor - 2017-10-29
* New snippet to scaffold blocks.

## [1.1.0] - Minor - 2017-10-24
### Added
* Support for TypeScript and React scopes (`.ts`, `.tsx`, and `.jsx`).
* New snippet to set the _x_.
* New snippet to set the _y_.
* New snippet to set the radius.
* New snippet to add a class.
* New snippet to add a group.
* New snippet for `d3.extent`.
* New snippet for `d3.scaleSequential`.
* New snippet for sorting a dataset.
* New snippets for customizing the stroke.
* New snippets for customizing the fill.
* New snippets for customizing the axis ticks.
* New snippet to set the text.
* New snippet to set the text anchor.

### Fixes
* Improve [d3-voronoi](https://github.com/d3/d3-voronoi) snippet.

## [1.0.1] - Patch - 2017-05-14
### Fixes
* Fix semicolon on margin snippet.

## [1.0.0] - Major - 2017-04-15
* Update to D3.v4.

### Added
* New snippets for [d3-axis](https://github.com/d3/d3-axis).
* New snippets for [d3-shape](https://github.com/d3/d3-shape).
* New snippet for [d3-voronoi](https://github.com/d3/d3-voronoi).

### Update
* Rename map snippet to geomap.

### Fixes
* Improve descriptions

## [0.2.0] - Minor - 2016-10-11
### Added
* New snippets contributed by @dephora for `domain`, `range`, `append`, `duration`, `enter` and `on`. Add `d3.svg.axis` snippet.

### Fixes
* Small bug on `attr` snippet, by @dephora.

## [0.1.1] - Patch
* Small bugfix on the queue snippet
* Improve anonymous function descriptions

## [0.1.0] - First Release
* Add the first snippets
