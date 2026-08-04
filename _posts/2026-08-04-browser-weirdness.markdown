---
layout: post
title:  "Browser Weirdness"
date:   2026-08-04 1:48:23 +0900
categories: programming technology
---
Did you know that the following code will not produce the same results in firefox vs chromium?
```html
<script>
let e = document.createElement('img');
e.src = "https://example.com/image.png";
e.onload = () => {
    e.sizes = "auto";
	console.log("onload")
};
</script>
```
Firefox will output `onload` twice, whereas the latter will call it in an endless loop. To add further confusion,
```html
<script>
let e = document.createElement('img');
e.src = "https://example.com/image.png";
e.onload = () => {
    e.width = 100;
	console.log("onload")
};
</script>
```
will only trigger `onload` once (despite the spec being pretty clear it should happen a bunch of times) and 
```html
<script>
let e = document.createElement('img');
e.src = "https://example.com/image.png";
e.onload = () => {
    e.sizes = "auto";
	console.log("onload")
};
</script>
```
will be an endless loop in all three browsers (despite what an open issue on the whatwg spec repo says should be the standard). Another wonderful instance of browsers being bad. Discovered by yours truly.
