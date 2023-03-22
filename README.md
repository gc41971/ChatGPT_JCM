# Multi Model ChatGPT Web
声明：此项目只发布于 Github，基于 Apache2.0 协议，免费且作为开源学习使用。并且不会有任何形式的卖号、付费服务、卖key等行为。谨防受骗。
项目使用Vue2进行开发，给大家提供一个好看的GPT壳子，有好的建议和bug欢迎大家提出来，星星超过1000个随机抽10个群聊活跃的用户送独有的openai key。

## 模型
![webui4.5](https://i.328888.xyz/2023/03/22/1wH85.jpeg)
## 会话
![webui4.5](https://i.328888.xyz/2023/03/22/1wbqZ.jpeg)
## 微调模型列表
![webui4.5](https://i.328888.xyz/2023/03/22/1wpyX.jpeg)
> 🤭记得点个小星星

# 部署步骤
## 参考视频
https://www.bilibili.com/video/BV1iL411k7pC  本地和云服务器部署视频


## 下载依赖包
```
npm install
```

## 运行
```
npm run serve
```

## 编译
```
npm run build
```

## 设置自动读取APIKEY
在.env.serve中添加代码
```
VUE_APP_OPENAI_API_KEY='你的openai api key'
```


# 技术栈

|  名称   | 版本  |
|  ----  | ----  |
| vue  | 2.6.14 |
| element-ui  | 2.15.12 |
| NodeJS  | 14.21.3 |
| npm  | 6.14.18 |

# 项目进度

|  接口   | 描述  |
|  ----  | ----  |
| List Models  | 获取模型列表 |
| Chat Completion  | GPT3.5模型 |
| Completion  | GPT3.5以下模型 |
| Create Image  | 根据描述生成图片 |
| Create image edit  | 根据上传的图片结合输入的描述生成图片 |
| Create Image Variation  | 根据上传的图片生成变体图片 |
| Create transcription  | 音频识别文字 |
| Create translation    | 英语音频识别 |
| fine-tune    | 待开发 |
| Files    | 待开发 |
| 多会话储存和上下文逻辑    | GPT3.5模型支持上下文逻辑,多窗口上下文对话 |
| 聊天截图到本地图片    | 截图功能，有缺陷只能截图当前窗口的图片，建议QQ长截图 |
| 导出导入数据   | 待开发 |
| 更换聊天窗口背景    | 支持输入背景图片URL |
| 更换主题    | 待开发 |
| 界面多语言    | 待开发 |
| More    | 待开发 |

# Docker部署

## 构建镜像
使用以下命令构建镜像，其中 "jcm-chatgpt" 是您想要给镜像取的名称，"." 表示 Dockerfile 在当前目录中。
```
docker build -t jcm-chatgpt .
```
## 运行镜像
构建完成后，可以使用以下命令运行镜像，其中 "my-container" 是您想要给容器取的名称。该命令会将容器端口 80 映射到本地机器的端口 80。
```
docker run --name my-chatgpt -p 80:80 jcm-chatgpt
```
# 免责声明
这不是官方的OpenAI产品。这是一个个人项目，与OpenAI没有任何关系。不要起诉我。
