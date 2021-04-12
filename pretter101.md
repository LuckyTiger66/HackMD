# Prettier 程式碼格式統一

[![hackmd-github-sync-badge](https://hackmd.io/kbB8yNVOQEC_iL7MKO_3CQ/badge)](https://hackmd.io/kbB8yNVOQEC_iL7MKO_3CQ)

###### tags: `Visual Studio Code`

## 為什麼要使用 
### 統一程式碼規則
* tab 空白幾格 
* "" 還是 ''
* {} [] 和數字跟字串的空白
## 如何使用
![](https://i.imgur.com/QdbT6Ca.png)
* Format Document 統一整份文件格式
* Format Selection 統一選取部分的文件格式

## 設定
```javascript=
在 vscode 中 
(Ctrl + , ) //搜尋 Prettier 
```
![](https://i.imgur.com/wknChIB.png)

## 遇到的問題
### 1. 引號消失
```htmlmixed=
Q: 本來物件與陣列裡面的引號，統一後消失
A: 設定 Quote Props 屬性的引號
預設值："as-needed" 只必要加上引號的屬性才會有引號。
改成 quoteProps: "preserve" 不格式化，依使用者的使用。
```
### 慣用單引號，預設值是雙引號
* 勾選起來，預設是沒有勾

![](https://i.imgur.com/bUKEXcT.png)

## reference
* [prettier 官網文件](https://prettier.io/docs/en/options.html)
* [在 vscode 裡面採用 Prettier 做程式碼格式統一的設定 -CloverHsc](http://cloverhsc.blogspot.com/2019/09/vscode-prettier.html)
* [Prettier - Code formatter -竹白](https://hackmd.io/@chupai/HkNT0IMhr)
* [英文引號用法：‘單引號’和“雙引號”的正確使用方法](https://www.editing.tw/blog/%E8%8B%B1%E6%96%87%E5%BC%95%E8%99%9F%E7%94%A8%E6%B3%95-%E5%96%AE%E5%BC%95%E8%99%9F%E5%92%8C%E9%9B%99%E5%BC%95%E8%99%9F%E7%9A%84%E6%AD%A3%E7%A2%BA%E4%BD%BF%E7%94%A8%E6%96%B9%E6%B3%95.html)

