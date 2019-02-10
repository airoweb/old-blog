---
layout: post
title: "How can I POST flag by REST API in Drupal 8 / JSON Sample"
categories: Drupal
author: "Behzad Amirinezhad"
meta: "flag"
---

Endpoint URL :
```html
Method : Post
https://example.com/entity/flagging?_format=json
```

Headers Parameter:
```html
X-CSRF-Token: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
Authorization: Basic Ud38dasd23rfcFECWq8239c2edc==
Content-Type: application/json
```

Body JSON:
```json
{
  "entity_id":["38"],
  "entity_type":["node"],
  "flag_id":[{"target_id": "bookmark","target_type": "flag"}],
  "uid": ["1"]
}
```

Tested with:
> [Drupal 8.6.9](https://www.drupal.org/project/drupal/releases/8.6.9)

> [Flag 4.0 alpha3](https://www.drupal.org/project/flag/releases/8.x-4.0-alpha3)
