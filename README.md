# document使用说明

## 安装

```bash
# 全局安装gitbook
$ npm install gitbook -g

# 初始化，执行了install => build => serve （第一次使用）
$ npm run pbuild

# 本地测试 
$ npm run dev 

# 打包
$ npm run build
```

## 发布

需要配合gh-pages, 打包产生的_book目录会自动合并到gh-pages分支

```bash
# 全局安装gh-pages
$ npm install gh-pages -g
# 打包发布
$ npm run push
```

## 配置

/book.json

```json
{
  "title": "前端环境说明书", // 标题
  "description": "", // 描述
  // 使用的语言， 如 en, ar, bn, cs, de, en, es, fa, fi, fr, he, it, ja, ko, no, pl, pt, ro, ru, sv, uk, vi, zh-hans, zh-tw
  "language": "zh-hans",// 简体中文
  // 作者 
  "author": "busyhe",
  // 配置使用的插件
  "plugins": [
    
  ],
  // 自定义页面样式， 默认情况下各generator对应的css文件
  "styles": {
      "website": "styles/website.css",
      "ebook": "styles/ebook.css",
      "pdf": "styles/pdf.css",
      "mobi": "styles/mobi.css",
      "epub": "styles/epub.css"
  }
  "pluginsConfig": {
  }
}
``` 

## 目录结构

/SUMMARY

![](http://o7nwnvtc2.bkt.clouddn.com/15249034028135.jpg)

```
# Summary

### Part I

* [Introduction](README.md)
* [Writing is nice](part1/writing.md)
* [GitBook is nice](part1/gitbook.md)

### Part II

* [We love feedback](part2/feedback_please.md)
* [Better tools for authors](part2/better_tools.md)

----

* [Last part without title](part3/title.md)
```

## 词汇表

词汇表文件，默认对应的文件是 GLOSSARY.md。该文件主要存储词汇信息，如果在其他页面中出现了该文件中的词汇，鼠标放到词汇上会给出词汇示意，可以将鼠标移到下面两个词汇上看下效果。

/Glossary

```
## Git
分散式版本控制软件

## Markdown
Aaron Swartz 跟John Gruber共同设计的排版语言
```

## 参考

http://gitbook.zhangjikai.com/installation.html


