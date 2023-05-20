---
title: HEXO配置
cover: 'https://img1.acrylic.org.cn/2023/04/16/643b6a036a2cb.webp'
top_group_index: 1
abbrlink: '6387'
date: 2023-03-24 13:10:02
tags:
---
## 根目录下`config.yml`

`5-21排`可替换为
```yml
# Site
title: 张洪Heo #标题
subtitle: '分享科技与生活' #副标题
description: '分享科技与生活' #描述
keywords: 张洪Heo,分享科技与生活 #关键词
author: 张洪Heo #作者
language: zh-cn #语言
timezone: '' #时区

# URL
## Set your site url here. For example, if you use GitHub Page, set url as 'https://username.github.io/project'
url: http://acrylic.zhheo.com #链接
permalink: :year/:month/:day/:title/
permalink_defaults:
pretty_urls:
  trailing_index: true # Set to false to remove trailing 'index.html' from permalinks
  trailing_html: true # Set to false to remove trailing '.html' from permalinks
```

## `scaffolds`模板

### 页面模板`scaffolds\page.md`

```md
---
title: {{ title }}
date: {{ date }}
updated: 
description: 
keywords: 
cover: 
layout: 
comments: 
type: 
tips: 
---

```

### 文章模板`scaffolds\post.md`

```md
---
title: {{ title }}
date: {{ date }}
updated: 
categories: 
tags: 
description: 
keywords: 
cover: 
top_group_index: #置顶top_group顺序，非负整数，数字越大越靠前
layout: 
comments: 
---

```

### 默认模板`scaffolds\draft.md`

```md
title: {{ title }}
date: {{ date }}
updated: 
categories: 
tags: 
description: 
keywords: 
cover: 
top_group_index: #置顶top_group顺序，非负整数，数字越大越靠前
layout: 
comments: 
---

```

至此,HEXO配置完毕🎉