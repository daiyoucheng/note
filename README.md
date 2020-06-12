1.vue axios请求怎么获取 Response中的自定义headers
后端发送请求的时候设置：
// 自定义响应头
ctx.res.setHeader('myheader', 'abc')
// 通过此header设置允许前端访问
ctx.res.setHeader('Access-Control-Expose-Headers', 'myheader')
前端
response.headers['myheader']
