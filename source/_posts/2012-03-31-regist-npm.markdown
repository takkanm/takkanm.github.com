---
layout: post
title: "npmモジュールを公開する方法"
date: 2012-03-31 18:06
comments: true
categories: diary
---

[先日](http://takkanm.github.com/blog/2012/03/30/node-im-kayac-0-dot-0-0/)npmモジュールを作成し、公開したときのメモを残しておきます。

## ユーザ登録

まず、ユーザー登録します。ユーザ登録するには、npm adduserコマンドを実行します。

```
$ npm adduser
```

コマンドを実行すると、対話的にユーザ名とemailアドレスとパスワードを入力します。その情報は~/.npmrcに保存されます。

## package.jsonの作成

npmモジュールの情報を保存しておくpackage.jsonを作成します。npm initを実行することで、対話的に情報を入力していきます。

```
$ npm init
```

## package registryへの登録

作成したnpmモジュールをpackage registry に登録します。package.jsonのあるディレクトリでnpm publishします。

```
$ npm publish
```
