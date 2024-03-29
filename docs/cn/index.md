---
title: "主页"
description: "SpaceVim 是一个模块化的 Vim 和 Neovim 的配置集合，以模块的方式组织和管理插件，提高 Vim 环境配置效率。"
lang: zh
---

[![matrix](https://img.spacevim.org/spacevim-cn-matrix.svg)](https://app.element.io/#/room/#spacevim-cn:matrix.org)
[![Telegram](https://img.spacevim.org/telegram-spacevim-cn.svg)](https://t.me/SpaceVim_CN/)
[![twitter](https://img.spacevim.org/twitter.svg)](https://twitter.com/SpaceVim)
[![GPLv3 License](https://img.spacevim.org/license-GPLv3-blue.svg)](development/#证书)
[![reddit](https://img.spacevim.org/reddit.svg)](https://www.reddit.com/r/SpaceVim/)

![welcome page](https://img.spacevim.org/release-v2.2.0.png)

SpaceVim 是一个模块化的 Vim 和 Neovim 配置集合，它的灵感来自于 [spacemacs](https://www.spacemacs.org/)。
以模块的方式组织插件及相关配置，将相关插件组合在一起提供完整的功能。
这将使得插件配置更加简单，减少用户选择并配置插件的时间。
仅需载入相关语言的模块即可得到一个开箱即用的 Vim IDE。

- [入门指南](quick-start-guide/): 基本的安装以及配置示例，同时包括了针对不同语言的配置技巧。
- [使用文档](documentation/): 完整的使用文档，详细介绍了每一个快捷键以及配置的功能。
- [可用模块](layers/): 罗列了目前已经实现的所有模块，包括功能模块和语言模块。

当前最新的稳定版为[v2.2.0](https://spacevim.org/SpaceVim-release-v2.2.0/)，发布于2023年7月5日。
[following-HEAD](following-head/) 页面罗列了自 `v2.2.0` 至今最新的更新以及变动。若需要了解项目的后续开发路线及计划，可以查阅[开发路线](roadmap/)页面。

## 最新特性

<ul>
    {% for post in site.categories.feature_cn offset: 0 limit: 5  %}
               <strong><a href="{{ post.url }}">{{ post.title }}</a></strong>
               <br>
               <span class="post-date">{{ post.date | date_to_string }}</span>
               <p>{{ post.description | truncatewords: 100 }}</p>
               <br>
               <img alt="{{ post.title }}" src="{{ post.image }}">
    {% endfor %}
</ul>

更多精彩内容会定期在 SpaceVim [博客](blog/)上发布。

## 常见问题

- 目前 SpaceVim 的开发状态如何？

  当前最新发布的稳定版本是 v2.3.0。可以查看[Roadmap](roadmap/)获取开发计划。

- SpaceVim 是尝试搭建一个 IDE 吗？

  是的，通过模块的方式，将各种功能封装成相应的模块，对多种语言提供了语言开发模块，目标是尝试模拟简易的集成开发环境。

- SpaceVim 支持多少种编程语言？

  ```sh
  ~/.SpaceVim> ls autoload/SpaceVim/layers/lang | wc -l
  87
  ```

- SpaceVim 支持什么版本的 Vim/Neovim？

  SpaceVim 目前已通过 gh 测试了如下版本的 vim 和 neovim：

  - vim: `master`, `8.1.2269`, `8.0.1453`, `8.0.0027`,`7.4.1689`,`7.4.629`, `7.4.052`
  - neovim: `nightly`, `v0.5.0`, `v0.4.4`, `v0.4.3`, `v0.4.2`, `v0.4.0`, `v0.3.8`

更多常见问题请阅读[常见问题解答](faq/)

<!-- vim:set nowrap: -->
