

# 第二章 如何生成web page
有两种方式可以生成web page。
###1. 直接使用gitbook命令的方式
gitbook自己生成静态网页，不需要用其他web服务器


* 生成到当前目录
 

    cd repoBook
    sudo gitbook serve .
    
### 2. 利用apache 作为web服务器

* 生成static page到指定的目录


    $ mkdir /tmp/gitbook
    $ gitbook build --output=/tmp/gitbook　

* 配置apache子域名




