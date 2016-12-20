# 第四节 book.json配置文件
在图书根目录下的book.json文件是gitbook软件的配置参数文件，主要用于对gitbook软件的插件功能进行配置。如下所示：

源码：

    {
       "plugins": [
          "swiftype"
       ],
       "pluginsConfig": {
          "swiftype": {
             "token": "utQHy1R2XyiVqDqaZxxx",
             "version": "2.0.0"
          }
       }
    }

 gitbook有很多插件，比如更好用的代码高亮插件Prism，该插件需要把原有代码高亮插件highlight移除，以避免冲突。如下用法：
 
     {
        "plugins": [
           "prism","-highlight"
        ]
     }
    
也可以添加自己的CSS样式
    
    {
        "styles": {
          "website": "docs/styles/website.css"
        }
    }




