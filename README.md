grunt-foreman [![NPM Module](http://img.shields.io/npm/v/grunt-foreman.svg?style=flat-square)](https://npmjs.org/package/grunt-foreman)
===

[![NPM](https://nodei.co/npm/grunt-foreman.png?downloads=true)](https://nodei.co/npm/grunt-foreman/)


### Usage
Use as such, if your procfile is called `Procfile` and you don't need anything else:
```javascript
grunt.loadNpmTasks("grunt-foreman");

grunt.registerTask("serve", "foreman");
```

Optionally, you can add configuration (by target, 'dev' as default) for one, many or any of:

* one or more `env` files
* a `Procfile`
* the port to use

```javascript
grunt.initConfig({
    foreman: {
        dev: {
            env: [ "development.env", "application.env" ],
            procfile: "Procfile.dev",
            port: 7000
        } //,
    //  production: {
    //      ...
    //  }
    }        
});
```

Enjoy!
