# 🌋 导出到 Obsidian

### [Obsidian](https://obsidian.md)

Obsidian 是一个基于 Markdown 文件的闭源笔记软件。用户可以在笔记的不同页面中建立内部链接，然后以图的形式将这些连接可视化。它旨在帮助用户以一种灵活的、非线性的方式组织和架构他们的想法和知识。Obsidian 对个人使用免费，商业许可需要付费使用。作家、研究人员、学者和其他需要灵活而强大的笔记工具的专业人士中Obsidian很流行。(摘自：[维基百科](https://zh.wikipedia.org/zh-cn/Obsidian))

### 操作说明

> 纸间书摘向 Obsidian 导出笔记功能的实现基于 [Local REST API](https://github.com/coddingtonbear/obsidian-local-rest-api) 插件提供的伺服功能。因此在开始前，您需要先在 Obsidian 中安装 [Local REST API](https://github.com/coddingtonbear/obsidian-local-rest-api) 这款三方插件。（向 [Local REST API](https://github.com/coddingtonbear/obsidian-local-rest-api) 的开发者表示感谢～ 🍬）

#### 安装 Local REST API 插件

![安装插件-1](https://doc-1252413502.cos.ap-nanjing.myqcloud.com/Obsidian1.png)
![安装插件-2](https://doc-1252413502.cos.ap-nanjing.myqcloud.com/Obsidian2.png)
![安装插件-3](https://doc-1252413502.cos.ap-nanjing.myqcloud.com/Obsidian3.png)

#### 配置 Local REST API 插件

![配置插件-1](https://doc-1252413502.cos.ap-nanjing.myqcloud.com/Obsidian4.png)

在插件安装后，您需要在「第三方插件」中启动 Local REST API 插件。

![配置插件-2](https://doc-1252413502.cos.ap-nanjing.myqcloud.com/WX20230820-171107%402x.png)

1. 进入 Local REST API 的设置界面
2. 开启 Show advanced settings
3. 将 Binding Host 的值修改成：0.0.0.0

> ‼️ 请务必要将 Bining Host 从默认的 127.0.0.1 更改成 0.0.0.0，否则将无法正常完成笔记的导出。其它的设置请保持默认值，无需更改。

#### 纸间书摘中的操作说明

> 1. 在开始导出前请确保<mark style="background-color:yello;">**手机与电脑处在同一个局域网下**</mark>（Obsidian 的导出是基于本地的局域网环境）。
> 2. 确保<mark style="background-color:yello;">**电脑端已经启动了 Obsidian，并已按照上述步骤完成对 Local REST API 插件的安装与配置**</mark>。

![Obsidian配置](https://doc-1252413502.cos.ap-nanjing.myqcloud.com/WX20230820-173801%402x.png)

1. 配置网络地址，请将设备在局域网中的 IP 地址填写到红框所在位置。
2. 配置 API Key，请按照下图复制 API Key 填写到蓝框所在位置。

![APIKey](https://doc-1252413502.cos.ap-nanjing.myqcloud.com/WX20230820-174336%402x.png)

> 💡 我们支持将书籍标签同步导出到 Obsidian，如果您不想为文档关联标签，请关闭「添加标签」功能。

> 🐶 在点击「导出」后，将会弹出一个「选择文件夹」的弹窗。此处只会显示内容非空的文件夹（不知道 Local REST API 为什么要这么设计）。即便您不选择任何文件夹也是可以导出的，此时导出的文档将会存储在 Obsidian 的根目录下。