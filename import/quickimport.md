# 🚀 快捷导入

## 从电脑导入

在将 Kindle 阅读器上的笔记导入到手机中，通常需要费时费力地将 MyClipping.txt 文件从电脑端复制到手机端。然而，使用纸间书摘应用中的**从电脑导入**功能，可以轻松解决这个繁琐的问题。纸间书摘内置了一个文件传输服务，在局域网络下，可直接将文件发送到手机。**从电脑导入**功能支持导入来自 **Kindle 阅读器**、**豆瓣阅读**和 **Apple Books** 的笔记。

>💡 要使用纸间书摘中的「从电脑导入」功能，需要满足一个前置条件：**手机和电脑必须在同一个局域网环境中，并且可以相互通信。**

![从电脑导入](https://doc-1252413502.cos.ap-nanjing.myqcloud.com/Xnip2022-01-03_13-44-52.png)

1. 文件服务器启动状态。
2. 内置服务器的访问地址。

你可以在上图中标记 2 的位置查看服务访问的地址。接下来，你可以通过浏览器打开上述网址来执行笔记导入的操作。下图展示了详细的操作流程。

![浏览器上的操作](https://doc-1252413502.cos.ap-nanjing.myqcloud.com/Xnip2022-01-03_13-58-49.png)

1. 在浏览器地址栏输入服务器地址。
2. 拖拽笔记文件至虚线区域。
3. 点击上传。
4. 当浏览器页面中显示**上传成功**的弹窗后纸间书摘将开始解析笔记，请回到手机上继续操作。

若笔记成功解析你将看到如下界面，否则你会在手机上看到有关导入失败的原因提示。

![选择要导入的内容](https://doc-1252413502.cos.ap-nanjing.myqcloud.com/Xnip2022-01-03_14-11-41.png)

选择好要导入的内容后点击**导入**即可完成笔记的导入。

> 👀 电脑端上传文件目前只支持单文件上传，但对于一些笔记的导入我们也支持批量。以 Koodo Reader 的 CSV 文件为例，您可以先将多个需要导入的 CSV 文件打包成一个 .zip 压缩文件，然后上传。纸间会自动解压缩并完成所有笔记的导入操作。需要注意的是，批量导入功能目前仅适用于 Koodo Reader 的 CSV 文件。

> 关于 MyClipping.txt 文件、豆瓣阅读笔记文件、Apple Books、Koodo Reader 笔记文件的获取方式我们将在本手册的相关章节中提到。

## 从「微信读书」授权导入

纸间书摘支持将微信读书中的所有书籍笔记批量导入到应用中。用户可以通过**授权导入**的方式，一次性将微信读书中所有书籍的笔记导入到纸间书摘中。这种方式不仅可以导入书籍的阅读状态，而且还能保证导入内容的数据完整性，并且相较于使用剪贴板导入，可以获得更高的导入效率。下图所示的步骤将指导用户如何实现微信读书的批量导入。

> 💡 在导入时，只会导入已包含摘录的书籍，并不会一并导入您微信读书中的所有书籍。

> ⚠️  在开始导入前，请确保微信读书中的「替身书架」已关闭。若替身书架处于开启状态，导入时将无法获取书籍的阅读状态及阅读时长。为确保完整导入，建议关闭「替身书架」后再执行导入操作。

> ⚠️  对于本地导入的书籍，支持导入书籍的笔记想法和阅读时长，**但无法获取到书籍的阅读状态**（无法自动帮您标记已读完的书籍）。

![微信读书授权导入流程](https://doc-1252413502.cos.ap-nanjing.myqcloud.com/%E5%BE%AE%E4%BF%A1%E8%AF%BB%E4%B9%A6%E6%8E%88%E6%9D%83%E5%AF%BC%E5%85%A5.png)

1. 点击「微信读书授权导入」进入功能。
2. 点击「保存二维码」，将二维码保存到本地相册。
3. **打开微信，扫描上一步保存的二维码**，进入微信读书网页版登陆授权界面，点击登录（注意：在打开微信扫码时不要关闭「书摘导入」界面，只需将纸间书摘切回后台即可）。
4. 切换回纸间书摘。
5. 若弹出上图中的对话框则表示授权成功，正在获取微信读书中的笔记。

> 💡 微信读书的登录二维码存在过期时间。在将二维码保存到本地后，应尽快完成扫码授权的操作。

扫码成功后会看到上图所示步骤 3 所在的页面。当点击登录若显示登录成功，返回纸间书摘即可看到步骤 3 所示的弹窗。如果显示登录失败，请返回纸间书摘刷新二维码后重新执行上述的流程。

> 💡 在网络不稳定的情况下可能会出现即便显示登陆成功，但回到 纸间书摘 却没有显示步骤 3 的弹窗，遇到此问题时请多尝试几次或更换设备。
> 如果你使用的是鸿蒙系统的设备，也有出现上述问题的可能。你可以通过小窗打开微信（让 纸间书摘 保持在前台可见）进行扫码，这样能提高导入的成功率。