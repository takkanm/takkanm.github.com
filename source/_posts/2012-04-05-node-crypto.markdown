---
layout: post
title: 'node.jsでsha1の値が欲しいとき'
date: 2012-04-05 06:45
comments: true
categories: diary
---

[Crypto](http://nodejs.org/docs/latest/api/crypto.html)モジュールを使用すればいいのですね。

```coffee
crypto = require 'crypto'

# sha1でハッシュを作ることを指定
sha1_hash = crypto.createHash 'sha1'

# 使用する原文を追加
sha1_hash.update 'abcdefg'

# ダイジェストの値を求める。引数でhexやbase64等を指定できる
sha1_hash.digest 'hex' #=> 2fb5e13419fc89246865e7a324f476ec624e8740
```
