# Upyougo.js

```html
<script>
// up script included on the page, already.

window.onload = function() {
  var up = new Up({
    mainAudio: '/src/to/audio.mp3',
    endAudio: '/src/to/end-audio.mp3'
  });
}

// You can run the up, by calling.
up.elevate();
</script>
```

```html
<div class="up-button">Back to Top</div>

<script>
// Up script included on the page, already.

window.onload = function() {
  var Up = new Up({
    element: document.querySelector('.up-button'),
    mainAudio: '/src/to/audio.mp3',
    endAudio: '/src/to/end-audio.mp3'
  });
}
</script>
```

```html
<div class="up-button">Back to Top</div>

<script>
// up script included on the page, already.

window.onload = function() {
  var elevator = new Elevator({
    element: document.querySelector('.up-button'),
    duration: 1000 // milliseconds
  });
}
</script>
```
