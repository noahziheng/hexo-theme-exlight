# exLight 主题

[Hexo](http://hexo.io) [Light](https://github.com/hexojs/hexo-theme-light) 主题中国大陆本地化分支

## 安装

在hexo根目录运行运行以下命令来安装exlight主题

```
git clone https://github.com/noahziheng/hexo-theme-exlight.git themes/exlight
```

## 特征

exLight主题相比light原主题有以下改动:  
 * 移除自带的墙内无法使用的FacebookComment，加入多说评论支持，仍支持hexo自带的disqus配置
 * 加入新的个人介绍挂件(感谢[Icarus](http://blog.zhangruipeng.me/hexo-theme-icarus/)提供灵感)，提供主要SNS链接
 * 加入友链挂件，只支持修改ejs添加友链的方式
 * 加入微博秀挂件
 * 替换搜索挂件为[TinySou](http://tinysou.com/)支持
 * 加入百度统计支持，保留Google Analytics支持
 * 加入JiaThis分享取代原生的墙内不可用分享组件
 * 加入InstantClick优化插件，提高加载速度

效果请参看我的博客[Noah's Blog](http://noahgao.net)  

## 配置

默认配置:

``` yaml
menu:
  Home: /
  Archives: /archives
  Projects: /projects
  About: /about

widgets:
- profile #个人介绍挂件
- search #基于TinySou的小挂件，需配置下面的TinySou标志
- recent_posts #最近文章挂件
- category #分类挂件
- tagcloud #标签云挂件
- weibo #微博秀挂件，需配置底下的UID
- links #友链挂件，添加友链需修改./layout/_widget/links.ejs
#另有tag挂件可选

excerpt_link: 阅读全文

jiathis:
  enable: true #JiaThis分享开关

fancybox: true #fancybox配置
baidu_tongji: #百度统计
google_analytics: #UA-XXXXXX-X
rss: #可不填写
duoshuo_shortname: noahgao #多说评论名称

tinysou_id: #tinysou引擎ID

weibo_uid: 2652975830 #微博秀UID
SNS: #右侧个人介绍widget社交链接配置
  github: http://github.com/noahziheng
  twitter: https://twitter.com/noahziheng
  facebook: https://www.facebook.com/profile.php?id=100007443646852
  weibo: http://weibo.com/noah1719
  zhihu: http://www.zhihu.com/people/noah-gao
profile: #右侧个人介绍widget配置
  name: #你的名字
  headimg: #你的头像地址
  description: #你的一句话简介
  location:  #你的位置
```
---
**以下是light主题官方使用方式介绍，exLight全部支持**
## Features

### Gallery Post

![](http://i.minus.com/ibp6Hbytwgof9y.jpg)

```
---
layout: photo
title: Gallery Post
photos:
- http://i.minus.com/ibobbTlfxZgITW.jpg
- http://i.minus.com/iedpg90Y0exFS.jpg
---
```

### Link Post

![](http://i.minus.com/i7hBbGqh14EWo.png)

```
---
layout: link
title: Link Post
link: http://www.google.com/
---
```

### Tweet Widget

![](http://i.minus.com/iMC8EyF9y0Y3y.PNG)

### Fancybox

![](http://i.minus.com/iHv7h7rZNqHvo.PNG)

[Hexo]: http://zespia.tw/hexo/
[Fancybox]: http://fancyapps.com/fancybox/