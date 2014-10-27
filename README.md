third (Third-party developers)
=====

第三方嵌入方向开发，通过在宿主网站嵌入一段代码(`js`or`html`or any other)，最终达到想要的效果（譬如展现一段广告，统计网名行为数据，
导流等）。

这类代码通常会具有可复用性，需要有顽强的生命力，能够在任何网站环境下面生存。

那么，他是否如正常的网站开发一样呢？答案是否定的。

###与普通网站的区别
-很明晰，`寄生`在其它网站，环境不受控制奥

###代码引入方式
-js
-html
-...

###css
我们常见的reset.css长这样  查看 [YUI CSS RESET](http://yui.yahooapis.com/3.18.0/build/cssreset/cssreset-min.css)

```html
html {
    color:#000;
    background:#FFF
}
body,div,dl,dt,dd,ul,ol,li,h1,h2,h3,h4,h5,h6,pre,code,form,fieldset,legend,input,textarea,p,blockquote,th,td {
    margin:0;
    padding:0
}
table {
    border-collapse:collapse;
    border-spacing:0
}
fieldset,img {
    border:0
}
address,caption,cite,code,dfn,em,strong,th,var {
    font-style:normal;
    font-weight:normal
}
ol,ul {
    list-style:none
}
caption,th {
    text-align:left
}
h1,h2,h3,h4,h5,h6 {
    font-size:100%;
    font-weight:normal
}
q:before,q:after {
    content:''
}
abbr,acronym {
    border:0;
    font-variant:normal
}
sup {
    vertical-align:text-top
}
sub {
    vertical-align:text-bottom
}
input,textarea,select {
    font-family:inherit;
    font-size:inherit;
    font-weight:inherit;
    *font-size:100%
}
legend {
    color:#000
}
#yui3-css-stamp.cssreset {
    display:none
}
```
但是，第三方开发中绝不能止步于此，为什么？

通常的开发，reset.css的含义更多的是为了磨平不同浏览器对属性默认值的理解。

而第三方开发，是需要抗干扰，需要重置，需要阻止每一个属性对于第三方内容的样式污染

譬如，宿主网站定义了这样一个属性

```html
    div {
    width: 200px;
}
```
一行简单的代码，你的内容是不是就悲剧的发生了难以置信的变化？

改怎么做？请参考[third reset.css](css/reset.css)

###开发注意事项
-怎么保证css环境的纯净
-js环境？

