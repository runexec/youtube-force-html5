```javascript
// ==UserScript==
// @name        youtube-force-html5
// @namespace   youtube-force-html5
// @include     https://www.youtube.com/*
// @version     1
// ==/UserScript==
// No Flash + youtube-nocookie embed =
// Forces Youtube to display HTML5 player

if(confirm('Html5?')) {
    x = document.URL.split('/');
    url = 'https://www.youtube-nocookie.com/embed/';
    url += x[x.length-1];
    document.location = url;
}
```
