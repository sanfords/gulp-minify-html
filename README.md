[![Build Status](https://travis-ci.org/jonathanepollack/gulp-minify-html.png?branch=master)](https://travis-ci.org/jonathanepollack/gulp-minify-html)
## Information

<table>
<tr> 
<td>Package</td><td>gulp-minify-html</td>
</tr>
<tr>
<td>Description</td>
<td>Minify css with <a href="https://github.com/Moveo/minimize">minimize.</a></td>
</tr>
<tr>
<td>Node Version</td>
<td>>= 0.6</td>
</tr>
</table>

## Usage

```
var minifyHTML = require('gulp-minify-html');

gulp.task('minify-html', function() {

  gulp.files('./static/html/*.html')
    .pipe(minifyHTML(opts))
    .pipe(gulp.folder('./dist/'))
});
```
### Options
* `empty` - `true, false`: do not removing empty attributes.
* `cdata` - `true, false`: do not stripping CDATA from scripts.
* `comments` - `true, false`: do not removing comments.
* `spare` - `true, false`: do not removing redundant attributes.
* `quotes` - `true, false`: do not removing arbitrary quotes.


## LICENSE

(MIT License)

Copyright (c) 2013 Jonathan Pollack <jonathanepollack@gmail.com>

Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the
"Software"), to deal in the Software without restriction, including
without limitation the rights to use, copy, modify, merge, publish,
distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so, subject to
the following conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
