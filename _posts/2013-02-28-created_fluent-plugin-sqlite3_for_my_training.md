---
layout: redirect
title: Created fluent-plugin-sqlite3 for my training
tags: fluentd sqlite3 plugin
lang: 
creation-date: 2013-02-28 09:06:29 +0900
modified-date: 2013-02-28 09:06:29 +0900
---
[fluentd][fd] is a cool product so I try it for my biz.

  [fd]: http://fluentd.org/

In the case I use it, I have to write some plugins of fluentd.
For now, as a training, I wrote a small plugin for sqlite3.

<https://github.com/tmtk75/fluent-plugin-sqlite3>

I added [ad hoc mode][adhoc].
It doesn't need you define schema.
It creates tables based on a JSON you sent.
I think you casully start to try this plugin.


Adding a plugin was easier than I've thought.
fluentd is nice!


  [adhoc]: https://github.com/tmtk75/fluent-plugin-sqlite3/blob/master/README.md#getting-started
