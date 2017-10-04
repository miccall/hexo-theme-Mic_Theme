---
# Miccall Theme
###### version 1.1.0
---
![title](http://onh0umlhz.bkt.clouddn.com/0524themetitle.PNG)
## Contents 目录

- General 概括
- Demo 演示
- Quick start 快速开始
- Docs 文档
- Contributing 贡献
- License 许可证

## General概括

- 主题开发 套用了大量的[HTML5 UP][2] 模板 因为作者是前端小白 css功底菜鸡
在此鸣谢支持我的各位大佬

## Demo 演示
！[miccall.tech](http://miccall.tech)

![此处输入图片的描述](http://onh0umlhz.bkt.clouddn.com/0524theme002.PNG)

![此处输入图片的描述](http://onh0umlhz.bkt.clouddn.com/0524theme003.PNG)

![此处输入图片的描述](http://onh0umlhz.bkt.clouddn.com/0524theme004.PNG)

## Quick start 快速开始
- 安装 hexo
- 请仔细阅读 Hexo 的官方文档，完成对 Hexo 的安装和基本的配置 。
- 下载本主题 并且放置于themes目录下 更改主题名字 并在站点根目录的配置文件中启用该主题
- 在主题的配置文件中修改相应的值

## Docs 文档
以下内容均为主题的配置文件 " _config.yml " (请区别于站点的配置文件)

head:      
  favicon : 网站的logo
  high_res_favicon : 高清头像
  apple_touch_icon :   高清头像
  keywords : 关键字

 Intro: 主题刚开始加载的界面   
  name  :  名字
  slogan  :  第二标语
  HeadButton  :  主页按钮名字

 Nav: 导航栏  
  Home_name: 主页名字
  is_use_categories : 是否启用分类  (true false)
  categories_name: 分类名字
  is_use_archives : 是否启用归档  (true false)
  archives_name: 归档名字
  icon:  导航栏上的图标
     github:
      use: true   是否启用
      link: 点击地址
      Twitter:
            use: false
          link:
    Facebook:
    use: false
      link:
      Instagram:
       use: false
       link:
   pages:  自定义连接页
      简历:
        link: "/about/"  link 的参数为相对路径，对应 hexo 目录下的 source 件夹内的相应文件夹。
     团队 :
        link: "/group/"
  图库 :
         link: "/gallery/"
    标签:
      link: "/tag/"
            自定义标签名
            link：“路径”

使用方法 ：

- 创建「about」页面
- 在站点根目录的 source 目录，新建一个about目录 。这个文件目录与 link属性 后的目录所对应，在里面创建一个 index.md 文件 , 在此创作 ablout内容 。

- 创建「group」页面
- 在站点根目录的 source目录，新建一个group目录 这个文件目录与 link属性 后的目录所对应
    ，在里面创建一个index.md 文件, fort-matter里面添加属性

```
    ---
    title: group
    date: 2017-01-17 21:05:04
    layout: links
    ---
```
然后 在站点根目录的 source目录 _data目录(没有的话新建一个)。然后在里面新建一个“ links.yml ”文件
```
名称 :
      link : 点击连接地址   
      avatar: 头像地址
      descr: 描述
```
多的也参照这种格式。
- 创建「gallery」页面
 在站点根目录的 source目录，新建一个gallery目录 这个文件目录与 link属性 后的目录所对应 ，在里面创建一个index.md 文件, fort-matter里面添加属性

```
    ---
    title: Gallery
    date: 2017-01-17 21:39:03
    layout: gallery
    ---
```
然后 在站点根目录的 source目录 _data目录(没有的话新建一个)。然后在里面新建一个“ gallery.yml ”文件

```
图片名称 :
  full_link : 图片地址
  thumb_link :略缩图地址
  descr : 图片描述

```
多的也参照这种格式。

- 创建「tag」页面
 在站点根目录的 source目录，新建一个tag目录 这个文件目录与 link属性 后的目录所对应
    ，在里面创建一个index.md 文件, fort-matter里面添加属性

```
    ---
    title: tags
    date: 2017-01-17 21:39:14
    layout: tags
    ---

```
ok 回到配置文件

- MainFirst: 导航栏下面的主页
     name: 大标题 名字
    description: 第二标签 描述   
     pic_url: 图片地址
     goto_ulr: 点击跳转


 Gallery :  图库页
     title: 标题  
    description: 描述

字体文件 不建议修改

 评论系统
 comment:
   use: disqus_click
   shortname: http-miccall-tech
  duoshuo_thread_key_type: path
   duoshuo_embed_js_url: "https://static.duoshuo.com/embed.js"
 changyan_appid:
     changyan_conf:
   changyan_thread_key_type: path


搜索系统
  search:
    use: google
    swiftype_key: Just another fine responsive  

Leancloud Views
leancloud:
    enable: false
    app_id: #你的 app_id
    app_key: #你的 app_key
    av_core_mini: "https://cdn1.lncld.net/static/js/av-core-mini-0.6.1.js"

访问量系统
  Busuanzi 不蒜子 Views
  busuanzi:
    enable: true   是否开启
    all_site_uv: true   全局启用 
    post_pv: true   单独文章启用 
    busuanzi_pure_mini_js: "https://dn-lbstatics.qbox.me/busuanzi/2.3/busuanzi.pure.mini.js"


- 开始创作你的文章: 
文章目录在 souice目录 的 _post目录下 以md格式文件的文章页 
新建一个md文件 格式为

```
		---

		title: 文章标题  
		date: 2017/3/27 13:48:25  文章发表时间 
		tags: 
		- 标签1
		- 标签2 ( 可选 )
		categories: Algorithm  分类
		thumbnail: https://xxxxxxxxxx.png    略缩图 
		（更多请访问hexo官网 ）
		---

		---
		。。。 文章正文 

```

### 代码高亮
  
  安装组件 参阅 http://github.com/ele828/hexo-prism-plugin


## Contributing 贡献
 欢迎各种形式的贡献，包括但不限于优化，添加功能，文档 & 代码的改进，问题和 bugs 的报告。期待您的 Pull Request。

## License 许可证
license
Open sourced under the GPL v3.0 license.
根据 GPL V3.0 许可证开源。
