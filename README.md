# multiple-pages

> 基于vue-cli的vue多页面配置模板

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8181
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report
```
## 如何使用

项目根目录pages中添加对应页面的js 和 vue文件 

在app.json中添加对应的页面配置 （例子在app.json中） 
``` javascript
    {
        "pages":[                                       //页面文件数组
            {
                "entry":"about",                        //入口文件名称
                "title":"关于",                         //该页面的标题
                "cdn":{                                 //该页面的需要加载的cdn
                    "js":[
                        
                    ]
                }
            },{
                "entry":"home",
                "title":"首页",
                "cdn":{}
            },{
                "entry":"index",
                "title":"主页",
                "cdn":{}
            }
        ],
        "basePath": "./src/pages/",                     //pages文件夹的相对路径
        "cdn": {                                        //每个页面都需要加载的cdn
            "js": [
                "https://cdn.bootcss.com/vue/2.5.2/vue.min.js",
                "https://cdn.bootcss.com/element-ui/2.1.0/index.js"
            ],
            "css": [
                "https://cdn.bootcss.com/element-ui/2.1.0/theme-chalk/index.css"
            ]
        },
        "externals": {                                  //打包的时候需要排除的项目依赖
            "vue": "Vue",
            "element-ui": "ElementUI"
        }

    }
```

## 参考文章
《用 cooking 搭建一个多页面易配置的 Vue 2 项目（进阶篇）》(https://zhuanlan.zhihu.com/p/22610408)

For a detailed explanation on how things work, check out the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).
