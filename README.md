#ngCircularJSON

An [Angular](https://angularjs.org/) service for [CircularJSON](https://github.com/WebReflection/circular-json)

##Installation

```
bower install ng-circular-json --save
```

##Usage

First, include the ng-circular-json.js file in your html.  The example assumes you have bower using the default 
components directory. 

```html
<script src="bower_components/ng-circular-json/dist/ng-circular-json.js"></script>
```

Second, include the ngCircularJSON module in you Angular app:

```
angular.module('exampleApp', ['ngCircularJSON']);
```

Then, inject the *CircularJSON* service wherever you need it. For example, in a controller:

```javascript
angular.module('exampleApp').controller('ExampleController', [function($scope, CircularJSON) {
    console.log('Logging a JSON Object with a possible circular structure: ' + CircularJSON.stringify($scope.exampleObject)
}]);
```

## Code
I used [CoffeeScript](http://coffeescript.org/) to write this library because I prefer it. The [gulp](http://gulpjs.com/)
build will compile the CoffeeScript into the javascript file.
   
## Issues
Please use the github issue tracker to add any issues with the code.

## Contributing
Contributions are welcome. Please fork the repo and issue a pull request with any changes you would like made.
    
## Special Thanks
I would like to extend a special thanks to James Hill at [oblongmana.com](http://oblongmana.com/) for his article on
[Angular - 3rd Party Injection](http://oblongmana.com/articles/angular-third-party-injection-pattern/)