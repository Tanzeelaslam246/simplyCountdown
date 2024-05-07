# SimplyCountdown.js

## Why Another Countdown?

SimplyCountdown.js was developed on a boring day to meet the need for a very basic JavaScript countdown library. It's perfect for creating 'under construction' pages and more.

## Getting Started

Install SimplyCountdown.js via npm or bower:

```bash
$ yarn add simplycountdown.js

# or

$ npm install simplycountdown.js
```

// Example with default parameters
simplyCountdown('[CSS-SELECTOR]', {
year: 2019, // required
month: 6, // required
day: 28, // required
// other parameters...
});

// Init with existing JavaScript Object
let myElement = document.querySelector('.my-countdown');
simplyCountdown(myElement, { /_ options _/ });

let multipleElements = document.querySelectorAll('.my-countdown');
simplyCountdown(multipleElements, { /_ options _/ });
Changelog
1.7.0
Countdowns can be initialized directly with HTML elements using variables like:
document.getElementById
document.querySelector
document.querySelectorAll
etc...
1.6.0
Compatibility with languages like German for plurals (PR #15), thanks to q30t
1.5.0
Resolve #10 - Add countup support
Upgrade yarn dev dependencies
Some minor code reformatting
1.4.0
Remove Bower support
Migrate from LESS to SASS (scss) for demo and themes
Migrate lib from ES5 to a basic ES6
Remove JSLint support
Add ESLint support based on customized Airbnb rules
