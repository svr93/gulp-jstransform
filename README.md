## Gulp [jstransform](https://github.com/facebook/jstransform/)

## Usage

```javascript
// npm i --save-dev https://github.com/svr93/gulp-jstransform/tarball/master
var jstransform = require('gulp-jstransform');

gulp.task('jstransform', function() {
  gulp.src('./src/*.js')

    // harmony true: shortcut to enable ES6 & ES7 transforms

    .pipe(jstransform({

      harmony: true,
      target: 'es3'

    }).on('error', gutil.log))
    .pipe(gulp.dest('./public/'))
});
```
