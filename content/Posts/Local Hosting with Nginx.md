---
title: How I local Hosted this
date: 2026-02-23
draft: false
tags:
  - Localhost
  - HomeLab
---
I locally hosted this using nginx, I downloaded the repo and pointed nginx at the html file, I then made a bash script that checks for new repo, downloads it and reloads nginx. I then used crontab to run that script every 10 minutes, this website was then forwarded through a cloudflared tunnel.

![Image Description](/images/IMG_0265.png) A photo of the machine hosting this server