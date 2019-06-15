## promise
> 目的是为了解决嵌套地狱的问题
1. Promise是一个构造函数
2. 怎么是使用构造函数
   ```javascript
   var promise = new Promise() // 通过new 操作符创建一个promise实例对象
   ```
3. `new Promise(函数)`函数有2个参数一个是resolve(成功的回调函数)一个reject(失败的回调函数)
    ```javascript
    var promise = new Promise(function (resolve, reject) {})
    ```
4. 在promise的原型上有2个方法分别是then和catch
   - `.then(成功的回调, 失败的回调)`
   - `.catch(失败的回调)`如果发生了异常都会进入到catch中

## fetch请求库
- `fetch(url, {}).then((res) => {return res.json()}.then(res => {//res}))`
- 如果想post请求怎么办呢？ 百度
- 在fetch中默认是不带cookie的，如果需要带上cookie需要设置credentials: 'include'