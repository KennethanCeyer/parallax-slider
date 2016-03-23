PIGNOSE-ParallaxSlider
===================

> jQuery slider supporting parallax effects.

[![npm version](https://badge.fury.io/js/pg-parallaxslider.svg)](https://badge.fury.io/js/pg-parallaxslider) [![Bower version](https://badge.fury.io/bo/pg-parallaxslider.svg)](https://badge.fury.io/bo/pg-parallaxslider) [![Join the chat at https://gitter.im/KennethanCeyer/PIGNOSE](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/KennethanCeyer/PIGNOSE?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

- Licenced under MIT
- This plugin supports most browsers including  Internet Explorer 8+, Chrome, Firefox, Safari and Opera.
- And also this plugin tested on Safari for MAC Platform, It is definitely safe on the most modern Browsers!

![Sample](http://www.nhpcw.com/upload/%25EB%258B%25A4%25EC%259A%25B4%25EB%25A1%259C%25EB%2593%259C%2B%25282%2529_021116021919.png)

## Getting Started

### Installation

> This plugin needs `jQuery` library.

- Check the jQuery library at [here](http://jquery.com/download/) `Recommend version 1.11.x higher`
- Also you need jQuery easing library at [here](http://gsgd.co.uk/sandbox/jquery/easing/) for animation.
- And insert this snippets

 ```html
<script type="text/javascript" src="[[Your directory for javascript]]/jquery.latest.min.js"></script>
<script type="text/javascript" src="[[Your directory for javascript]]/jquery.easing.js"></script>
```

- import pignose-parallaxslider files(css, js)

 ```html
 <link rel="stylesheet" href="dist/css/pignose.parallaxslider.min.css" />
 <script type="text/javascript" src="dist/js/pignose.parallaxslider.min.js"></script>
```

### If you use Bower

1. open terminal and type those command line.

 ```shell
bower install pg-parallaxslider
 ```
 
2. move `dist/js/pignose.parallaxslider.min.js` and `dist/css/pignose.parallaxslider.min.css` to your project folder.

### If you use npm

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
			<li><img src="assets/img/visual_slide01.jpg" alt="slider image" /></li>
			<li><img src="assets/img/visual_slide02.jpg" alt="slider image" /></li>
			<li><img src="assets/img/visual_slide03.jpg" alt="slider image" /></li>
			<li><img src="assets/img/visual_slide04.jpg" alt="slider image" /></li>
			<li><img src="assets/img/visual_slide05.jpg" alt="slider image" /></li>
			<li><img src="assets/img/visual_slide06.jpg" alt="slider image" /></li>
		</ul>

		<!-- Slide Description Image Area (316 x 328) -->
		<div class="script-wrap">
			<ul class="script-group">
				<li><div class="inner-script"><img src="http://placehold.it/276x288/f8f8f8/b71200" alt="thumbnail slider image" /></div></li>
				<li><div class="inner-script"><img src="http://placehold.it/276x288/f8f8f8/b71200" alt="thumbnail slider image" /></div></li>
				<li><div class="inner-script"><img src="http://placehold.it/276x288/f8f8f8/b71200" alt="thumbnail slider image" /></div></li>
				<li><div class="inner-script"><img src="http://placehold.it/276x288/f8f8f8/b71200" alt="thumbnail slider image" /></div></li>
				<li><div class="inner-script"><img src="http://placehold.it/276x288/f8f8f8/b71200" alt="thumbnail slider image" /></div></li>
				<li><div class="inner-script"><img src="http://placehold.it/276x288/f8f8f8/b71200" alt="thumbnail slider image" /></div></li>
			</ul>
			<div class="slide-controller">
				<a href="#" class="btn-prev"><img src="assets/img/btn_prev.png" alt="prev Slide" /></a>
				<a href="#" class="btn-play"><img src="assets/img/btn_play.png" alt="start Slide" /></a>
				<a href="#" class="btn-pause"><img src="assets/img/btn_pause.png" alt="pause Slide" /></a>
				<a href="#" class="btn-next"><img src="assets/img/btn_next.png" alt="next Slide" /></a>
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
| diffTime | `number` | 300 | the millisecond time that you want to put between main view and sub view as a  parallax. |
| controlAnim | `boolean` | true | if you set this property to false, this plugin will ignore the status of animation queue. |
| pagination | `boolean` | true | if you set this property to true, pagination controller will show. |
| auto | `boolean` | true | if you set this property to true, this slider will start automatically. |
| isLocal | `boolean` | true | this property set that each of controllers(play, stop, prev and next) is belong local of those container or not. |
| play | `jQuery object` | null | the jQuery object of play button. |
| pause | `jQuery object` | null | the jQuery object of pause button. |
| next | `jQuery object` | null | the jQuery object of next button. |
| prev | `jQuery object` | null | the jQuery object of prev button. |
| afterMove | `callback` | null | this callback will be called after slider moved. |

## Issues

> We are wating for your requests.

Please report to us, If you find some problems.

Thank you!
