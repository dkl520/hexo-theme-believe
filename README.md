# hexo-theme-believe

这个主题取名believe.希望选用这个主题的人永远相信美好的事情即将发生。
A simple theme for Hexo named believe. :point_right: [Demo](http://www.tianhao.site/blog) :point_left:

## ScreenShot
![Daily](http://oct3pmpde.bkt.clouddn.com/fengmian.jpg)

## Usage
1. In the `root` directory:
    ```git
    $ git clone https://github.com/th720309/hexo-theme-believe.git
    $ npm install --save hexo-renderer-sass
    ```

2. Change the `theme` property in the `config.yml` file.
    ```yml
    # theme: landscape
    theme: hexo-theme-believe
    ```

3. Run: `hexo server`


##Configuration
     


----------


```
# basic
title: believe
subtitle: 笔直向前，说到做到
favicon: /favicon.ico

#logo
logo: http://oct3pmpde.bkt.clouddn.com/timg.jpg

# duoshuo-comment
#duoshuo_shortname: th720309

highlight:
  enable: true
  line_number: false
  auto_detect: false
  tab_replace:

# nav #
nav:
  首页: .
  归档: archives
  关于: about
  项目: project
  RSS: atom.xml

# baiduanalysis
  #baiduanalysis: 

# hexo-renderer-sass
node_sass:
  outputStyle: nested
  precision: 5
  sourceComments: false

# Default post title
default_post_title: Untitled

# social
social:
  github: https://github.com/th720309
  weibo: http://weibo.com/th0527
  twitter: https://twitter.com
  facebook: https://facebook.com

footer: Powered by <a href="https://hexo.io/">Hexo</a> with Theme <a href="http://www.tianhao.site/blog">believe</a>
```

##Features


----------

How to add comment field in your article?
-----------------------------------------

    
  编辑站点的 config.yml ，添加 duoshuo_shortname 字段，设置如下  
             
    # duoshuo-comment
        duoshuo_shortname: 此处为你的多说帐号
           　

How to add baiduanalysis in your website?
-----------------------------------------

        
     # baiduanalysis(用于百度站长工具验证所有权的ID)
        (sample)baiduanalysis:  https://hm.baidu.com/hm.js?c0451e16533956173997b85f7a8de666
           

How to customize page footer?
-----------------------------

编辑站点的 _config.yml，添加

     footer: 你要自定义的内容（支持HTML标签）
      # 举例：
     # footer:  Powered by <a href="https://hexo.io/">Hexo</a> with Theme <a href="http://www.tianhao.site/blog">believe</a>


最近看到好多同学使用了这个主题，遇到一些问题，我统一回复一下。


----------
## 留言和关于页 ##

　　　许多同学添加了这两个页面后发现没有显示，not found 404,　原因是未添加内容。找到hexo文件夹，找到source文件夹，添加对应名称文件夹，文件夹内添加index.md文件，index.md文件内输入markdown格式文档，便可以显示出来相对应的专页了。如下所示：

```
﻿---
layout: post
title: 关于我　
type: about
tag: 关于
---
					
## **About Me**

关于我，一个未来的小小程序员，茫茫宇宙中的一粒小石子。目前就读于大连交通大学，一个苦逼的理工男。凭借着一点点的兴趣已经走过了三个年头，现在已经是大四的老油条，但总的来说还是一个小屁孩，哈哈。

## **About Blog**

平时喜欢写写博客，之前一直在CSDN记录一些算法题和一些完成的小作品，这次借助hexo+Github page 搭建了这个博客，打算写写个人的一些感悟影评什么的，当然可能也会有一些IT类的文章，谁让我是苦逼理工男（逃）。

## **Contact Me**

新浪微博：[点击进入我的新浪微博（可以加个关注哈哈）](http://weibo.com/th0527)

知乎：[点击进入我的知乎](https://www.zhihu.com/people/tian-hao-69-26)

Github:  [点击进入我的github(欢迎fork me)](https://github.com/th720309)

CSDN : [点击进入我的CSDN](http://blog.csdn.net/u013775952)
```


----------


## 相册页 ##

相册页相对比较麻烦，这是我个人针对自己的博客的个人化定制，没打算放入hexo 主题框架中，毕竟这是一个静态网站，相册的添加不是那么容易，，如需添加相册页，需要自己懂得html和css布局，因为相册页属于个人化定制，所以在此不放代码共享了，如若想加入该专业，可以在believe主题文件夹下找到layout文件夹，在里面添加photo.ejs，自主化定制自己的photo.ejs，然后如关于页相同，不同的是在index.md中layout一栏为photo.

