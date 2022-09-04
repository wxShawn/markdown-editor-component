# Markdown editor component
## 介绍
这是一个基于 vue.js 和 marked.js 开发的 markdown 编辑器组件。
## 截图
![组件截图](https://raw.githubusercontent.com/wxShawn/media-lib/main/images/markdown-editor-sc.png)
## 使用
1. 将`MarkdownEditor`文件夹以及里面的文件复制到自己的项目中。
2. 下载相关依赖：
```json
"dependencies": {
  "github-markdown-css": "^5.1.0",
  "highlight.js": "^11.6.0",
  "marked": "^4.0.18",
  "vue": "^3.2.37"
}
```
3. 引入组件：
```js
import MarkdownEditor from "./components/MarkdownEditor";
```
## API
### props
|名称|类型|说明|
|:-:|:-:|:-:|
|content|string|编辑器的文本内容|
### events
|名称|事件上传值|说明|
|:-:|:-:|:-:|
|dataChange|data: { title, md, html }|编辑器的文本内容改变时触发|