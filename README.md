index.py与index.wsgi文件内容相同
wechat.py 本地测试tornado异步，测试通过
2017/11/20
问题：
SAE云应用使用tornado异步
函数运行到resp = yield client.fetch(url)报错
无法异步向微信客户端发请求导致功能丢失
解决：
1.在SAE云应用中如何使用tornado异步客户端发请求
2.不使用异步直接阻塞，等请求完成再继续执行（效率低下）