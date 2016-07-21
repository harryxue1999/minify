# minify
 A plugin that loads (using [text](https://github.com/requirejs/text)) HTML/CSS files and minifies them into a requirejs module.

### Usage
Load HTML/CSS files in your project with `minify!` added in front of the file name. Example:
```
define(['minify!index.html', 'minify!style.css'], function (html, css) {
    // Your code here
});
```
Or alternatively, you can load the module into a browser and use it to load other HTML/CSS files:
```
require(['minify']); // If module has not been loaded in yet
require(['minify!path/to/the/index.html']); // Defines the module
var html = require('minify!path/to/the/index.html'); // {String}
```

> Copyright (c) 2016 Harry Xue
