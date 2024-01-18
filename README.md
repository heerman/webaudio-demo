# Web Audio Demo

A simple Web Audio API html demo

### Demo

```html
<!DOCTYPE html>
<button id="playButton">Play Tone</button>
<script>
document.getElementById('playButton').addEventListener('click', function() {
    var audioCtx = new AudioContext()
    var osc = audioCtx.createOscillator()
    osc.connect(audioCtx.destination)
    osc.start()
    osc.stop(audioCtx.currentTime + 1)
})
</script>
```
