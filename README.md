PIGNOSE-LayerSlider
===================

> This slider supports the parallax sliding effects.

- Version 0.0.1
- Licenced MIT
- Update Aug, 04, 2014

![Sample](http://www.pigno.se/barn/PIGNOSE-LayerSlider/assets/img/sample.jpg)

## Start

### Installation

> This plugin needs `jQuery` library.

- Check the jQuery library at [here](http://jquery.com/download/) `Recommend version 1.11.x higher`
- Also need jQuery easing library at [here](http://gsgd.co.uk/sandbox/jquery/easing/)
- And insert the snippets

 ```html
<script type="text/javascript" src="[[Your directory for javascript]]/jquery.latest.min.js"></script>
<script type="text/javascript" src="[[Your directory for javascript]]/jquery.easing.js"></script>
```

### Usage

[Check demo and documents](http://www.pigno.se/barn/PIGNOSE-LayerSlider/)

> Refer to below exhibit.

#### HTML

```html
<div id="visual">
	<div class="slide-visual">
		<!-- Slide Image Area (1000 x 424) -->
		<ul class="slide-group">
			<li><img src="assets/img/visual_slide01.jpg" alt="Dummy Image" /></li>
			<li><img src="assets/img/visual_slide02.jpg" alt="Dummy Image" /></li>
			<li><img src="assets/img/visual_slide03.jpg" alt="Dummy Image" /></li>
			<li><img src="assets/img/visual_slide04.jpg" alt="Dummy Image" /></li>
			<li><img src="assets/img/visual_slide05.jpg" alt="Dummy Image" /></li>
			<li><img src="assets/img/visual_slide06.jpg" alt="Dummy Image" /></li>
		</ul>

		<!-- Slide Description Image Area (316 x 328) -->
		<div class="script-wrap">
			<ul class="script-group">
				<li><div class="inner-script"><img src="http://placehold.it/276x288/f8f8f8/b71200" alt="Dummy Image" /></div></li>
				<li><div class="inner-script"><img src="http://placehold.it/276x288/f8f8f8/b71200" alt="Dummy Image" /></div></li>
				<li><div class="inner-script"><img src="http://placehold.it/276x288/f8f8f8/b71200" alt="Dummy Image" /></div></li>
				<li><div class="inner-script"><img src="http://placehold.it/276x288/f8f8f8/b71200" alt="Dummy Image" /></div></li>
				<li><div class="inner-script"><img src="http://placehold.it/276x288/f8f8f8/b71200" alt="Dummy Image" /></div></li>
				<li><div class="inner-script"><img src="http://placehold.it/276x288/f8f8f8/b71200" alt="Dummy Image" /></div></li>
			</ul>
			<div class="slide-controller">
				<a href="#" class="btn-prev"><img src="assets/img/btn_prev.png" alt="Prev Slide" /></a>
				<a href="#" class="btn-play"><img src="assets/img/btn_play.png" alt="Start Slide" /></a>
				<a href="#" class="btn-pause"><img src="assets/img/btn_pause.png" alt="Pause Slide" /></a>
				<a href="#" class="btn-next"><img src="assets/img/btn_next.png" alt="Next Slide" /></a>
			</div>
		</div>
	</div>
</div>
```

#### Javascript

```javascript
$(window).load(function() {
	$('#visual').pignoseLayerSlider({
		play    : '.btn-play',
		pause   : '.btn-pause',
		next    : '.btn-next',
		prev    : '.btn-prev'
	});
});
```

#### Options

| name | value | default | description |
|------|-------|---------|-------------|
| speed | `number` | 1200 | the millisecond time for speed of the slide animation. |
| interval | `number` | 3000 | the millisecond time for interval of the slide animation. |
| direction | `string` | right | the direction of slide animation. |
| diffTime | `number` | 300 | the millisecond time that you wanna make parallax between main view and sub view. |
| controlAnim | `boolean` | true | if you set this property to false, this plugin will ignore the status of animation queue. |
| pagination | `boolean` | true | if you set this property to true, pagination controller will show. |
| auto | `boolean` | true | if you set this property to true, this slider will start automatically. |
