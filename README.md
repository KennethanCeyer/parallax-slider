PIGNOSE-LayerSlider
===================

> This slider support the parallax sliding effects. [See Demo](http://www.pigno.se/barn/PIGNOSE-LayerSlider/)

- Version 0.0.1
- Licenced MIT
- Update Aug, 04, 2014

![Sample](http://www.pigno.se/barn/PIGNOSE-LayerSlider/assets/img/sample.jpg)

### Usage

> Please refer index.html document.

#### HTML

```html
<div id="slide-view">
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
	$('#slide-view').pignoseLayerSlider({
		play    : '.btn-play',
		pause   : '.btn-pause',
		next    : '.btn-next',
		prev    : '.btn-prev'
	});
});
```
