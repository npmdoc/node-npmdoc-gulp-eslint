# api documentation for  [gulp-eslint (v3.0.1)](https://github.com/adametry/gulp-eslint#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-gulp-eslint.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-gulp-eslint) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-gulp-eslint.svg)](https://travis-ci.org/npmdoc/node-npmdoc-gulp-eslint)
#### A gulp plugin for processing files with ESLint

[![NPM](https://nodei.co/npm/gulp-eslint.png?downloads=true)](https://www.npmjs.com/package/gulp-eslint)

[![apidoc](https://npmdoc.github.io/node-npmdoc-gulp-eslint/build/screenCapture.buildNpmdoc.browser.%2Fhome%2Ftravis%2Fbuild%2Fnpmdoc%2Fnode-npmdoc-gulp-eslint%2Ftmp%2Fbuild%2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-gulp-eslint/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-gulp-eslint/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-gulp-eslint/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Adametry"
    },
    "bugs": {
        "url": "https://github.com/adametry/gulp-eslint/issues"
    },
    "contributors": [
        {
            "name": "Shinnosuke Watanabe",
            "email": "snnskwtnb@gmail.com",
            "url": "https://github.com/shinnn"
        }
    ],
    "dependencies": {
        "bufferstreams": "^1.1.1",
        "eslint": "^3.0.0",
        "gulp-util": "^3.0.6"
    },
    "description": "A gulp plugin for processing files with ESLint",
    "devDependencies": {
        "@shinnn/eslint-config-node": "^2.0.0",
        "babel-eslint": "^6.1.0",
        "from2-string": "^1.1.0",
        "gulp": "^3.9.0",
        "istanbul": "^0.4.4",
        "mocha": "^2.2.5",
        "should": "^9.0.2",
        "vinyl": "^1.0.0"
    },
    "directories": {
        "example": "example",
        "test": "test"
    },
    "dist": {
        "shasum": "04e57e3e18c6974267c12cf6855dc717d4a313bd",
        "tarball": "https://registry.npmjs.org/gulp-eslint/-/gulp-eslint-3.0.1.tgz"
    },
    "files": [
        "index.js",
        "util.js"
    ],
    "gitHead": "6059c2245c677a48add3ca4bbe5912f601732826",
    "homepage": "https://github.com/adametry/gulp-eslint#readme",
    "keywords": [
        "gulpplugin",
        "eslint",
        "gulp",
        "errors",
        "warnings",
        "check",
        "source",
        "code",
        "formatter",
        "js",
        "javascript",
        "task",
        "lint",
        "plugin"
    ],
    "license": "MIT",
    "maintainers": [
        {
            "name": "shinnn",
            "email": "snnskwtnb@gmail.com"
        },
        {
            "name": "adametry",
            "email": "dark.account@gmail.com"
        }
    ],
    "name": "gulp-eslint",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/adametry/gulp-eslint.git"
    },
    "scripts": {
        "coverage": "istanbul cover _mocha",
        "gulp": "gulp",
        "gulp-example": "gulp --gulpfile=example/config.js",
        "pretest": "gulp test",
        "test": "mocha"
    },
    "version": "3.0.1"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module gulp-eslint](#apidoc.module.gulp-eslint)
1.  [function <span class="apidocSignatureSpan">gulp-eslint.</span>failAfterError ()](#apidoc.element.gulp-eslint.failAfterError)
1.  [function <span class="apidocSignatureSpan">gulp-eslint.</span>failOnError ()](#apidoc.element.gulp-eslint.failOnError)
1.  [function <span class="apidocSignatureSpan">gulp-eslint.</span>format (formatter, writable)](#apidoc.element.gulp-eslint.format)
1.  [function <span class="apidocSignatureSpan">gulp-eslint.</span>formatEach (formatter, writable)](#apidoc.element.gulp-eslint.formatEach)
1.  [function <span class="apidocSignatureSpan">gulp-eslint.</span>result (typeof action !== 'function')](#apidoc.element.gulp-eslint.result)
1.  [function <span class="apidocSignatureSpan">gulp-eslint.</span>results (action)](#apidoc.element.gulp-eslint.results)
1.  object <span class="apidocSignatureSpan">gulp-eslint.</span>util

#### [module gulp-eslint.util](#apidoc.module.gulp-eslint.util)
1.  [function <span class="apidocSignatureSpan">gulp-eslint.util.</span>createIgnoreResult ('node_modules/')](#apidoc.element.gulp-eslint.util.createIgnoreResult)
1.  [function <span class="apidocSignatureSpan">gulp-eslint.util.</span>filterResult (result, filter)](#apidoc.element.gulp-eslint.util.filterResult)
1.  [function <span class="apidocSignatureSpan">gulp-eslint.util.</span>firstResultMessage (result, condition)](#apidoc.element.gulp-eslint.util.firstResultMessage)
1.  [function <span class="apidocSignatureSpan">gulp-eslint.util.</span>handleCallback (callback, value)](#apidoc.element.gulp-eslint.util.handleCallback)
1.  [function <span class="apidocSignatureSpan">gulp-eslint.util.</span>isErrorMessage (message)](#apidoc.element.gulp-eslint.util.isErrorMessage)
1.  [function <span class="apidocSignatureSpan">gulp-eslint.util.</span>migrateOptions (options)](#apidoc.element.gulp-eslint.util.migrateOptions)
1.  [function <span class="apidocSignatureSpan">gulp-eslint.util.</span>resolveFormatter (formatter)](#apidoc.element.gulp-eslint.util.resolveFormatter)
1.  [function <span class="apidocSignatureSpan">gulp-eslint.util.</span>resolveWritable (writable)](#apidoc.element.gulp-eslint.util.resolveWritable)
1.  [function <span class="apidocSignatureSpan">gulp-eslint.util.</span>transform (transform, flush)](#apidoc.element.gulp-eslint.util.transform)
1.  [function <span class="apidocSignatureSpan">gulp-eslint.util.</span>tryResultAction (action, result, done)](#apidoc.element.gulp-eslint.util.tryResultAction)
1.  [function <span class="apidocSignatureSpan">gulp-eslint.util.</span>writeResults (results, formatter, writable)](#apidoc.element.gulp-eslint.util.writeResults)



# <a name="apidoc.module.gulp-eslint"></a>[module gulp-eslint](#apidoc.module.gulp-eslint)

#### <a name="apidoc.element.gulp-eslint.failAfterError"></a>[function <span class="apidocSignatureSpan">gulp-eslint.</span>failAfterError ()](#apidoc.element.gulp-eslint.failAfterError)
- description and source-code
```javascript
() => {
	return gulpEslint.results(results => {
		const count = results.errorCount;
		if (!count) {
			return;
		}

		throw new PluginError('gulp-eslint', {
			name: 'ESLintError',
			message: 'Failed with ' + count + (count === 1 ? ' error' : ' errors')
		});
	});
}
```
- example usage
```shell
...
        // of the file object so it can be used by other modules.
        .pipe(eslint())
        // eslint.format() outputs the lint results to the console.
        // Alternatively use eslint.formatEach() (see Docs).
        .pipe(eslint.format())
        // To have the process exit with an error code (1) on
        // lint error, return the stream and pipe to failAfterError last.
        .pipe(eslint.failAfterError());
});

gulp.task('default', ['lint'], function () {
    // This will only run if the lint task is successful...
});
'''
...
```

#### <a name="apidoc.element.gulp-eslint.failOnError"></a>[function <span class="apidocSignatureSpan">gulp-eslint.</span>failOnError ()](#apidoc.element.gulp-eslint.failOnError)
- description and source-code
```javascript
() => {
	return gulpEslint.result(result => {
		const error = util.firstResultMessage(result, util.isErrorMessage);
		if (!error) {
			return;
		}

		throw new PluginError('gulp-eslint', {
			name: 'ESLintError',
			fileName: result.filePath,
			message: error.message,
			lineNumber: error.line
		});
	});
}
```
- example usage
```shell
...
	}));
'''

Type: 'function (results, callback) { callback(error); }'

Call an asynchronous function once for all ESLint file results before a stream finishes. The callback must be called for the stream
 to finish. If a value is passed to the callback, it will be wrapped in a Gulp PluginError and emitted from the stream.

### eslint.failOnError()

Stop a task/stream if an ESLint error has been reported for any file.

'''javascript
// Cause the stream to stop(/fail) before copying an invalid JS file to the output directory
gulp.src(['**/*.js','!node_modules/**'])
	.pipe(eslint())
...
```

#### <a name="apidoc.element.gulp-eslint.format"></a>[function <span class="apidocSignatureSpan">gulp-eslint.</span>format (formatter, writable)](#apidoc.element.gulp-eslint.format)
- description and source-code
```javascript
(formatter, writable) => {
	formatter = util.resolveFormatter(formatter);
	writable = util.resolveWritable(writable);

	return gulpEslint.results(results => {
		// Only format results if files has been lint'd
		if (results.length) {
			util.writeResults(results, formatter, writable);
		}
	});
}
```
- example usage
```shell
...
    // So, it's best to have gulp ignore the directory as well.
    // Also, Be sure to return the stream from the task;
    // Otherwise, the task may end before the stream has finished.
    return gulp.src(['**/*.js','!node_modules/**'])
        // eslint() attaches the lint output to the "eslint" property
        // of the file object so it can be used by other modules.
        .pipe(eslint())
        // eslint.format() outputs the lint results to the console.
        // Alternatively use eslint.formatEach() (see Docs).
        .pipe(eslint.format())
        // To have the process exit with an error code (1) on
        // lint error, return the stream and pipe to failAfterError last.
        .pipe(eslint.failAfterError());
});
...
```

#### <a name="apidoc.element.gulp-eslint.formatEach"></a>[function <span class="apidocSignatureSpan">gulp-eslint.</span>formatEach (formatter, writable)](#apidoc.element.gulp-eslint.formatEach)
- description and source-code
```javascript
(formatter, writable) => {
	formatter = util.resolveFormatter(formatter);
	writable = util.resolveWritable(writable);

	return gulpEslint.result(result => util.writeResults([result], formatter, writable));
}
```
- example usage
```shell
...
    // Also, Be sure to return the stream from the task;
    // Otherwise, the task may end before the stream has finished.
    return gulp.src(['**/*.js','!node_modules/**'])
        // eslint() attaches the lint output to the "eslint" property
        // of the file object so it can be used by other modules.
        .pipe(eslint())
        // eslint.format() outputs the lint results to the console.
        // Alternatively use eslint.formatEach() (see Docs).
        .pipe(eslint.format())
        // To have the process exit with an error code (1) on
        // lint error, return the stream and pipe to failAfterError last.
        .pipe(eslint.failAfterError());
});

gulp.task('default', ['lint'], function () {
...
```

#### <a name="apidoc.element.gulp-eslint.result"></a>[function <span class="apidocSignatureSpan">gulp-eslint.</span>result (typeof action !== 'function')](#apidoc.element.gulp-eslint.result)
- description and source-code
```javascript
action => {
	if (typeof action !== 'function') {
		throw new Error('Expected callable argument');
	}

	return util.transform((file, enc, done) => {
		if (file.eslint) {
			util.tryResultAction(action, file.eslint, util.handleCallback(done, file));
		} else {
			done(null, file);
		}
	});
}
```
- example usage
```shell
...

### eslint(configFilePath)

Type: 'String'

Shorthand for defining 'options.configFile'.

### eslint.result(action)

Type: 'function (result) {}'

Call a function for each ESLint file result. No returned value is expected. If an error is thrown, it will be wrapped in a Gulp
PluginError and emitted from the stream.

'''javascript
gulp.src(['**/*.js','!node_modules/**'])
...
```

#### <a name="apidoc.element.gulp-eslint.results"></a>[function <span class="apidocSignatureSpan">gulp-eslint.</span>results (action)](#apidoc.element.gulp-eslint.results)
- description and source-code
```javascript
results = function (action) {
	if (typeof action !== 'function') {
		throw new Error('Expected callable argument');
	}

	const results = [];
	results.errorCount = 0;
	results.warningCount = 0;

	return util.transform((file, enc, done) => {
		if (file.eslint) {
			results.push(file.eslint);
			// collect total error/warning count
			results.errorCount += file.eslint.errorCount;
			results.warningCount += file.eslint.warningCount;
		}
		done(null, file);

	}, done => {
		util.tryResultAction(action, results, util.handleCallback(done));
	});
}
```
- example usage
```shell
...
'''

Type: 'function (result, callback) { callback(error); }'

Call an asynchronous function for each ESLint file result. The callback must be called for the stream to finish. If a value is passed
 to the callback, it will be wrapped in a Gulp PluginError and emitted from the stream.


### eslint.results(action)

Type: 'function (results) {}'

Call a function once for all ESLint file results before a stream finishes. No returned value is expected. If an error is thrown,
it will be wrapped in a Gulp PluginError and emitted from the stream.

The results list has a "warningCount" property that is the sum of warnings in all results; likewise, an "errorCount" property is
 set to the sum of errors in all results.
...
```



# <a name="apidoc.module.gulp-eslint.util"></a>[module gulp-eslint.util](#apidoc.module.gulp-eslint.util)

#### <a name="apidoc.element.gulp-eslint.util.createIgnoreResult"></a>[function <span class="apidocSignatureSpan">gulp-eslint.util.</span>createIgnoreResult ('node_modules/')](#apidoc.element.gulp-eslint.util.createIgnoreResult)
- description and source-code
```javascript
file => {
	return {
		filePath: file.path,
		messages: [{
			fatal: false,
			severity: 1,
			message: file.path.indexOf('node_modules/') < 0 ?
				'File ignored because of .eslintignore file' :
				'File ignored because it has a node_modules/** path'
		}],
		errorCount: 0,
		warningCount: 1
	};
}
```
- example usage
```shell
...
			// (https://github.com/gulpjs/gulp/blob/master/docs/recipes/specifying-a-cwd.md)
			// Also, ESLint doesn't adjust file paths relative to an ancestory .eslintignore path.
			// E.g., If ../.eslintignore has "foo/*.js", ESLint will ignore ./foo/*.js, instead of ../foo/*.js.
			// Eslint rolls this into 'CLIEngine.executeOnText'. So, gulp-eslint must account for this limitation.

			if (linter.options.ignore && options.warnFileIgnored) {
				// Warn that gulp.src is needlessly reading files that ESLint ignores
				file.eslint = util.createIgnoreResult(file);
			}
			cb(null, file);
			return;
		}

		if (file.isStream()) {
			file.contents = file.contents.pipe(new BufferStreams((err, buf, done) => {
...
```

#### <a name="apidoc.element.gulp-eslint.util.filterResult"></a>[function <span class="apidocSignatureSpan">gulp-eslint.util.</span>filterResult (result, filter)](#apidoc.element.gulp-eslint.util.filterResult)
- description and source-code
```javascript
(result, filter) => {
	if (typeof filter !== 'function') {
		filter = isErrorMessage;
	}
	const messages = result.messages.filter(filter, result);
	return {
		filePath: result.filePath,
		messages: messages,
		errorCount: messages.reduce(countErrorMessage, 0),
		warningCount: messages.reduce(countWarningMessage, 0)
	};
}
```
- example usage
```shell
...
	function verify(str, filePath) {
		const result = linter.executeOnText(str, filePath).results[0];
		// Note: Fixes are applied as part of "executeOnText".
		// Any applied fix messages have been removed from the result.

		if (options.quiet) {
			// ignore warnings
			return util.filterResult(result, options.quiet);
		}

		return result;
	}

	return util.transform((file, enc, cb) => {
		const filePath = path.relative(process.cwd(), file.path);
...
```

#### <a name="apidoc.element.gulp-eslint.util.firstResultMessage"></a>[function <span class="apidocSignatureSpan">gulp-eslint.util.</span>firstResultMessage (result, condition)](#apidoc.element.gulp-eslint.util.firstResultMessage)
- description and source-code
```javascript
(result, condition) => {
	if (!result.messages) {
		return null;
	}

	return result.messages.find(condition);
}
```
- example usage
```shell
...
/**
 * Fail when an ESLint error is found in ESLint results.
 *
 * @returns {stream} gulp file stream
 */
gulpEslint.failOnError = () => {
	return gulpEslint.result(result => {
		const error = util.firstResultMessage(result, util.isErrorMessage);
		if (!error) {
			return;
		}

		throw new PluginError('gulp-eslint', {
			name: 'ESLintError',
			fileName: result.filePath,
...
```

#### <a name="apidoc.element.gulp-eslint.util.handleCallback"></a>[function <span class="apidocSignatureSpan">gulp-eslint.util.</span>handleCallback (callback, value)](#apidoc.element.gulp-eslint.util.handleCallback)
- description and source-code
```javascript
(callback, value) => {
	return err => {
		if (err != null && !(err instanceof gutil.PluginError)) {
			err = new gutil.PluginError(err.plugin || 'gulp-eslint', err, {
				showStack: (err.showStack !== false)
			});
		}

		callback(err, value);
	};
}
```
- example usage
```shell
...
gulpEslint.result = action => {
	if (typeof action !== 'function') {
		throw new Error('Expected callable argument');
	}

	return util.transform((file, enc, done) => {
		if (file.eslint) {
			util.tryResultAction(action, file.eslint, util.handleCallback(done, file));
		} else {
			done(null, file);
		}
	});
};

/**
...
```

#### <a name="apidoc.element.gulp-eslint.util.isErrorMessage"></a>[function <span class="apidocSignatureSpan">gulp-eslint.util.</span>isErrorMessage (message)](#apidoc.element.gulp-eslint.util.isErrorMessage)
- description and source-code
```javascript
function isErrorMessage(message) {
	const level = message.fatal ? 2 : message.severity;

	if (Array.isArray(level)) {
		return level[0] > 1;
	}

	return level > 1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-eslint.util.migrateOptions"></a>[function <span class="apidocSignatureSpan">gulp-eslint.util.</span>migrateOptions (options)](#apidoc.element.gulp-eslint.util.migrateOptions)
- description and source-code
```javascript
function migrateOptions(options) {
	if (typeof options === 'string') {
		// basic config path overload: gulpEslint('path/to/config.json')
		options = {
			configFile: options
		};
	}

	return options;
}
```
- example usage
```shell
...
/**
 * Append ESLint result to each file
 *
 * @param {(Object|String)} [options] - Configure rules, env, global, and other options for running ESLint
 * @returns {stream} gulp file stream
 */
function gulpEslint(options) {
	options = util.migrateOptions(options) || {};
	const linter = new CLIEngine(options);

	function verify(str, filePath) {
		const result = linter.executeOnText(str, filePath).results[0];
		// Note: Fixes are applied as part of "executeOnText".
		// Any applied fix messages have been removed from the result.
...
```

#### <a name="apidoc.element.gulp-eslint.util.resolveFormatter"></a>[function <span class="apidocSignatureSpan">gulp-eslint.util.</span>resolveFormatter (formatter)](#apidoc.element.gulp-eslint.util.resolveFormatter)
- description and source-code
```javascript
(formatter) => {
	// use ESLint to look up formatter references
	if (typeof formatter !== 'function') {
		// load formatter (module, relative to cwd, ESLint formatter)
		formatter =	CLIEngine.getFormatter(formatter) || formatter;
	}

	return formatter;
}
```
- example usage
```shell
...
* Format the results of each file individually.
*
* @param {(String|Function)} [formatter=stylish] - The name or function for a ESLint result formatter
* @param {(Function|Stream)} [writable=gulp-util.log] - A funtion or stream to write the formatted ESLint results.
* @returns {stream} gulp file stream
*/
gulpEslint.formatEach = (formatter, writable) => {
	formatter = util.resolveFormatter(formatter);
	writable = util.resolveWritable(writable);

	return gulpEslint.result(result => util.writeResults([result], formatter, writable));
};

/**
* Wait until all files have been linted and format all results at once.
...
```

#### <a name="apidoc.element.gulp-eslint.util.resolveWritable"></a>[function <span class="apidocSignatureSpan">gulp-eslint.util.</span>resolveWritable (writable)](#apidoc.element.gulp-eslint.util.resolveWritable)
- description and source-code
```javascript
(writable) => {
	if (!writable) {
		writable = gutil.log;
	} else if (typeof writable.write === 'function') {
		writable = writable.write.bind(writable);
	}
	return writable;
}
```
- example usage
```shell
...
*
* @param {(String|Function)} [formatter=stylish] - The name or function for a ESLint result formatter
* @param {(Function|Stream)} [writable=gulp-util.log] - A funtion or stream to write the formatted ESLint results.
* @returns {stream} gulp file stream
*/
gulpEslint.formatEach = (formatter, writable) => {
	formatter = util.resolveFormatter(formatter);
	writable = util.resolveWritable(writable);

	return gulpEslint.result(result => util.writeResults([result], formatter, writable));
};

/**
* Wait until all files have been linted and format all results at once.
*
...
```

#### <a name="apidoc.element.gulp-eslint.util.transform"></a>[function <span class="apidocSignatureSpan">gulp-eslint.util.</span>transform (transform, flush)](#apidoc.element.gulp-eslint.util.transform)
- description and source-code
```javascript
transform = function (transform, flush) {
	if (typeof flush === 'function') {
		return new Transform({
			objectMode: true,
			transform,
			flush
		});
	}

	return new Transform({
		objectMode: true,
		transform
	});
}
```
- example usage
```shell
...
			// ignore warnings
			return util.filterResult(result, options.quiet);
		}

		return result;
	}

	return util.transform((file, enc, cb) => {
		const filePath = path.relative(process.cwd(), file.path);

		if (file.isNull()) {
			cb(null, file);
			return;
		}
...
```

#### <a name="apidoc.element.gulp-eslint.util.tryResultAction"></a>[function <span class="apidocSignatureSpan">gulp-eslint.util.</span>tryResultAction (action, result, done)](#apidoc.element.gulp-eslint.util.tryResultAction)
- description and source-code
```javascript
tryResultAction = function (action, result, done) {
	try {
		if (action.length > 1) {
			// async action
			action.call(this, result, done);
		} else {
			// sync action
			action.call(this, result);
			done();
		}
	} catch (error) {
		done(error == null ? new Error('Unknown Error') : error);
	}
}
```
- example usage
```shell
...
gulpEslint.result = action => {
	if (typeof action !== 'function') {
		throw new Error('Expected callable argument');
	}

	return util.transform((file, enc, done) => {
		if (file.eslint) {
			util.tryResultAction(action, file.eslint, util.handleCallback(done, file));
		} else {
			done(null, file);
		}
	});
};

/**
...
```

#### <a name="apidoc.element.gulp-eslint.util.writeResults"></a>[function <span class="apidocSignatureSpan">gulp-eslint.util.</span>writeResults (results, formatter, writable)](#apidoc.element.gulp-eslint.util.writeResults)
- description and source-code
```javascript
(results, formatter, writable) => {
	if (!results) {
		results = [];
	}

	const firstResult = results.find(result => result.config);

	const message = formatter(results, firstResult ? firstResult.config : {});
	if (writable && message != null && message !== '') {
		writable(message);
	}
}
```
- example usage
```shell
...
* @param {(Function|Stream)} [writable=gulp-util.log] - A funtion or stream to write the formatted ESLint results.
* @returns {stream} gulp file stream
*/
gulpEslint.formatEach = (formatter, writable) => {
	formatter = util.resolveFormatter(formatter);
	writable = util.resolveWritable(writable);

	return gulpEslint.result(result => util.writeResults([result], formatter, writable));
};

/**
* Wait until all files have been linted and format all results at once.
*
* @param {(String|Function)} [formatter=stylish] - The name or function for a ESLint result formatter
* @param {(Function|stream)} [writable=gulp-util.log] - A funtion or stream to write the formatted ESLint results.
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
