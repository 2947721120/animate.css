#Animate.css
*Just-add-water CSS animation*

`animate.css` 是一个很酷，有趣，和跨浏览器动画为您使用在您的项目。伟大的强调，主页，滑块，一般只需加水魅力。

##基本用法
1. 包括在您的文档中的样式表 `<head>`

  ```html
  <head>
    <link rel="stylesheet" href="animate.min.css">
  </head>
  ```
2. 添加类“动画”的元素，你想动画。

您还可以将类的。添加class `animated` 你想持续动画。
 您还可以将class的 `infinite` 包含为一个无限循环.

3. 最后，您需要添加下列class之一：

  * `bounce`
  * `flash`
  * `pulse`
  * `rubberBand`
  * `shake`
  * `headShake`
  * `swing`
  * `tada`
  * `wobble`
  * `jello`
  * `bounceIn`
  * `bounceInDown`
  * `bounceInLeft`
  * `bounceInRight`
  * `bounceInUp`
  * `bounceOut`
  * `bounceOutDown`
  * `bounceOutLeft`
  * `bounceOutRight`
  * `bounceOutUp`
  * `fadeIn`
  * `fadeInDown`
  * `fadeInDownBig`
  * `fadeInLeft`
  * `fadeInLeftBig`
  * `fadeInRight`
  * `fadeInRightBig`
  * `fadeInUp`
  * `fadeInUpBig`
  * `fadeOut`
  * `fadeOutDown`
  * `fadeOutDownBig`
  * `fadeOutLeft`
  * `fadeOutLeftBig`
  * `fadeOutRight`
  * `fadeOutRightBig`
  * `fadeOutUp`
  * `fadeOutUpBig`
  * `flipInX`
  * `flipInY`
  * `flipOutX`
  * `flipOutY`
  * `lightSpeedIn`
  * `lightSpeedOut`
  * `rotateIn`
  * `rotateInDownLeft`
  * `rotateInDownRight`
  * `rotateInUpLeft`
  * `rotateInUpRight`
  * `rotateOut`
  * `rotateOutDownLeft`
  * `rotateOutDownRight`
  * `rotateOutUpLeft`
  * `rotateOutUpRight`
  * `hinge`
  * `rollIn`
  * `rollOut`
  * `zoomIn`
  * `zoomInDown`
  * `zoomInLeft`
  * `zoomInRight`
  * `zoomInUp`
  * `zoomOut`
  * `zoomOutDown`
  * `zoomOutLeft`
  * `zoomOutRight`
  * `zoomOutUp`
  * `slideInDown`
  * `slideInLeft`
  * `slideInRight`
  * `slideInUp`
  * `slideOutDown`
  * `slideOutLeft`
  * `slideOutRight`
  * `slideOutUp`

全例子：
```html
<h1 class="animated infinite bounce">例</h1>
```

[Check out all the animations here!](https://daneden.github.io/animate.css/)

##使用
在你的网站上使用animate.css，只需拖放到您的文档中的样式表 `<head>`, 并添加class `animated` 到一个元素，以及任何动画名称。这是它！你已经有了一个CSS动画元素。好极了 !

```html
<head>
  <link rel="stylesheet" href="animate.min.css">
</head>
```

你可以做很多其他的东西animate.css当你结合jQuery或添加您自己的CSS规则。动态添加使用jQuery轻松动画：

```javascript
$('#yourElement').addClass('animated bounceOutLeft');
```

当动画结束时，也可以检测到：

<!--
Before you make changes to this file, you should know that $('#yourElement').one() is *NOT A TYPO*

http://api.jquery.com/one/
-->

```javascript
$('#yourElement').one('webkitAnimationEnd mozAnimationEnd MSAnimationEnd oanimationend animationend', doSomething);
```

[View a video tutorial](https://www.youtube.com/watch?v=CBQGl6zokMs) 关于如何使用Animate.css使用jQuery在这里。 

**Note:** `jQuery.one()` is used when you want to execute the event handler at most *once*. More information [here](http://api.jquery.com/one/).

You can change the duration of your animations, add a delay or change the number of times that it plays:

```css
#yourElement {
  -vendor-animation-duration: 3s;
  -vendor-animation-delay: 2s;
  -vendor-animation-iteration-count: infinite;
}
```

*Note: be sure to replace "vendor" in the CSS with the applicable vendor prefixes (webkit, moz, etc)*

## 自定义生成
Animate.css由 [Grunt](http://gruntjs.com), 您可以创建自定义很容易地构建。首先，你需要步兵和其他所有依赖关系：

```sh
$ cd path/to/animate.css/
$ sudo npm install
```

Next, run `grunt watch` to watch for changes and compile your custom builds. For example, if you want only some of the the “attention seekers”, simply edit the `animate-config.json` file to select only the animations you want to use.

```javascript
"attention_seekers": {
  "bounce": true,
  "flash": false,
  "pulse": false,
  "shake": true,
  "headShake": true,
  "swing": true,
  "tada": true,
  "wobble": true,
  "jello":true
}
```

## 许可证
animate.css授权MIT许可下. (http://opensource.org/licenses/MIT)

## Contributing
Pull requests are the way to go here. I apologise in advance for the slow action on pull requests and issues. I only have two rules for submitting a pull request: match the naming convention (camelCase, categorised [fades, bounces, etc]) and let us see a demo of submitted animations in a [pen](http://codepen.io). That last one is important.
