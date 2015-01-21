# protractor-cucumber-junit

Provide a cucumber-js support file and json2xml converter to generate JUnitXML file for CI

## Install

1. Copy reporter/reporter.js to your cucumber support folder

2. Cucumberjs-junitxml should be added to your test codebase as a dev dependency.  You can do this with:

``` shell
$ npm install cucumberjs-junitxml --save-dev 
```

Alternatively you can manually add it to your package.json file:

``` json
{
  "devDependencies" : {
    "cucumberjs-junitxml": "latest"
  }
}
```

then install with:

``` shell
$ npm install --dev
```

## Run

Run your cucumber-js command. The reports should be saved to tests/features/output/

``` shell
$ ./node_modules/.bin/cucumber.js
```

And you can manually convert your json to xml by

``` shell
$ cat cucumber_report.json | ./node_modules/.bin/cucumber-junit > cucumber_report.xml
```

## License

[MIT](http://opensource.org/licenses/MIT)
