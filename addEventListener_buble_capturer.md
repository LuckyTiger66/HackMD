# addEventListener() buble & capture 冒泡與捕獲

[![hackmd-github-sync-badge](https://hackmd.io/5464SsS9ROufePrYDkZyng/badge)](https://hackmd.io/5464SsS9ROufePrYDkZyng)

###### tags: `JavaScript`

![](https://i.imgur.com/sL9QhWW.jpg)
@karine_photo_64
## 前言
使用 addEventListener()，有時候發現執行了兩次或不是想要的效果，到底是出了甚麼問題?
有可能就是 event 冒泡或捕獲產生的問題。

## event 是甚麼?
空白網頁中，在開發者模式 console 中輸入以下程式碼，然後點擊網頁，就可以找出 event
```javascript=
document.addEventListener('click', function(e){
  console.log(e);
}, false);
```
![](https://i.imgur.com/qgANRgz.png)

## 範例
* https://codepen.io/LuckyTiger/pen/ExZQqLJ
<a href="https://codepen.io/LuckyTiger/pen/ExZQqLJ" target="_blank" style="text-decoration:none">![](https://i.imgur.com/UX3DQ7r.png)</a>

## reference
* [EventTarget.addEventListener() -MDN](https://developer.mozilla.org/en-US/docs/Web/API/EventTarget/addEventListener)
* [HTML DOM addEventListener() 方法 -Runoob](https://www.runoob.com/jsref/met-element-addeventlistener.html)
* [重新認識 JavaScript: Day 15 隱藏在 "事件" 之中的秘密 -Kuro](https://ithelp.ithome.com.tw/articles/10192015)