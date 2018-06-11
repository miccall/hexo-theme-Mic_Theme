# Miccall Theme Readme
###### version 1.2.0

<img src="http://onh0umlhz.bkt.clouddn.com/githubhexothemereadmemain.png" width="100%" />

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

个人网站 : [miccall.tech](http://miccall.tech)

主题文章列表: 
<img src="http://onh0umlhz.bkt.clouddn.com/githubhexothemereadmesecond.png" width="100%" />
主题文章主页: 
<img src="http://onh0umlhz.bkt.clouddn.com/githubhexothemereadmepost.png" width="100%" />
主题图库页: 
<img src="http://onh0umlhz.bkt.clouddn.com/githubhexothemereadmegallery.png" width="100%" />

## Quick start 快速开始

- 请仔细阅读 Hexo 的官方文档，完成对 Hexo 的[安装](https://hexo.io/zh-cn/docs/index.html#%E5%AE%89%E8%A3%85)和[基本的配置](https://hexo.io/zh-cn/docs/configuration.html)。

- 下载本主题并且放置于`themes`目录下，更改主题名字，并在站点根目录的配置文件`_config.yml`中启用该主题。

```
    # Extensions
    ## Plugins: https://hexo.io/plugins/
    ## Themes: https://hexo.io/themes/
    theme: miccall

```
- 在主题的配置文件`_config.yml`中修改相应的值。

## Docs 文档

以下内容均为主题的配置文件 `_config.yml`内容（请区别于站点的配置文件）。

##### 一 . head标签下 

1.网站的logo 
    **favicon:** "/img/logo_miccall.png"

2.搜索的关键字 :
keywords提供的网页关键词通常是为搜索引擎分类网页使用的；
可以为网页提供多个关键词，多个关键词应该使用空格分开；
不要给网页定义过多的关键词，最好保持在10个以下，过多的关键词，搜索引擎将忽略；
不要给网页定义与网页描述内容无关的关键词；
由于网页制作者滥用keywords(提供过多的关键词或者提供与网页无关的关键词)，导致目前常用的搜索引擎降低了keywords的重要性。
    **keywords:** miccall

3.主页背景图片：默认链接是在主站以下目录的 "img/bg.jpg" 就代表"miccall.tech/img/bg.jpg" 暂不支持外链
    **backgroundpic :** "img/bg.jpg"


##### 二 . Intro: 主题刚开始加载的界面
    
1.名字 
    **name:** MICCALL

2.第二标语
    **slogan:** "Whatever is worth doing is worth doing well I'll think of you every step of the way"

3.主页按钮上面的文字     
    **HeadButton:** MICCALL

##### 三 .Nav: 导航栏

```    
    Home_name: 主页 # 主页名字
    is_use_categories : true # 是否启用分类
    categories_name: 分类 # 分类名字
    is_use_archives : false # 是否启用归档
    archives_name: 归档 # 归档名字
    icon: # 导航栏上的图标
        github:
            use: true # 是否启用
            link: https://github.com/miccall # 点击地址
        Twitter:
            use: false
            link:
        Facebook:
            use: false
            link:
        Instagram:
            use: false
            link:
    pages:
    # 自定义连接页
    # link 的参数为相对路径，对应 hexo 目录下的 source 件夹内的相应文件夹
        简历:
            link: "/about/"
        团队 :
            link: "/group/"
        图库 :
            link: "/gallery/"
        标签:
            link: "/tag/"
        #自定义标签名
        #   link：“路径”

    MainFirst: # 导航栏下面的主页
        name: Miccall Metro # 大标题名字
        description: Welcome to my Blog   # 第二标签 描述
        pic_url: /img/me.jpg # 图片地址
        goto_ulr: "" # 点击跳转

    Gallery: # 图库页
        title: Mr.metro
        description: Just another fine responsive
```

使用方法 ：

1. 创建「about」页面

    - 在站点根目录的`source`目录，新建一个`about`目录，这个文件目录与 `link: "/about/"`所对应，在里面创建一个 `index.md` 文件，在此创作 `about`内容。

1. 创建「group」页面

    - 在站点根目录的`source`目录，新建一个`group`目录，这个文件目录与`link: "/group/"`所对应，在里面创建一个`index.md`文件。
    - `front-matter`里面添加属性

        ```
        ---
        title: group
        date: 2017-01-17 21:05:04
        layout: links
        ---
        ```
    - 然后在站点根目录的 `source`目录` _data`目录(没有的话新建一个)。然后在里面新建一个`links.yml`文件，多成员依次添加。
        ```
        # 成员1
        名称 :
              link: 点击连接地址   
              avatar: 头像地址
              descr: 描述
        # 成员2
        名称 :
              link: 点击连接地址   
              avatar: 头像地址
              descr: 描述
        ```

1. 创建「gallery」页面

    - 在站点根目录的`source`目录，新建一个`galler`y目录，这个文件目录与`link: "/gallery/"`所对应 ，在里面创建一个`index.md`文件, `front-matter`里面添加属性

        ```
        ---
        title: Gallery
        date: 2017-01-17 21:39:03
        layout: gallery
        ---
        ```

    - 然后在站点根目录的`source`目录 `_data`目录(没有的话新建一个)。然后在里面新建一个`gallery.yml`文件，多图片依次添加，图片名称不要重复。

        ```
        图片名称1:
          full_link: 图片地址
          thumb_link: 略缩图地址
          descr: 图片描述
        图片名称2:
          full_link: 图片地址
          thumb_link: 略缩图地址
          descr: 图片描述
        ```

1. 创建「tag」页面


    - 在站点根目录的`source`目录，新建一个`tag`目录，这个文件目录与`link: "/tag/"`所对应  ，在里面创建一个`index.md `文件，`front-matter`里面添加属性。

        ```
        ---
        title: tags
        date: 2017-01-17 21:39:14
        layout: tags
        ---
        ```
1. 修改背景图片：更换`\themes\miccall\source\images`中的`bg.jpg`，不要改名，否则需要更改CSS内容。

1. 修改导航栏下面的个人图片：更换`\themes\miccall\source\img`中的`me.jpg`，不要改名，否则需要更改CSS内容。

1. 字体文件不建议修改。

1. 评论系统：`use`的配置选项`false | duoshuo | disqus | disqus_click | changyan`

    ```
    comment:
       use: disqus_click
       shortname: http-miccall-tech
       duoshuo_thread_key_type: path
       duoshuo_embed_js_url: "https://static.duoshuo.com/embed.js"
       changyan_appid:
       changyan_conf:
       changyan_thread_key_type: path
    ```

1. 搜索系统：

    ```
    search:
      use: google
      swiftype_key: Just another fine responsive  
    ```

1. 访问量系统

    ```
    Leancloud Views
    leancloud:
        enable: false
        app_id: # 你的 app_id
        app_key: # 你的 app_key
        av_core_mini: "https://cdn1.lncld.net/static/js/av-core-mini-0.6.1.js"
    ```


    ```
    busuanzi:
      enable: true  #  是否开启
      all_site_uv: true # 全局启用
      post_pv: true # 单独文章启用
      busuanzi_pure_mini_js: "https://dn-lbstatics.qbox.me/busuanzi/2.3/busuanzi.pure.mini.js"
    ```

1. 开始创作你的文章：文章目录在`blog/source/_post`目录下新建一个`.md`文件：

    ```
    ---
    title: # 文章标题  
    date: 2017/3/27 13:48:25  # 文章发表时间
    tags:
    - 标签1
    - 标签2 (可选)
    categories: Algorithm # 分类
    thumbnail: https://xxxxxxxxxx.png # 略缩图
    ---

    文章正文

    ```

### 代码高亮

安装组件参阅http://github.com/ele828/hexo-prism-plugin

## Contributing 贡献

欢迎各种形式的贡献，包括但不限于优化，添加功能，文档 & 代码的改进，问题和 bugs 的报告。期待您的 Pull Request。

- 感谢 [@moecopilot](https://github.com/moecopilot) 的贡献 ： 修复了文章链接 (已更新)
- 更改了画廊中图片为居中及缩放(已更新)
- 主页上会显示categories而不显示tag(涉及到排版问题，没有采用)
- 感谢 [@sli1989](https://github.com/sli1989) 的贡献 ： 修复了主页 me.jpg的设置问题 (已更新)
- 感谢 [@staunchkai](https://github.com/staunchkai)的贡献 : 1. 添加 Valine 评论 
- 2. 导航栏社交图标自定义 
- 感谢 [@acupt](https://github.com/acupt)的贡献 ：1、修复了https网站引用 ‘bootstrap.min.css’ 和 ‘font-awesome.min.css’ 文件错误的问题
- 2、links.yml不配置属性link/qq/wachat/weibo则不显示图标

## License 许可证

license
Open sourced under the GPL v3.0 license.
根据 GPL V3.0 许可证开源。