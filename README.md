---
title: DeepSite
emoji: 🐳
colorFrom: blue
colorTo: blue
sdk: docker
pinned: true
app_port: 5173
license: mit
short_description: Imagine and Share in 1-Click
---

Check out the configuration reference at https://huggingface.co/docs/hub/spaces-config-reference

将本项目移植到本地运行，运行方式：

下载源代码

git clone https://github.com/skywalk163/deepsite

进入目录deepsite

执行安装

npm install

执行build

npm run build

然后npm start就行了

npm start

注意需要修改server.js文件源代码，替换成自己的llm大模型url和key，当前设置的是
'''
const openai = new OpenAI({
  baseURL: 'http://192.168.1.5:1337/v1',
  apiKey: 'your-api-key', // 如果需要认证
});
'''