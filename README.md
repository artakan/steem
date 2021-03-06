# SteemJS
SteemJS the JavaScript API for Steem blockchain

## Documentation 
Here is full documentation: https://github.com/adcpm/steem/tree/master/doc

## Browser 
```html 
<script src="./steem.min.js"></script>
<script>
steem.getAccounts(['ned', 'dan'], function(err, response){
    console.log(err, response);
});
</script>
```

## Server
## Install
```
$ npm install steem --save
```

## Examples
### Get Accounts
```js
var Steem = require('steem');
var steem = new Steem();

steem.getAccounts(['ned', 'dan'], function(err, result) {
	console.log(err, result);
});
```

### Get State
```js 
steem.getState('/trends/funny', function(err, result) {
	console.log(err, result);
});
```

### Get Config
```js 
steem.getConfig(function(err, result) {
	console.log(err, result);
});
```

## Contributions
Patches are welcome! Contributors are listed in the package.json file. Please run the tests before opening a pull request and make sure that you are passing all of them. If you would like to contribute, but don't know what to work on, check the issues list or on Slack https://steem.slack.com/ channel #steemjs.

## Issues
When you find issues, please report them!

## License
MIT