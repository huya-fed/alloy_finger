# alloy_finger 使用文档

---

超轻量级 Web 手势库

---

## 例子

[http://alloyteam.github.io/AlloyFinger/](http://alloyteam.github.io/AlloyFinger/)


## 使用说明



	var af = new AlloyFinger(element, {
	    touchStart: function () { },
	    touchMove: function () { },
	    touchEnd:  function () { },
	    touchCancel: function () { },
	    multipointStart: function () { },
	    multipointEnd: function () { },
	    tap: function () { },
	    doubleTap: function () { },
	    longTap: function () { },
	    singleTap: function () { },
	    rotate: function (evt) {
	        console.log(evt.angle);
	    },
	    pinch: function (evt) {
	        console.log(evt.zoom);
	    },
	    pressMove: function (evt) {
	        console.log(evt.deltaX);
	        console.log(evt.deltaY);
	    },
	    swipe: function (evt) {
	        console.log("swipe" + evt.direction);
	    }
	});
	
	/**
	 * this method can also add or remove the event handler
	 */
	var onTap = function() {};
	
	af.on('tap', onTap);
	af.on('touchStart', function() {});
	
	af.off('tap', onTap);
	
	/**
	 * this method can destroy the instance
	 */
	af = af.destroy();



## 官方的

[https://github.com/AlloyTeam/AlloyFinger](https://github.com/AlloyTeam/AlloyFinger)


