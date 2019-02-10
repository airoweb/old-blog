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
```json
X-CSRF-Token: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
Authorization: Basic Ud38dasd23rfcFECWq8239c2edc==
Content-Type: application/json
```

Body JSON:
```json
{
  "entity_id":["38"], //Node ID 
  "entity_type":["node"],
  "flag_id":[{"target_id": "bookmark","target_type": "flag"}],
  "uid": ["1"] // User ID
}
```
