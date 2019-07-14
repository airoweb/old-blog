
---
layout: post
title: "Remove Other account from MacOS X's login screen"
categories: MacOS
author: "Behzad Amirinezhad"
meta: "apple"
---

Open terminal app and run command :
```bash
Msudo defaults write /Library/Preferences/com.apple.loginwindow SHOWOTHERUSERS_MANAGED -bool FALSE
```

revert it:
```bash
sudo defaults write /Library/Preferences/com.apple.loginwindow SHOWOTHERUSERS_MANAGED -bool TRUE
```
