---
layout: post
title: "How to make div fixed after you scroll to that div?"
categories: Javascript
author: "Behzad Amirinezhad"
meta: "Javascript"
---

You have need HTML code like this:

```html
<div class="fixme"></div>
```

and then this javascript to apply css:

```javascript
var fixmeTop = $('.fixme').offset().top;
$(window).scroll(function() {
    var currentScroll = $(window).scrollTop();
    if (currentScroll >= fixmeTop) {
        $('.fixme').css({
            position: 'fixed',
            top: '0',
            left: '0'
        });
    } else {
        $('.fixme').css({
            position: 'static'
        });
    }
});
```

> [External Link](http://jsfiddle.net/5n5MA/2/)
