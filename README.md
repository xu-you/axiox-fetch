# 简单介绍 Axiox 与 Fetch

## 一、Axios
#### 1.axios是什么
axios是一个基于 promise（关于promise不明白的小伙伴可以看一下 [阮一峰老师的教学](http://es6.ruanyifeng.com/#docs/promise)或[这篇文章](https://www.talkingcoder.com/article/6336155176377712832)来学习） 的 HTTP 库，可以用在浏览器和 node.js 中。

#### 2.axios 的主要特性包括：
*  基于 Promise （所谓 Promise，就是一个对象，用来传递异步操作的消息）
*  支持浏览器和 node.js
*  可添加拦截器和转换请求和响应数据
*  请求可以取消
*  自动转换 JSON 数据
*  客户端支持防范 XSRF
*  支持各主流浏览器及 IE8+

#### 3.axios使用
###### Get 方式:
```javascript
axios.get(url,{
  params:{
    username: "金星老师"
  }
})
.then(function (res) {
  console.log(res.data);
})
.catch(function (error) {
  console.log(error);
})
```
###### Post 方式:
```javascript
axios.post(url,{
  name: this.username,
  password: this.password
},{
  "headers": {"Content-Type": "application/x-www-form-urlencodeed"}
}).then(function(res){
  console.log(res.data);
})
.catch(function (error) {
  console.log(error);
})
```

<br />

## 二、Fetch
#### 1.fetch是什么
fetch是一种XMLHttpRequest对象来获取后台的数据之外的一种更优的解决方案。

#### 2.fetch的特性:
fetch方法返回一个Promise对象, 根据 Promise Api 的特性, fetch可以方便地使用then方法将各个处理逻辑串起来, 使用 Promise.resolve() 或 Promise.reject() 方法将分别返会肯定结果的Promise或否定结果的Promise, 从而调用下一个then 或者 catch. 一但then中的语句出现错误, 也将跳到catch中.
