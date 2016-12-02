# Bleak


> 感谢Peter Amende的主题[bleak](https://github.com/zutrinken/bleak)，本主题由此改造而成。

***


# 介绍


###我对原主题的改动

 - 修改字体，使其适应中文版ghost
 - 使用 [highlight.js](https://highlightjs.org/) 实现代码高亮
 - 使用 [iconfont](http://www.iconfont.cn/plus)添加github和微博图标
 - 修改原主题滚动视差卡顿失效的bug
 - 将一些指示修改成符合中文语境
 - 添加多说评论

可以访问我的博客查看[demo](http://sunchen.com.cn/)

##安装

首先确保你的服务器已经安装了 Git

进入 ghost 根目录下的 themes 文件夹(`ghost/content/themes`)，然后运行以下命令：

```bash
git clone https://github.com/sunchen1996/bleak-master
```

重启 ghost 服务，进入后台就可以看到 bleak这个主题了。

## 更新

在 `themes/bleak-master` 目录下执行：

```bash
git pull origin
``` 

## 自定义
我对原主题做了一些改动，主要有：

### 代码高亮

采用 [highlight.js](https://highlightjs.org/) 做代码高亮，只需要修改 `default.hbs` 中的主题即可，默认采用 tomorrow 主题：

```
<link rel="stylesheet" type="text/css" href="{{asset "css/highlight/tomorrow.css"}}" />
```

### 社交按钮与图标

采用 [iconfont](http://www.iconfont.cn/plus)的图标字体来展示社交按钮，请参考我的 `css/style.css` 文件中的代码：

```html
@font-face {font-family: "iconfont";
    src: url('../iconfont/iconfont.eot?t=1479649402048'); /* IE9*/
    src: url('../iconfont/iconfont.eot?t=1479649402048#iefix') format('embedded-opentype'), /* IE6-IE8 */
    url('../iconfont/iconfont.woff?t=1479649402048') format('woff'), /* chrome, firefox */
    url('../iconfont/iconfont.ttf?t=1479649402048') format('truetype'), /* chrome, firefox, opera, Safari, Android, iOS 4.2+*/
    url('../iconfont/iconfont.svg?t=1479649402048#iconfont') format('svg'); /* iOS 4.1- */
}

.iconfont {
    font-family:"iconfont" !important;
    font-size:16px;
    font-style:normal;
    -webkit-font-smoothing: antialiased;
    -webkit-text-stroke-width: 0.2px;
    -moz-osx-font-smoothing: grayscale;
}
```

如果你需要使用别的图片，只要去 [iconfont](http://www.iconfont.cn/plus)查找即可。


###多说
在`default.hbs`文件中
```
    <script>var duoshuoQuery = {short_name:"替换为你自己的多说二级域名"};</script>
```



##说明
bleak是一个很有潜力的主题，至少我很喜欢，虽然原作者早已放弃更新维护，但我仍然会不断对它进行开发与修改。

##License

MIT © [sunchen](http://sunchen.com.cn)