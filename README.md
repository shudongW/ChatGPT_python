# ChatGPT_python
Open AI ChatGPT流式输出。Open AI Stream output. ChatGPT Stream output.

此项目只是对chatgpt-python 的一个简单示例项目，实现流式输出，仅做参考。有提升建议的可以私聊

交流群：

满了加微信：


主要是基于SSE（Server-Send Events） 实现的。也是最近在了解到SSE。
OpenAI官网在接受Completions接口的时候，有提到过这个技术。 Completion对象本身有一个stream属性，当stream为true时候Api的Response返回就会变成Http长链接
https://platform.openai.com/docs/api-reference/completions/create
https://developer.mozilla.org/en-US/docs/Web/API/Server-sent_events/Using_server-sent_events#event_stream_format

依赖

部署

修改配置

运行
