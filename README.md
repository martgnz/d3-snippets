# d3-snippets
An [Atom](https://atom.io) package with [D3v4](https://d3js.org) snippets. Accelerate your graphics!

Contributions are appreciated, if you miss a snippet feel free to create an issue or open a pull request.

![d3-snippets in action](https://cloud.githubusercontent.com/assets/1236790/13730058/c2121150-e944-11e5-85fb-2158f62e082d.gif)

## Install
You can install it inside Atom (just search for `d3-snippets`) or via command line:
```
$ apm install d3-snippets
```

## Reference
<a name="app" href="#app">#</a> <code>app</code> [<>](snippets/append.cson "Source")

Append something.

```js
.append('${1:}')
```

<a name="area" href="#area">#</a> <code>area</code> [<>](snippets/area.cson "Source")

Area generator.

```js
var area = d3.area()
    .x(function(d) { return x(d.${1:}); })
    .y1(function(d) { return y(d.${2:}); })
    .y0(y(0));
```

<a name="attr" href="#attr">#</a> <code>attr</code> [<>](snippets/attr.cson "Source")

Set attributes.

```js
.attr('${1:}', '${2:}')
```

<a name="axisb" href="#axisb">#</a> <code>axisb</code> [<>](snippets/axis-bottom.cson "Source")

Bottom-oriented axis.

```js
d3.axisBottom(${1:x});
```

<a name="axisl" href="#axisl">#</a> <code>axisl</code> [<>](snippets/axis-left.cson "Source")

Left-oriented axis.

```js
d3.axisLeft(${1:y});
```

<a name="axisr" href="#axisr">#</a> <code>axisr</code> [<>](snippets/axis-right.cson "Source")

Right-oriented axis.

```js
d3.axisRight(${1:y});
```

<a name="axist" href="#axist">#</a> <code>axist</code> [<>](snippets/axis-top.cson "Source")

Top-oriented axis.

```js
d3.axisTop(${1:x});
```

<a name="axis" href="#axis">#</a> <code>axis</code> [<>](snippets/axis.cson "Source")

Create a SVG axis.

```js
d3.axis()
    .scale(${1:})
    .ticks(${2:})
    .orient('${3:}')
```

<a name="circle" href="#circle">#</a> <code>circle</code> [<>](snippets/circle.cson "Source")

Create a SVG circle.

```js
.enter()
    .append('circle')
    .attr('cx', ${1:})
    .attr('cy', ${2:})
    .attr('r', ${3:})
    .style('fill', '${4:#111}');
```

<a name="class" href="#class">#</a> <code>class</code> [<>](snippets/class.cson "Source")

Set the element class.

```js
.attr('class', '${1:}')
```

<a name="csv" href="#csv">#</a> <code>csv</code> [<>](snippets/csv.cson "Source")

Load a CSV file.

```js
d3.csv('${1:}', function(error, data) {
    ${2:console.log(data);}
});
```

<a name="curve" href="#curve">#</a> <code>curve</code> [<>](snippets/curve.cson "Source")

Curve shorthand.

```js
.curve(d3.${1:curveCatmullRom}.alpha(0.5));
```

<a name="fdi" href="#fdi">#</a> <code>fdi</code> [<>](snippets/data-index.cson "Source")

Return the data and the index.

```js
function(d, i) { return ${1:};}
```

<a name="fd" href="#fd">#</a> <code>fd</code> [<>](snippets/data.cson "Source")

Return the data.

```js
function(d) { return ${1:};}
```

<a name="dom" href="#dom">#</a> <code>dom</code> [<>](snippets/domain.cson "Source")

Set the scale domain.

```js
.domain([${1:}, ${2:}])
```

<a name="dur" href="#dur">#</a> <code>dur</code> [<>](snippets/duration.cson "Source")

Set the transition duration.

```js
.duration(${1:})
```

<a name="ellipse" href="#ellipse">#</a> <code>ellipse</code> [<>](snippets/ellipse.cson "Source")

Create a SVG ellipse.

```js
.enter().append('ellipse')
    .attr('cx', ${1:})
    .attr('cy', ${2:})
    .attr('rx', ${3:})
    .attr('ry', ${4:})
    .style('fill', '${5:#111}');
```

<a name="ent" href="#ent">#</a> <code>ent</code> [<>](snippets/enter.cson "Source")

Enter the data.

```js
.enter()
```

<a name="extent" href="#extent">#</a> <code>extent</code> [<>](snippets/extent.cson "Source")

Set the dataset extent.

```js
d3.extent(${1:data}, function(d) { return d.${2:value}; });
```

<a name="fill-opacity" href="#fill-opacity">#</a> <code>fill-opacity</code> [<>](snippets/fill-opacity.cson "Source")

Set the element fill opacity.

```js
.attr('fill-opacity', ${1:0.5})
```

<a name="fill" href="#fill">#</a> <code>fill</code> [<>](snippets/fill.cson "Source")

Set the element fill.

```js
.attr('fill', '${1:none}')
```

<a name="fn" href="#fn">#</a> <code>fn</code> [<>](snippets/function.cson "Source")

Blank anonymous function.

```js
function() { return ${1:};}
```

<a name="geomap" href="#geomap">#</a> <code>geomap</code> [<>](snippets/geo-map.cson "Source")

Create the projection and path for a map.

```js
var projection = d3.${1:geoMercator}()
    .fitSize([${2:width}, ${3:height}], ${4:land});

var path = d3.geoPath()
    .projection(projection);
${7:}
```

<a name="g" href="#g">#</a> <code>g</code> [<>](snippets/group.cson "Source")

Create a SVG group.

```js
svg
    .append('g')
    .attr('class', '${1:}')
```

<a name="join" href="#join">#</a> <code>join</code> [<>](snippets/join.cson "Source")

Start with a data join.

```js
d3.selectAll('${1:}')
    .data(${2:})
```

<a name="json" href="#json">#</a> <code>json</code> [<>](snippets/json.cson "Source")

Load a JSON file.

```js
d3.json('${1:}', function(error, data) {
    ${2:console.log(data);}
});
```

<a name="lineg" href="#lineg">#</a> <code>lineg</code> [<>](snippets/line-generator.cson "Source")

Line generator.

```js
var line = d3.line()
  .x(function(d) { return x(d.${1:}); })
  .y(function(d) { return y(d.${2:}); });
```

<a name="line" href="#line">#</a> <code>line</code> [<>](snippets/line.cson "Source")

Create a SVG Line.

```js
.enter().append('line')
    .attr('x1', ${1:})
    .attr('y1', ${2:})
    .attr('x2', ${3:})
    .attr('y2', ${4:})
    .style('stroke', '${5:#111}');
```

<a name="locale" href="#locale">#</a> <code>locale</code> [<>](snippets/locale.cson "Source")

Set a default locale.

```js
var ${1:en_US} = {
    'decimal': '.',
    'thousands': ',',
    'grouping': [3],
    'currency': ['$', ''],
    'dateTime': '%a %b %e %X %Y',
    'date': '%m/%d/%Y',
    'time': '%H:%M:%S',
    'periods': ['AM', 'PM'],
    'days': ['Sunday', 'Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday', 'Saturday'],
    'shortDays': ['Sun', 'Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat'],
    'months': ['January', 'February', 'March', 'April', 'May', 'June', 'July', 'August', 'September', 'October', 'November', 'December'],
    'shortMonths': ['Jan', 'Feb', 'Mar', 'Apr', 'May', 'Jun', 'Jul', 'Aug', 'Sep', 'Oct', 'Nov', 'Dec']
}

formatDefaultLocale(${2:en_US});
timeFormatDefaultLocale(${3:en_US});

```

<a name="margin" href="#margin">#</a> <code>margin</code> [<>](snippets/margin.cson "Source")

Append a SVG with the margin convention.

```js
var margin = {top: ${1:20}, right: ${2:10}, bottom: ${3:20}, left: ${4:10}},
    width = ${5:960} - margin.left - margin.right,
    height = ${6:500} - margin.top - margin.bottom;

var svg = d3.select('${7:body}').append('svg')
    .attr('width', width + margin.left + margin.right)
    .attr('height', height + margin.top + margin.bottom)
  .append('g')
    .attr('transform', 'translate(' + margin.left + ',' + margin.top + ')');

${8:}
```

<a name="nest" href="#nest">#</a> <code>nest</code> [<>](snippets/nest.cson "Source")

Nest a dataset.

```js
var nest = d3.nest()
    .key(function(d) { return ${1:}; })
    .entries(${2:});
```

<a name="on" href="#on">#</a> <code>on</code> [<>](snippets/on.cson "Source")

Listen for events on the selection.

```js
.on('${1:}', ${2:})
```

<a name="queue" href="#queue">#</a> <code>queue</code> [<>](snippets/queue.cson "Source")

Create a queue to load multiple files.

```js
d3.queue()
    .defer(${1:d3.json}, '${2:}')
    .defer(${3:d3.json}, '${4:}')
    .await(function(error, ${5:file1}, ${6:file2}) {
        console.log(${7:file1}, ${8:file1});
    });
```

<a name="r" href="#r">#</a> <code>r</code> [<>](snippets/radius.cson "Source")

Set the element radius.

```js
.attr('r', ${1:5})
```

<a name="ran" href="#ran">#</a> <code>ran</code> [<>](snippets/range.cson "Source")

Set the scale range.

```js
.range([${1:}, ${2:}])
```

<a name="rect" href="#rect">#</a> <code>rect</code> [<>](snippets/rect.cson "Source")

Create a SVG rect.

```js
.enter().append('rect')
    .attr('x', ${1:})
    .attr('y', ${2:})
    .attr('width', ${3:width})
    .attr('height', ${4:height})
    .attr('rx', ${5:0})
    .attr('ry', ${6:0})
    .style('fill', '${7:#111}');
```

<a name="seq" href="#seq">#</a> <code>seq</code> [<>](snippets/scale-sequential.cson "Source")

Create a sequential scale.

```js
d3.scaleSequential(d3.${1:interpolateViridis})
    .domain([${2:}])
```

<a name="scale" href="#scale">#</a> <code>scale</code> [<>](snippets/scale.cson "Source")

Create a sample scale.

```js
d3.${1:scaleLinear}()
    .domain([${2:}, ${3:}])
    .range([${4:}, ${5:}]);
```

<a name="sel" href="#sel">#</a> <code>sel</code> [<>](snippets/select.cson "Source")

Select an element.

```js
d3.select('${1:}')
```

<a name="sela" href="#sela">#</a> <code>sela</code> [<>](snippets/selectAll.cson "Source")

Select all the elements.

```js
d3.selectAll('${1:}')
```

<a name="sort" href="#sort">#</a> <code>sort</code> [<>](snippets/sort.cson "Source")

Sort a dataset.

```js
${1:data}.sort(function(a, b) {
    return ${2:a}.${3:value} - ${4:b}.${5:value};
});
```

<a name="stroke-opacity" href="#stroke-opacity">#</a> <code>stroke-opacity</code> [<>](snippets/stroke-opacity.cson "Source")

Set the element stroke opacity.

```js
.attr('stroke-opacity', ${1:0.5})
```

<a name="stroke-width" href="#stroke-width">#</a> <code>stroke-width</code> [<>](snippets/stroke-width.cson "Source")

Set the element stroke width.

```js
.attr('stroke-width', ${1:1})
```

<a name="stroke" href="#stroke">#</a> <code>stroke</code> [<>](snippets/stroke.cson "Source")

Set the element stroke.

```js
.attr('stroke', '${1:black}')
```

<a name="style" href="#style">#</a> <code>style</code> [<>](snippets/style.cson "Source")

Set the element style.

```js
.style('${1:}', '${2:}')
```

<a name="anchor" href="#anchor">#</a> <code>anchor</code> [<>](snippets/text-anchor.cson "Source")

Set the text anchor.

```js
.attr('text-anchor', '${1:middle}')
```

<a name="text" href="#text">#</a> <code>text</code> [<>](snippets/text.cson "Source")

Set the element text.

```js
.text('${1:}')
```

<a name="tickSize" href="#tickSize">#</a> <code>tickSize</code> [<>](snippets/tick-size.cson "Source")

Set the tick size.

```js
.tickSize(${1:})
```

<a name="tickValues" href="#tickValues">#</a> <code>tickValues</code> [<>](snippets/tick-values.cson "Source")

Set the tick values.

```js
.tickValues(['${1:}'])
```

<a name="translate" href="#translate">#</a> <code>translate</code> [<>](snippets/translate.cson "Source")

Translate the element.

```js
.attr('transform', 'translate(' + ${1:0} + ',' + ${2:0} + ')')
```

<a name="voronoi" href="#voronoi">#</a> <code>voronoi</code> [<>](snippets/voronoi.cson "Source")

Create a Voronoi diagram.

```js
var voronoi = d3.voronoi()
    .x(function(d) {return x(d.${1:}); })
    .y(function(d) {return y(d.${2:}); })
    .extent([[0, 0], [${3:width}, ${4:height}]]);

var voronoiGroup = svg.append('g')
    .attr('class', 'voronoi');

voronoiGroup.selectAll('path')
    .data(voronoi.polygons(${5:data}))
    .enter().append('path')
    .attr('d', function(d) { return d ? 'M' + d.join('L') + 'Z' : null; })

```

<a name="x" href="#x">#</a> <code>x</code> [<>](snippets/x.cson "Source")

Set the x position.

```js
.attr('x', ${1:})
```

<a name="y" href="#y">#</a> <code>y</code> [<>](snippets/y.cson "Source")

Set the y position.

```js
.attr('y', ${1:})
```

## Hacking
```
$ cd ~/.atom/packages
$ git clone git@github.com:martgnz/d3-snippets.git
$ cd d3-snippets
$ apm install
$ apm link
```

## Credit
Most of the inspiration comes from [fabriotav](https://github.com/fabriciotav/d3-snippets-for-sublime-text-2)'s  and [shancarter](https://github.com/shancarter/sublime-text-d3/)'s Sublime Text packages.
