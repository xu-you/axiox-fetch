# Axiox 与 Fetch

## 一、Axios
#### 1.axios是什么
axios是一个基于 promise 的 HTTP 库，可以用在浏览器和 node.js 中。
#### 2.axios使用
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
