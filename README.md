# grunt-nopache

> Grunt nopache task.

## Getting Started
This plugin requires Grunt `~0.4.5`

If you haven't used [Grunt](http://gruntjs.com/) before, be sure to check out the [Getting Started](http://gruntjs.com/getting-started) guide, as it explains how to create a [Gruntfile](http://gruntjs.com/sample-gruntfile) as well as install and use Grunt plugins. Once you're familiar with that process, you may install this plugin with this command:

```shell
npm install grunt-nopache --save-dev
```

Once the plugin has been installed, it may be enabled inside your Gruntfile with this line of JavaScript:

```js
grunt.loadNpmTasks('grunt-nopache');
```

## The "nopache" task

### Overview
In your project's Gruntfile, add a section named `nopache` to the data object passed into `grunt.initConfig()`.

```js
grunt.initConfig({
  nopache: {
    options: {
      // Task-specific options go here.
    },
    your_target: {
      // Target-specific file lists and/or options go here.
    },
  },
});
```

### Options

#### options.base
Type: `String`
Default value: `'.'`

The path used for the base of the nopache server.

#### options.port
Type: `Integer`
Default value: `2400`

A Integer used for the port the server will listen on.

#### options.keepAlive
Type: `Boolean`
Default value: `false`

Sets whether the server should run in the background.  If running as a web server the suggested value is `true`.

#### options.php
Type: `Object` or `String`
Default value: `null`

If a string is provided, grunt will try to resolve it as a filename and use the file to import an object via `require`.  In either case, the object is passed to nopache to mock php files.  See [nopache](http://www.npmjs.com/packages/nopache) for details.

## Contributing
In lieu of a formal styleguide, take care to maintain the existing coding style. Add unit tests for any new or changed functionality. Lint and test your code using [Grunt](http://gruntjs.com/).

## Release History
_(Nothing yet)_
