---
layout: post
title: "Varnish One Liners"
date: 2014-08-18 16:28
comments: false
categories: devops
---

Fetch varnish logs for particular IP address:
varnishlog -o -c | perl -ne 'BEGIN { $/ = "";} print if (/RxURL.*\/$/m and /ReqStart.*127.0.0.1/);'

Others:
https://www.varnish-cache.org/trac/wiki/VarnishlogExamples
http://mclear.co.uk/2011/04/25/varnishlog-cheat-sheet/
