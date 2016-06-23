---
layout: post
title:  "What's going on with Jabit?"
date:   2016-06-23 16:20:55 +0200
categories: jabit
---
I recently implemented acknowledgements, which was still mmissing. As it broke a few things -- not in a big way, but nevertheless -- I wanted to implement a few more possibly breaking changes.

More specifically, I want to improve network performance, which currently seems to have a few performance issues. The new NetworkHandler uses java.nio and therefore uses fewer threads. On the other hand, it needs about 4 MiB per connection, which of course cries optimization. Also, it still doesn't work properly.

Another thing I'd like to look at: the service provider interface, which could possibly make creation of the `BitmessageContext` substantially easier.

And then my notebook is being repaired, making it hard to keep working for the time being, so I'll try to improve documentation instead.

