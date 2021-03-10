---
tags: JavaScript
---

# for 迴圈 沒有用 let 或 var 宣告變數

## 前言
* 常看到 for 迴圈，沒有用 let 或 var 宣告變數，可以使用，所以研究一下這三種情況有甚麼差別?
1. `for (i = 1; i <= 10; i++)`
2. `for (var j = 1; j <= 10; j++)`
3. `for (let k = 1; k <= 10; k++)`

### 結論懶人包: 
* 不建議沒有用 let 或 var 宣告變數，可以會因為可以被刪除，而造成程式 Bug。

### 範例程式碼
```javascript=
for (i = 1; i <= 10; i++) {
  console.log(i); // 1, 2, 3, 4, 5, 6, 7, 8, 9, 10
}
console.log(i); // 1, 2, 3, 4, 5, 6, 7, 8, 9, 10
delete i;
console.log(i); // i is not defined

for (var j = 1; j <= 10; j++) {
  console.log(j); // 1, 2, 3, 4, 5, 6, 7, 8, 9, 10
}
console.log(j); // 11
delete j;
console.log(j); // 11

for (let k = 1; k <= 10; k++) {
  console.log(k); // 1, 2, 3, 4, 5, 6, 7, 8, 9, 10
}
console.log(k); // k is not defined
delete k;
console.log(k); // k is not defined

```


## 沒有用 let 或 var 可以被刪除
### 範例程式碼
```javascript=
var a = 'a';
delete a; // false

b = 'b';
delete b; // ture
```

## 心得
![](https://i.imgur.com/5T0Z2eW.png =300x)


## reference
* [淺談 var 與 let 的差異以及有無宣告變數的差異 -Ray](https://hsiangfeng.github.io/javascript/20200425/539985371/)
* [delete 操作符 -MDN](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Operators/delete)
* [Loops and iteration -MDN](https://developer.mozilla.org/zh-TW/docs/Web/JavaScript/Guide/Loops_and_iteration)