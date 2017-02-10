# svg slider using d3

jake kara
jake@jakekara.com

# usage

See index.html for full demo code.

HTML:

```
      <h1 id="output">Slider demo</h1>
      <svg id="slider_svg" width="100%"></svg>
```

JS:

```
      var s = new slider()
      	  .svg(d3.select("#slider_svg")) // an SVG element -- required
      	  .values([-100, 100]) // range of values -- required
      	  .draw() // draws the slider -- required when ready. recalled on resize
      	  .callback(function(v){ // set up a callback function -- optional
		d3.select("#output").text(v); // v is the current value of the slider
      		});
```