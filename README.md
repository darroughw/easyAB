# [easyAB](http://srom.github.io/easyAB/)

easyAB is a light-weight (< 2 Ko) jQuery / Zepto plugin for easily setting up A/B and multivariate tests using Google Analytics.<br>
This tool aims at helping entrepreneurs and tech savvy building better landing pages for their projects and products.

## Quick start

```javascript
// change the color of .my-button for 50% of my visitors and
// track the users with analytics using a single method!
$('.my-button').easyab({
  'slot': 5, // set the custom var on the slot 5
  'name': 'test-button',
  'default-value': 'green',
  'alternatives': [
    {
      // set an alternative
      'value': 'blue',
      'alternative': function($this) { $this.css('background-color', 'blue'); }
    }
  ],
});
```

Comprehensive doc: [srom.github.io/easyAB/](http://srom.github.io/easyAB/)

## Road map

- Add support for [Universal Analytics](https://support.google.com/analytics/answer/2790010?hl=en)
- Add support for [Content Experiment API](http://analytics.blogspot.fr/2013/06/google-analytics-becomes-robust-testing.html)
- Add better ways to track tests in dev mode

## License

Copyright 2013 [Romain Strock](https://twitter.com/_srom) - [MIT License](https://github.com/srom/easyAB/blob/master/LICENSE)

[![githalytics.com alpha](https://cruel-carlota.pagodabox.com/3b9f5baa8c54378cb668b5c1a2ede638 "githalytics.com")](http://githalytics.com/srom/easyAB)
