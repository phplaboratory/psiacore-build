# psiacore-build

A helper to add tasks to gulp.

## Getting started

Install with:

```sh
npm install psiacore-build
```

and use and require in your gulp file: 

```javascript
var gulp = require('gulp');
var psiacoreTasks = require('psiacore-build');

psiacoreTasks('submodule');
gulp.task('default', ['lint', 'test', 'browser', 'coverage']);
```

### Notes

* There's no default task to allow for each submodule to set up their own configuration
* If the module is node-only, avoid adding the browser tasks with:
```javascript
var psiacoreTasks = require('psiacore-build');
psiacoreTasks('submodule', {skipBrowsers: true});
```

## Contributing

See [CONTRIBUTING.md](https://github.com/phplaboratory/psiacore) on the main psiacore repo for information about how to contribute.

## License

Code released under [the MIT license](https://github.com/phplaboratory/psiacore/blob/master/LICENSE).

Copyright 2015 BitPay, Inc. psiacore is a trademark maintained by BitPay, Inc.

