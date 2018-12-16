---
layout: post
title: "How to use PhpMyAdmin to do a find & replace in your database"
categories: Database
author: "Behzad Amirinezhad"
meta: "database"
---
Run this query to find A and replace with B:

```php
UPDATE `tablename` SET `fieldname` = REPLACE(title,'A','B')
//optional when you search in a Drupal database.WHERE  `type` =  'fieldtype' AND  `fieldname` LIKE  '%A%'
```
> Note: You can use "WHERE" to limit your search.
