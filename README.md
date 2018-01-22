# browser-open


### openBrowser(url: string): boolean
Attempts to open the browser with a given URL.
On Mac OS X, attempts to reuse an existing Chrome tab via AppleScript.
Otherwise, falls back to opn behavior.

var path = require('path');
var browserOpen = require('browser-open');

if (browserOpen('http://localhost:3000')) {
  console.log('The browser tab has been opened!');
}
