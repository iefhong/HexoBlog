---
title: Hexo Doc
date: 2017-06-05 13:47:21
categories:
- programming
tags:
- other
---
Hexo博客的用法，官方的文档写的有一些简单。很多点受限于英文水平，一直没有看懂。  
后面通过实践以及一些技术博客，慢慢了解到Hexo的语法。  
hexo的markdown支持格式有点奇怪，vs code里面编辑好的页面在hexo生成的静态页面中没有显示正确的样式(如无序列表)

# Hexo结构
* _config.yml  
    源代码文件夹下的_config.yml文件，通过yaml文件进行Hexo的基本设置。[站点信息、链接、源码文件夹、写作格式、分类、标签、时间格式、分页、主题、发布等]
* source文件夹
    用于存放markdown文档和assets文件夹(需要配置post_asset_folder为true)
* public文件夹
    用于存放编译后的Hexo静态页面
* scaffolds文件夹
    用于设置博客基本样式,不是很懂
* themes文件夹
    用于保存、设置主题
* db.json
    用于保存Hexo的变量信息，包含hexo的分类、标签信息等。自动生成，除必要的删除某些信息，否则不去修改。

# Hexo常用命令
* Init
    ```
    $ hexo init [folder]
    ```
    folder为项目名，命令为生成一个新的Hexo项目

* New
    ```
    $ hexo new [layout] <title>
    ```

    layout默认为文章，title为文件标题(有空格时，需要用引号)  
    layout
    * page 
    页面
    * post 
    文章 (default)
    * archive
    文档
    * category 
    分类
    * tag 
    标签  

* 生成静态页面
    ```
    $ hexo generate
    ```

* 本地服务器调试
    ```
    $ hexo server
    ```

* 发布
    ```
    $ hexo deploy
    ```

* 清理缓存文件db.json
    ```
    $ hexo clean
    ```
