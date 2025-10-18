# git-demo

一个练习git操作的demo仓库。


## Why

一个练习git操作的demo仓库，如提交、回退、分支合并等进阶操作。


## Where

文件按年归档，文件名使用年月（yyyyMM）进行命名，后缀统一为.md
统一按照一下格式添加YAML Front Matter
```yaml
title: yyyyMM
date: yyyy-MM-dd HH:mm:ss
```
其中yyyyMM为一级标题，yyyyMMdd作为二级标题，二级标题简介内容“yyyy-MM-dd 新增/变更内容如下。”


## How

### 变更内容

尽量使用文本文件，主要使用歌词作为变更内容。
示例
> 一条小路，悠悠青山，山花暗自香。
> 
> 当日日期，如 2025-10-18
> 摘自
>《别来无恙》
> 卡奇社
> 该内容可能受版权保护。

### 分支管理

- main 不做commit，只接受tag，develop分支基于main分支创建。
- develop
- feature 特性开发，基于develop分支创建；开发完成后代码合并到develop（使用squash选项进行压缩）并删除feature分支。
- release 基于develop分支创建，可在该分支上进行测试和bug修复，发布之后删除release分支。
- hotfix 基于main分支创建，开发完成后需合并回main分支和develop分支，同时在main分支打上tag。

参考文档 [gitflow 规范指南](https://www.cnblogs.com/kevin-ying/p/14329768.html)


## gitmoji 参考

参考地址 [gitmoji.dev](https://gitmoji.dev)

提交时使用 gitmoji
- :bug: Fix a bug.
- :fire: Remove code or files.
- :bug: Fix a bug.
- :ambulance: Fix a critical hotfix.
- :sparkles: Introduce new features.
- :memo: Add or update documentation.
- :lipstick: Add or update the UI and style files.
- :tada: Begin a project.
- :bookmark: Release / Version tags.
- :recycle: Refactor code.
- :coffin: Remove dead code.
- :necktie: Add or update business logic.
