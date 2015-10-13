PIGNOSE-ParallaxSlider
===================

> The slider supports parallax slide effect.

[![npm version](https://badge.fury.io/js/pg-parallaxslider.svg)](https://badge.fury.io/js/pg-parallaxslider) [![Join the chat at https://gitter.im/KennethanCeyer/PIGNOSE](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/KennethanCeyer/PIGNOSE?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

- Licenced MIT
- This plugin supports most browser Internet Explorer 8+, Chrome, Firefox, Safari, Opera.
- The plugin tested Safari for `MAC Platform`, This is definitely safe on Most Browsers!
- Support `Bower`

![Sample](http://www.nhpcw.com/upload/2015-10-10%2B%25EC%2598%25A4%25EC%25A0%2584%2B1-03-59_101015010418.jpg)

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

- And load pignose-parallaxslider files(css, js)

 ```html
 <link rel="stylesheet" href="assets/css/pignose.parallaxslider.min.css" />
 <script type="text/javascript" src="assets/js/pignose.parallaxslider.min.js"></script>
```

### If you are using Bower

1. open a command line and type this

 ```shell
bower install pg-parallaxslider
 ```
 
2. move `assets/js/pignose.parallaxslider.min.js` and `assets/css/pignose.parallaxslider.min.css` to your project folder.

### If you are using npm

1. open a command line and type this

 ```shell
npm install pg-parallaxslider
 ```

## Usage

- [Check demo and documents](http://www.pigno.se/barn/PIGNOSE-ParallaxSlider/)

> Refer to below exhibit.

#### HTML

```html
<div id="visual">
	<div class="slide-visual">
		<!-- Slide Image Area (1000 x 424) -->
		<ul class="slide-group">
			<li><img src="assets/img/visual_slide01.jpg" alt="Slider Image" /></li>
			<li><img src="assets/img/visual_slide02.jpg" alt="Slider Image" /></li>
			<li><img src="assets/img/visual_slide03.jpg" alt="Slider Image" /></li>
			<li><img src="assets/img/visual_slide04.jpg" alt="Slider Image" /></li>
			<li><img src="assets/img/visual_slide05.jpg" alt="Slider Image" /></li>
			<li><img src="assets/img/visual_slide06.jpg" alt="Slider Image" /></li>
		</ul>

		<!-- Slide Description Image Area (316 x 328) -->
		<div class="script-wrap">
			<ul class="script-group">
				<li><div class="inner-script"><img src="http://placehold.it/276x288/f8f8f8/b71200" alt="Thumbnail Slider Image" /></div></li>
				<li><div class="inner-script"><img src="http://placehold.it/276x288/f8f8f8/b71200" alt="Thumbnail Slider Image" /></div></li>
				<li><div class="inner-script"><img src="http://placehold.it/276x288/f8f8f8/b71200" alt="Thumbnail Slider Image" /></div></li>
				<li><div class="inner-script"><img src="http://placehold.it/276x288/f8f8f8/b71200" alt="Thumbnail Slider Image" /></div></li>
				<li><div class="inner-script"><img src="http://placehold.it/276x288/f8f8f8/b71200" alt="Thumbnail Slider Image" /></div></li>
				<li><div class="inner-script"><img src="http://placehold.it/276x288/f8f8f8/b71200" alt="Thumbnail Slider Image" /></div></li>
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
	$('#visual').pignoseParallaxSlider({
		play    : '.btn-play',
		pause   : '.btn-pause',
		next    : '.btn-next',
		prev    : '.btn-prev'
	});
});
```

## Options

| name | value | default | description |
|------|-------|---------|-------------|
| speed | `number` | 1200 | the millisecond time for speed of the slide animation. |
| interval | `number` | 3000 | the millisecond time for interval of the slide animation. |
| direction | `string` | right | the direction of slide animation. |
| diffTime | `number` | 300 | the millisecond time that you wanna make parallax between main view and sub view. |
| controlAnim | `boolean` | true | if you set this property to false, this plugin will ignore the status of animation queue. |
| pagination | `boolean` | true | if you set this property to true, pagination controller will show. |
| auto | `boolean` | true | if you set this property to true, this slider will start automatically. |
| isLocal | `boolean` | true | it is about play/pause/next/prev button area. it will find control button from anywhere, if you set the property true. |
| play | `jQuery object` | null | the jQuery object of play button. |
| pause | `jQuery object` | null | the jQuery object of pause button. |
| next | `jQuery object` | null | the jQuery object of next button. |
| prev | `jQuery object` | null | the jQuery object of prev button. |
| afterMove | `callback` | null | this callback will be called after slider moved. |

## Issues

> We are welcome about announcing the issue.

Please inform us, If you find some problems.

Thank you!
