# ChatGPT_python
Open AI ChatGPT流式输出。Open AI Stream output. ChatGPT Stream output.

此项目只是对chatgpt-python 的一个简单示例项目，实现流式输出，仅做参考。有提升建议的可以私聊

交流群：
![image](https://github.com/shudongW/ChatGPT_python/blob/main/Screenshots/chat.png)
满了加微信：
![image](https://github.com/shudongW/ChatGPT_python/blob/main/Screenshots/me.png)
## SSE
主要是基于SSE（Server-Send Events） 实现的。也是最近在了解到SSE。
OpenAI官网在接受Completions接口的时候，有提到过这个技术。 Completion对象本身有一个stream属性，当stream为true时候Api的Response返回就会变成Http长链接
https://platform.openai.com/docs/api-reference/completions/create

https://developer.mozilla.org/en-US/docs/Web/API/Server-sent_events/Using_server-sent_events#event_stream_format

## Setup
依赖
```bash
   $ pip install -r requirements.txt
   ```
部署
```bash
   $ cd openai-quickstart-python
   ```
修改配置
```bash
   $ vi app.py
   $ openai.api_key = 'sk-*******************'
   $ 改为你的api_key
   $ cd upload/
   $ vi channelBob.html  sendMsg.html
   $ 修改 http://localhost 为你的真是服务器ip地址
   ```
运行
```bash
   $ python app.py
   $ 客户端访问：ip:5100/ 会自动跳转sendMsg.html
   $ 再打开ip:5100/upload/channelBob.html
   $ sendMsg.html中参数channel=channel_bob, msg=XXXXX
   $ 观察channelBob.html
   ```
