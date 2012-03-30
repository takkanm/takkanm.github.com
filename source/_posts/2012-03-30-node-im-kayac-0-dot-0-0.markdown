---
layout: post
title: "im.kayac.comにメッセージを送るnpmモジュールを書いた"
date: 2012-03-30 08:33
comments: true
categories: diary
---

昨年iPhoneに変更して、push通知サービスに[Boxcar](http://boxcar.io/)を使っていたのですが、私のiPhoneではうまく動かないことが多いため不満でした。 そこで、(今更感はありますが)[im.kayac.com](http://im.kayac.com/)を使うことにしてみました。

最近coffeescriptを触る機会が増えてきたので、node.jsで使えるライブラリをcoffeescriptで書いてnpm化してみました。node.jsでリアルタイムな何かをiPhoneやAndroidに通知したいとき等に、お使いください。

- [npm registry](http://search.npmjs.org/#/node-im-kayac)
- [takkanm/node-im-kayac](https://github.com/takkanm/node-im-kayac)

まだ、メッセージを送るだけしかできないので、残りのところもちゃんと作っていこうと思います。

初めてのnpmモジュール作成だったので(その手順とかは後で書く)、このモジュールの配置でいいのかとか大変疑問なので有識者に聞いてみたいところ。
