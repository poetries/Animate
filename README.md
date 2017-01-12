Animate
---
animate.js is a simple library that helps you write smooth motion effects


Usage
---

- Include animate.min.js in your page:

```javascript
<script src=animate.min.js></script>
```

or 

```
<script src="http://7xq6al.com1.z0.glb.clouddn.com/Animate.min.js"></script>
```

- Take Animate for example

animateTime version usage method:

```javascript
animateTime(obj,json,callback);
```

example:

```javascript
animateSpeed(obj,{
	"left":500,
	"width":200,
	"height":300,
	"opacity":100
},function(){ //callback
	this.innerHTML = "我是速度版本";
});
```

animateSpeed version usage method:

```javascript
animateSpeed(obj,json,time,prop,callback);
```

example:

```javascript
animateTime(obj,{
	"left":500,
	"opacity":100
},1000,"elasticOut",function(){ //callback
	this.innerHTML = "我是时间版本";
});
```

animatable properties
---

- obj 要运动的元素对象
- json 传入多个属性
- time 需要动画变换的时间
- callback 回调函数
- prop 运动的特效函数
  - linear 匀速
  - easeIn 加速曲线
  - easeOut 减速曲线
  - easeBoth 加加速曲线
  - easeInStrong 减减速曲线
  - easeOutStrong 加加速减减速曲线
  - elasticIn 正弦衰减曲线 (弹动渐入)
  - elasticOut 正弦增强曲线 (弹动渐出)
  - elasticBoth
  - backIn 回退加速 (回退渐入)
  - backOut 回缩的距离
  - backBoth
  - bounceIn 弹球减振（弹球渐出）
  - bounceOut 
  - bounceBoth


Demo and Application examp
---

- [demo](http://codepen.io/poetries/pen/dNMRoQ)
- [运用速度版animateSpeed实现banner轮播](http://codepen.io/poetries/pen/ZLWyWJ)


License
---

© 2017 A [poetries's](http://blog.poetries.top) [ideas](https://github.com/poetries/ideas).	