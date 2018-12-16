---
layout: post
title: "Change files and folders permission with ssh"
categories: Server
author: "Behzad Amirinezhad"
meta: "ssh"
---
Run in your root ssh

for directories :
```ssh
find /home/username/domains/example.com/public_html/ -type d -print0 | xargs -0 chmod 0755
```

for files :
```ssh
find /home/username/domains/example.com/public_html/ -type f -print0 | xargs -0 chmod 0644
```
> Note: change "username" with your hosting account's username and "example.com" with your domain name.
