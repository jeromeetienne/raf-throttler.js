# raf-throttler.js

raf-throttler.js is a micro library to throttle and instrument [requestAnimationFrame](https://developer.mozilla.org/en-US/docs/Web/API/window/requestAnimationFrame).
It has been written to help debugging, as part 
of [three.js inspector chrome devtools extension](https://github.com/jeromeetienne/threejs-inspector).
You can throttle the rate to see how your animation is reacting.
Perfect debug tool if you wanna see what your game looks like at 20fps!

The code is simple, you likely could have coded that yourself. It is published
so hopefully you dont have to :)

Show Don't Tell
===============
* [examples/basic.html](http://jeromeetienne.github.io/raf-throttler.js/examples/basic.html)
\[[view source](https://github.com/jeromeetienne/raf-throttler.js/blob/master/examples/basic.html)\] :
It shows a basic usage of rafHijacker.js .

### Examples usage

First let's throttle requestAnimationFrame at 10 fps

```
var rafHijacker	= new RafHijacker()
rafHijacker.fps = 10
```

Now we gonna disable throttling

```
rafHijacker.fps = -1
```

And at the end, restore the original requestAnimationFrame function

```
rafHijacker.restore()
```

### TODO
- to rename raf-throttler.js ?
