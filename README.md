# 抖音续火助手

运行于抖音网页版私信页的油猴用户脚本。支持选择会话、预览文案、定时发送，以及手动重试当天发送失败的会话。

## 安装和使用

1. 安装 Tampermonkey 或 ScriptCat，并允许其在抖音运行用户脚本。
2. [安装脚本](https://raw.githubusercontent.com/c2451134117-cyber/douyin-fire-helper/main/douyin-fire-helper.user.js)，然后刷新[抖音聊天页](https://www.douyin.com/chat)。
3. 在续火助手面板中点 **用户选择** 设置目标会话。在 **偏好设置** 中配置发送时间和文案。
4. 用 **消息预览** 核对文案。定时发送需要聊天页保持打开、账号保持登录。

如需按星期发送 `[auto-response]Monday` 这样的文案，在 **专属一言** 中为每天填写对应的英文星期名和前缀，将 **自定义消息模板** 设为 `[专属一言]`，并关闭一言 API 和 TXTAPI。

## 本版修改

- 专属一言按填写的原文输出，去掉自动添加的「周几专属」前缀。
- 打开搜索结果中的目标会话后，核对会话标题再输入消息。
- 单个会话失败时继续处理其他会话。再次点击 **立即发送** 可以重试当天失败的会话，已成功发送的会话会被跳过。

## 来源与许可

本仓库基于 [dr-190/ScriptCat-Douyin-Fire-Helper](https://github.com/dr-190/ScriptCat-Douyin-Fire-Helper)，保留原脚本署名及上游 [MIT 许可证](LICENSE)和[版权声明](NOTICE)。
