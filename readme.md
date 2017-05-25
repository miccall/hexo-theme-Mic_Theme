---
# Miccall Theme 
###### version 1.0.1 
---
![title][1] 
## Contents 目录

- General 概括
- Demo 演示
- Quick start 快速开始
- Docs 文档
- Contributing 贡献
- License 许可证

## General概括 

主题开发 套用了大量的[HTML5 UP][2] 模板 因为作者是前端小白 css功底菜鸡
在此鸣谢支持我的各位大佬 

## Demo 演示
 - [miccall.tech][3]
![此处输入图片的描述][4]

![此处输入图片的描述][5]

![此处输入图片的描述][6]

## Quick start 快速开始
 - 安装 hexo 
 - 请仔细阅读 Hexo 的官方文档，完成对 Hexo 的安装和基本的配置 。
 - 下载本主题 并且放置于themes目录下 更改主题名字 并在站点根目录的配置文件中启用该主题 
 - 在主题的配置文件中修改相应的值

## Docs 文档

- head: 网站的logo  头像 高清头像 关键字  
    favicon: 
    high_res_favicon: 
    apple_touch_icon: 
    keywords: 

- Intro: 主题刚开始加载的界面 名字 第二标语 主页按钮名字 
    name: 
    slogan: 
    HeadButton: 

- Nav: 导航栏  
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
            link: "/about/"  link 的参数为相对路径，对应 hexo 目录下的 source 文件夹内的相应文件夹。 
        团队 :
            link: "/group/"
        图库 :
            link: "/gallery/"
        标签:
            link: "/tag/"
        #自定义标签名
        #   link：“路径”
使用方法 ： 
 - 创建「about」页面
   在站点根的source目录 新建一个abou目录 这个文件目录与 link 后的目录所对应 
   在里面创建一个md文件 在此创作 
 - 创建「group」页面
    在站点根的source目录 新建一个group目录 这个文件目录与 link 后的目录所对应
    在里面创建一个md文件 命名index formatter里面 layout: links 
    然后 在站点根的source目录 _data
 - 创建「gallery」页面
 - 创建「tag」页面
 
- MainFirst: 导航栏下面的主页 
    name: 大标题 名字 
    description: 第二标签 描述   
    pic_url: 图片地址 
    goto_ulr: 点击跳转 
- Gallery :  图库页 
    title: 标题  
    description: 描述 
字体文件 不建议修改 
 
- 评论系统 
comment:
    use: disqus_click
    shortname: http-miccall-tech 
    duoshuo_thread_key_type: path
    duoshuo_embed_js_url: "https://static.duoshuo.com/embed.js"
    changyan_appid:
    changyan_conf:
    changyan_thread_key_type: path

- 搜索系统 
search:
    use: google
    swiftype_key: Just another fine responsive  

Leancloud Views
leancloud:
    enable: false
    app_id: #你的 app_id
    app_key: #你的 app_key
    av_core_mini: "https://cdn1.lncld.net/static/js/av-core-mini-0.6.1.js"
    
- 访问量系统 
Busuanzi 不蒜子 Views
busuanzi:
    enable: true
    all_site_uv: true
    post_pv: true
    busuanzi_pure_mini_js: "https://dn-lbstatics.qbox.me/busuanzi/2.3/busuanzi.pure.mini.js"

## Contributing 贡献
 欢迎各种形式的贡献，包括但不限于优化，添加功能，文档 & 代码的改进，问题和 bugs 的报告。期待您的 Pull Request。
 
## License 许可证
license
Open sourced under the GPL v3.0 license.
根据 GPL V3.0 许可证开源。



  [1]: 
  [2]: 
  [3]: 
  [4]: 
  [5]: http://onh0umlhz.bkt.clouddn.com/0524theme003.PNG
  [6]: http://onh0umlhz.bkt.clouddn.com/0524theme004.PNG