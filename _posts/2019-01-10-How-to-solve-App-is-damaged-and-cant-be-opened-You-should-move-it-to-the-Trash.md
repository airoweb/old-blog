---
layout: post
title: "How to solve “App” is damaged and can’t be opened. You should move it to the Trash?"
categories: MacOS
author: "Behzad Amirinezhad"
meta: "apple"
---

Some installation error about damaged disk image. Run in terminal :
```bash
sudo spctl --master-disable
```
Now you can run your app!

You can enable it again by:
```bash
sudo spctl --master-enable
```
