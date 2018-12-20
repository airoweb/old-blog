
]---
layout: post
title: "How to make div fixed after you scroll to that div?"
categories: Javascript
author: "Behzad Amirinezhad"
meta: "Javascript"
---

I am trying to send a post and commit it from my phone.

```html
<div class="fixme"></div>
```

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
