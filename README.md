# grunt-def

> Grunt plugin for element.def.

## Getting Started
This plugin requires Grunt.

If you haven't used [Grunt](http://gruntjs.com/) before, be sure to check out the [Getting Started](http://gruntjs.com/getting-started) guide, as it explains how to create a [Gruntfile](http://gruntjs.com/sample-gruntfile) as well as install and use Grunt plugins. Once you're familiar with that process, you may install this plugin with this command:

```shell
npm install grunt-def --save-dev
```

Once the plugin has been installed, it may be enabled inside your Gruntfile with this line of JavaScript:

```js
grunt.loadNpmTasks('grunt-def');
```

## The "def" task

### Overview
In your project's Gruntfile, add a section named `def` to the data object passed into `grunt.initConfig()`.

```js
grunt.initConfig({
  def: {
    options: {
      // Task-specific options go here.
    },
    your_target: {
      // Target-specific file lists and/or options go here.
    },
  },
})
```

### Options

#### options.defName
Type: `String`
Default value: `'def'`

A string value that is used to make sure to find all the `def` functions in source files

### Usage Examples

#### Default Options

```js
grunt.initConfig({
  def: {
    files: {
      'dest/default_options': 'src/testing',
    },
  },
})
```

#### Custom Options

```js
grunt.initConfig({
  def: {
    options: {
      defName: 'customFn'
    },
    files: {
      'dest/default_options': 'src/testing',
    },
  },
})
```

## Release History

[History](CHANGELOG.md)

## License
Copyright (c) 2015 Zhonglei Qiu. Licensed under the MIT license.
