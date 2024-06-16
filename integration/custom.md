# 😼 模板自定义

纸间为发送到关联应用的笔记提供了默认模板。如果这些默认模板不满足您的需求，您可以自定义笔记样式：在纸间书摘中，我们提供了一个模板引擎（[freemarker](https://freemarker.apache.org/index.html)），允许您通过编写自己的模板代码来个性化您的笔记导出样式。

> 🐱 想要学习如何编写模板，您可以参考以下 FreeMark 的文档。这可能需要一定的编程知识。如果您遇到困难，欢迎联系开发者，微信号：scarecrow0x18

> 文档地址：https://freemarker.apache.org/docs/index.html

在使用纸间书摘自定义笔记样式时，请利用提供的模板变量编写模板。您可以点击「运行」测试模板，并在下方文本框查看结果，以确认模板是否正确编写。若要检查模板效果，可使用「发送至」功能将笔记发送至关联应用。确保模板正确无误后，请点击「保存」以确保将来发送时应用新模板。如需恢复默认模板，选择「恢复默认」。

![](https://doc-1252413502.cos.ap-nanjing.myqcloud.com/WX20240128-180814%402x.png)

##  模板示例<!-- {docsify-ignore} -->

下面单独为 flomo、writeathon、inbox 编写了一份模板示例，相较于纸间书摘中默认提供的模板，以下模板添加了对「阅读位置」、「章节」的支持。您可以将这些模板直接复制粘贴到纸间书摘的「模板自定义」功能中以启用。

## flomo
```
<#if note?length gt 0 >
${note}

</#if>
<#if idea?length gt 0 >
想法：
${idea}

</#if>
<#if images?size gt 0 >
图片：
<#list images as image >
${image}
</#list>

</#if>
<#if chapter?length gt 0 >
章节：${chapter}
</#if>
<#if pageNumber?length gt 0 >
位置：${pageNumber}
</#if>
<#if tags?size gt 0 >
#${appName}/${bookTitle}<#list tags as tag>/${tag}</#list>
<#else>
#${appName}/${bookTitle}
</#if>
```
## writeathon
```
<#if note?length gt 0 >
${note}

</#if>
<#if idea?length gt 0 >
<#list idea?split("\n") as section>
> ${section}
</#list>

</#if>
<#if images?size gt 0>
<#list images as image>
![](${image})
</#list>

</#if>
<#if chapter?length gt 0 >
章节：${chapter}
</#if>
<#if pageNumber?length gt 0 >
位置：${pageNumber}
</#if>
<#if tags?size gt 0>
#${appName}/${bookTitle}<#list tags as tag>/${tag}</#list>
<#else>
#${appName}/${bookTitle}
</#if>
```
## inBox
```
<#if note?length gt 0 >
${note}

</#if>
<#if idea?length gt 0 >
想法：
${idea}

</#if>
<#if images?size gt 0 >
图片：
<#list images as image >
![](${image})
</#list>

</#if>
<#if chapter?length gt 0 >
章节：${chapter}
</#if>
<#if pageNumber?length gt 0 >
位置：${pageNumber}
</#if>
<#if tags?size gt 0 >
#${appName}/${bookTitle}<#list tags as tag>/${tag}</#list>
<#else>
#${appName}/${bookTitle}
</#if>
```
> 🐱 想了解更多关于模板编写的信息，请参考 [freemarker](https://freemarker.apache.org/docs/index.html) 。我们鼓励您尝试自行编写模板，这将带来极大的成就感。当然，如果您需要帮助，我们很乐意协助您编写所需模板。请联系开发者（微信：scarecrow0x18）🆓 🆓 🆓。
