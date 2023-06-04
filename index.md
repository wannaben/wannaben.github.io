
THIS IS A TEST ONLY

<video controls width="400" autoplay="true">
    <source src="https://tst.dynamsoft.com/public/docs/dbr/javascript/How%20to%20Use%20Dynamsoft%20Barcode%20Reader%20JavaScript%20SDK%20v1.1.mp4">
</video>

```javascript
// Check if the video has already played in the current session
if (sessionStorage.getItem('videoPlayed') !== 'true') {
  // Save the information in session storage to prevent autoplay on subsequent visits
  sessionStorage.setItem('videoPlayed', 'true');
} else {
  // Remove the autoplay attribute if the video has already played
  var video = document.getElementById('myVideo');
  video.removeAttribute('autoplay');
}
```


# Welcome to My Website

Please select an option:

- [About](about.md)
- [Contact](contact.md)


