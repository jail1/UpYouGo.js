# Upyougo.js
`Elevator.js` lives entirely within the js realm, which makes things fairly simple to use.

You'll need to create a new instance of Up, using new Up, and pass it some audio settings.
```html
<script>
// Elevator script included on the page, already.

window.onload = function() {
  var elevator = new Up({
    mainAudio: '/src/to/audio.mp3',
    endAudio: '/src/to/end-audio.mp3'
  });
}

// You can run the elevator, by calling.
elevator.elevate();
</script>
```

You can also add an "element" option, clicking this element will invoke the "Scroll to top" functionality, we all love and crave.
```html
<div class="elevator-button">Back to Top</div>

<script>
// Elevator script included on the page, already.

window.onload = function() {
  var Up = new Up({
    element: document.querySelector('.up-button'),
    mainAudio: '/src/to/audio.mp3',
    endAudio: '/src/to/end-audio.mp3'
  });
}
</script>
```

If you're really serious (boring), you don't have to use audio... and can also set a fixed time to scroll to the top
```html
<div class="elevator-button">Back to Top</div>

<script>
// Elevator script included on the page, already.

window.onload = function() {
  var elevator = new Elevator({
    element: document.querySelector('.elevator-button'),
    duration: 1000 // milliseconds
  });
}
</script>
```
