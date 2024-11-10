# 💄 导出到「思源」

## [思源笔记](https://b3log.org/siyuan/)

思源笔记是一款隐私优先的个人知识管理系统，支持完全离线使用，同时也支持端到端加密同步。融合块、大纲和双向链接，重构你的思维。

## 操作说明

> 1. 在开始导出前请确保<mark style="background-color:yello;">**手机与电脑处在同一个局域网下**</mark>（思源笔记的 API 导出是基于本地的局域网环境）。
> 2. 确保<mark style="background-color:yello;">**电脑端已经启动了思源笔记，并且设置中的「网络伺服」功能已开启**</mark>（路径：SiYuan/关于/网络伺服）。

## 获取配置参数

### 1. 获取网络地址、端口号。

1. 打开思源设置界面。点击顶部的「SiYuan」，之后在弹出的菜单中点击「设置」。
![开启设置界面](https://doc-1252413502.cos.ap-nanjing.myqcloud.com/%E6%88%AA%E5%B1%8F2023-07-01%2015.30.04.png)

2. 在开启的设置界面中点击「关于」。以下图设置为例，网络地址为：192.168.0.109。端口号为：6806。
![关于](https://doc-1252413502.cos.ap-nanjing.myqcloud.com/%E6%88%AA%E5%B1%8F2023-07-01%2015.38.41.png)

### 2. 获取 API token。

1. 开启访问授权码

    ![开启访问授权码](https://doc-1252413502.cos.ap-nanjing.myqcloud.com/SCR-20241110-nzfb.png) 
    
    点击「设置」来启用访问授权码。⚠️ 访问授权码是必须的，如果不开启您将无法访问到思源的伺服服务。

2. 获取 API token

    以下图为例，API token 的值为：67b502cs7vya1m2s
    ![API token](https://doc-1252413502.cos.ap-nanjing.myqcloud.com/%E6%88%AA%E5%B1%8F2023-07-01%2015.57.11.png)

    将获取到的 <mark style="background-color:yellow;">**网络地址、端口号、API token**</mark> 依次填写到纸间书摘即可完成导出前的配置工作。
