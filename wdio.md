### WDIO 

* Use `chai` assertion library: `npm install chai`

* Add to Webstorm support `chai` and `mocha`: `Preferences | Languages & Frameworks | JavaScript | Libraries`


### Actions

```javascript

// Open URL
browser.url('http://localhost:3006/');

// Get text from tag using CSS selector
const actual = $('h1').getText();
// using XPath
const actual = $('//h1').getText();

// Selector XPath
const submitButtonSelector = $('//button[@type="submit"]');

// Get element by selector
const submitButton = $(submitButtonSelector);

// Click on element
submitButton.click();

// Get CSS property (returns object)
const color = $('//button[@type="submit"]').getCSSProperty('color');


// Set value to input field
const emailField = $('//*[@name="email"]');
emailField.setValue('5901867@gmail.com');

// Select from dropdown
// Check radio button 
// Check checkbox
// Drag-and-drop

// Pause 1 sec
browser.pause(1000);

```

### Run options

Run scecific file `wdio wdio.conf.js --spec ./test/specs/login.js`
