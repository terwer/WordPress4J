# wordpress4j

WordPress on Java platform. 100% compatible with the latest WordPress version on Java and SpringBoot platform.

## 技术构想

WordPress在Java平台的实现。前后端完全分离，后端只提供核心API和实现，UI和插件、主题等完全由前端完成。

100%兼容最新版WordPress标准，纯Java实现，后端API和核心支持基于SpringBoot技术体系。

前端采用Nuxt2，插件和技术体系基于Vue和Nuxt2技术体系，请参考 [jvue-front-2](https://github.com/terwer/jvue-front-2)。

## 说一说为为什么这么选型的原因

Q：为什么不继续使用WordPress，要重新实现？

A：

WordPress是一个历史悠久，质量卓越受人尊敬的项目，有良好的插件体系和生态。

但是它至少有以下几点是我觉得不太好的地方

1、基于PHP，代码与界面混杂在一起，维护起来可读性很差，这也是我最不能忍受的。有人会反驳我，说这样写起来方便，但是我想说的是，方便的同时带来的是维护起来的噩梦。

2、整个WordPress项目的前端几乎没有什么架构，只是纯js的实现。

随着es6标准的发布，TypeScript的兴起与Vue、React技术的成熟，大前端规范化UI体系已经成熟，所以前端完全独立会让代码可读性大大增强，再加上ts的业务能力，前端写复杂插件、主题已经非常容易，纯js的弊端已经可以解决，而且比起后端有太多优势。

Q：为什么不使用SpringBoot模板引擎，例如freemarker，thymeleaf等，而选择完全独立的前端体系？

这个在上面第二点已经阐述。使用模板引擎就又将后端代码与UI冗杂在一起，失去了本项目的初衷。
