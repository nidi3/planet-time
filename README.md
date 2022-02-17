# planet-time

[Take your time](https://nidi3.github.io/planet-time)

Use this snippet to show the planet timer.

```html

<iframe id="planet-time" style="border: none; width: 100%; height: 250px;"></iframe>
<script>
fetch('https://api.github.com/repos/nidi3/planet-time/contents/planet-time.html')
        .then(res => res.json())
        .then(data => document.getElementById('planet-time').src = 'data:text/html;base64,' + encodeURIComponent(data['content']));
</script>
```
