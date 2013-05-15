YUI ScrollSpy Plugin
====================

![Travis Build Status](https://api.travis-ci.org/juandopazo/yui3-scrollspy.png)

A Bootstrap-inspired ScrollSpy plugin for YUI

Getting Started
---------------

Create a new YUI instance for your application and populate it with the modules you need by specifying them as arguments to the `YUI().use()` method. YUI will automatically load any dependencies required by the modules you specify. Then plug the ScrollSpy plugin to the body of the page or any scrollable node and set the `target` attribute to any list that contains links to elements in the page.

```html
<script>
YUI({
    gallery: 'gallery-2013.05.15-21-12'
}).use('gallery-scrollspy', function (Y) {
    
    Y.one('body').plug(Y.Plugin.ScrollSpy, {
        target: '#navbar'
    });

});
</script>
```

Alternatively you can set the target node as a `data-` attribute of the plugged node.

```html
<body data-target="#navgar">...</body>
```
