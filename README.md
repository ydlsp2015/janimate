jAnimate
========
Plugin to help you use [Animate.css](http://daneden.github.io/animate.css/) with jQuery.  

**Interactive Demo/Examples:** http://renatorib.github.io/janimate/

## Animate.css
Do not know Animate.css? If you're new to the wonderful world of Animate.css, I highly recommend you [visit this link](http://daneden.github.io/animate.css/), to see what you can do with Animate.css.

## Download & Usage
NOTE: You need have **jQuery** and **Animate.css** in your project to use janimate.

You can use janimate with `bower`, `npm` or [download by rawgit file](https://cdn.rawgit.com/renatorib/janimate/master/dist/janimate.min.js)

### via bower
`bower install jquery-janimate`  
```html
<script src="bower_components/jquery-janimate/dist/janimate.min.js"></script>
```
### via npm
`npm install janimate`  
```html
<script src="node_modules/janimate/dist/janimate.min.js"></script>
```
### via rawgit cdn
`https://cdn.rawgit.com/renatorib/janimate/master/dist/janimate.min.js`
```html
<script src="https://cdn.rawgit.com/renatorib/janimate/master/dist/janimate.min.js"></script>
```

## Difference between jAnimate and jAnimateOnce
`jAnimateOnce()` clean the animation classes when the animation ends, which means that any effect that you do, it will return to normal. Suitable for the purposes of **Attention Seekers**. Not suitable for when you want the final animation stand, as effects of **Exits** and **Entrances**. In these cases, you should use the `jAnimate()`.

## Basic example
```html
<!DOCTYPE html>
<head>
  <meta charset="utf-8">
  <title>janimate example</title>
  <link rel="stylesheet" href="https://cdn.rawgit.com/daneden/animate.css/master/animate.css">
</head>
<body>

  <h1>Hello jAnimate</h1>
  <button class="e1">swing</button>
  <button class="e2">shake</button>
  <button class="e3">fadeOut</button>
  <button class="e4">fadeIn</button>

  <script src="https://code.jquery.com/jquery-1.11.2.min.js"></script>
  <script src="https://cdn.rawgit.com/renatorib/janimate/master/dist/janimate.min.js"></script>
  <script type="text/javascript">
      $(document).ready(function(){

        $('.e1').click(function(){
          $('h1').jAnimateOnce('swing');
        });

        $('.e2').click(function(){
          $('h1').jAnimateOnce('shake');
        });

        $('.e3').click(function(){
          $('h1').jAnimate('fadeOut');
        });

        $('.e4').click(function(){
          $('h1').jAnimate('fadeIn', function(self, effect){
            alert(effect + ' finish');
          });
        });

      });
  </script>
  
</body>
```

## Effects

* bounce
* flash
* pulse
* rubberBand
* shake
* swing
* tada
* wobble
* bounceIn
* bounceInDown
* bounceInLeft
* bounceInRight
* bounceInUp
* bounceOut
* bounceOutDown
* bounceOutLeft
* bounceOutRight
* bounceOutUp
* fadeIn
* fadeInDown
* fadeInDownBig
* fadeInLeft
* fadeInLeftBig
* fadeInRight
* fadeInRightBig
* fadeInUp
* fadeInUpBig
* fadeOut
* fadeOutDown
* fadeOutDownBig
* fadeOutLeft
* fadeOutLeftBig
* fadeOutRight
* fadeOutRightBig
* fadeOutUp
* fadeOutUpBig
* flipInX
* flipInY
* flipOutX
* flipOutY
* lightSpeedIn
* lightSpeedOut
* rotateIn
* rotateInDownLeft
* rotateInDownRight
* rotateInUpLeft
* rotateInUpRight
* rotateOut
* rotateOutDownLeft
* rotateOutDownRight
* rotateOutUpLeft
* rotateOutUpRight
* hinge
* rollIn
* rollOut
* zoomIn
* zoomInDown
* zoomInLeft
* zoomInRight
* zoomInUp
* zoomOut
* zoomOutDown
* zoomOutLeft
* zoomOutRight
* zoomOutUp
* slideInDown
* slideInLeft
* slideInRight
* slideInUp
* slideOutDown
* slideOutLeft
* slideOutRight
* slideOutUp
