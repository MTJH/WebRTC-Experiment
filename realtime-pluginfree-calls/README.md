**Just copy HTML code in your site and that's all you need to do. Nothing to install! No requirements!**

====
# Browser Support

This [WebRTC Experiment](https://webrtc-experiment.appspot.com/calls/) works fine on following web-browsers:

| Browser        | Support           |
| ------------- |:-------------:|
| Firefox | [Aurora](http://www.mozilla.org/en-US/firefox/aurora/) |
| Firefox | [Nightly](http://nightly.mozilla.org/) |
| Google Chrome | [Stable](https://www.google.com/intl/en_uk/chrome/browser/) |
| Google Chrome | [Canary](https://www.google.com/intl/en/chrome/browser/canary.html) |
| Google Chrome | [Beta](https://www.google.com/intl/en/chrome/browser/beta.html) |
| Google Chrome | [Dev](https://www.google.com/intl/en/chrome/browser/index.html?extra=devchannel#eula) |

--

[How to share audio-only streams](https://webrtc-experiment.appspot.com/docs/how-to-share-audio-only-streams.html) ? Early workaround for Chrome Canary!

```javascript
audio.src = webkitURL.createObjectURL(event.stream);
audio.addEventListener('play', function () {
	this.muted = false;
	this.volume = 1;
}, false);

audio.play();
```

====
## License & Credits

MIT: https://webrtc-experiment.appspot.com/licence/ : Copyright (c) 2013 [Muaz Khan](https://plus.google.com/100325991024054712503).
