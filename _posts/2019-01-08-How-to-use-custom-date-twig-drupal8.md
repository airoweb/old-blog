---
layout: post
title: "How to use custom date format in Drupal 8 Twig template"
categories: Drupal
author: "Behzad Amirinezhad"
meta: "php"
---

Replace default {{ date }} with follofing code:

```php
 { { node.getCreatedTime|format_date('persiandate') } }
```


> Note: "persiandate" is machine name of your custom date format

