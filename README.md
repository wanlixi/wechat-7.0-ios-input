# wechat-7.0-ios-input
ios手机，在微信7.0版本的bug
```
// 兼容ios 微信7.0以上版本页面被顶上去下不来的问题
let timer = setInterval(() => {
  if (['showPlacePhone', 'showPlaceVeri', 'showPlacePic'].every(item => this.state[item])) {
    window.scrollTo(0, 0)
    clearInterval(timer)
  }
}, 200)
```
