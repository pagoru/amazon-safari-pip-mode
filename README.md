# amazon-safari-pip-mode
Start Amazon instant video in Safari (macOS) and use Picture in Picture Mode.

## Steps:
1. Start stream on amazon
2. Open console (Web Inspector) (CMD+ALT+i)
  * Safari dev. tools should be aktivated [how to](https://developer.apple.com/library/content/documentation/AppleApplications/Conceptual/Safari_Developer_Guide/GettingStarted/GettingStarted.html)
3. Past this:
``` javascript
Object.values(document.getElementsByTagName('video')).forEach(video => video.webkitSetPresentationMode("picture-in-picture"));
```
  * Sometimes you need to click Pause and then play before you run this code.
4. Ready (Close Inspector)
