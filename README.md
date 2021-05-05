# TwT Diary · TwT 日记

Static pure HTML+CSS markdown diary powered by GitHub Gist.

由GitHub Gist提供服务的静态纯HTML+CSS Markdown日记。

## 就这么简单

修改`index.html`后放在自己的Repo并开启`GitHub Pages`。

### Favicon

替换`<!-- ** Favicon ** -->`部分。

推荐[RealFaviconGenerator.net](RealFaviconGenerator.net)，可以快速生成跨平台、跨浏览器的favicon。

### CSS

可以修改`<!-- ** Internal CSS ** -->`部分的CSS代码定制样式。

Gist的结构如下：

![annotation](https://user-images.githubusercontent.com/12462465/117210899-36ea1980-adf0-11eb-8cde-e87bdfe64405.png)

![structure](https://user-images.githubusercontent.com/12462465/117211652-33a35d80-adf1-11eb-92da-5f2d2664ac96.png)

#### 字体

```css
.gist article.markdown-body {
    font-family: 'Sample', sans-serif;
}

.gist .markdown-body code {
    font-family: inherit !important;
}

.gist article.markdown-body ul {
    font-family: inherit !important;
}
```

#### 字体与背景颜色

```css
div.gist-file {
    color: antiquewhite;
    background: transparent;
}

div.gist-data {
    background: transparent;
}

.gist article.markdown-body {
    background: transparent;
}

.gist .markdown-body code {
    background-color: hsla(0, 0%, 100%, .2) !important;
}
```

#### 隐藏底部hosted by GitHub

```css
.gist-meta {
    display: none;
}
```

### Gist 链接

在GitHub Gist中创建`Secret` (私有) Gist，复制`Embed`嵌入代码，替换`<!-- ** Gist Address Here ** -->`下的部分。

![Snipaste_2021-05-05_21-59-51](https://user-images.githubusercontent.com/12462465/117208705-53388700-aded-11eb-9781-138b38e6f428.png)

```html
<script src="https://gist.github.com/XXX/XXXXX.js"></script>
```
