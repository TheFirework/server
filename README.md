# Setup 1
```bash
git clone git@github.com:TheFirework/server.git
```

# Setup 2
```bash
cd server && npm install
```
或者
```bash
cd server && yarn
```

# setup 3
```bash
yarn start
```
或者
```bash
npm run start
```
# setup 4
打开mock.js编写模拟接口

```js
import example from './mock/example';//导入其他接口

export default {
  //支持POST GET DELETE PUT 等方法
  //格式为 请求方式+空格+请求地址
  "POST /exampleApi" : (req, res) => {
    console.log(req.body)
    res.send({
      status : "OK",
      code : 200,
      data : ""
    })
  },
  ...example
}
```

## 选项
- 更改启动端口号(默认3000)
```bash
yarn start 端口号
```


