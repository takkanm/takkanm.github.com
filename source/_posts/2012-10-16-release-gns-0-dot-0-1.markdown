---
layout: post
title: "GitHub の personalized feed を通知センターに表示する gns を作りました"
date: 2012-10-16 00:38
comments: true
categories: ruby
---

[GitHub for Mac が Mountain Lion の通知センターに対応した](https://github.com/blog/1287-github-for-mac-notifications) とのことなので、「これは便利だわー」って使っていたんだけど、通知のためだけに使わないアプリケーションを起動するのはつらいので、似たようなのを作ってみた。

- [gns](https://github.com/takkanm/gns)
- [gns | RubyGems.org](https://rubygems.org/gems/gns)

private なリポジトリへの通知も見たいので、[GitHub API](http://developer.github.com/v3/events/)を使わず、personalized feed から情報をとるようにした。ちゃんと、personalized feed が設定できて起動すれば、こんな感じで通知センターに通知されます。

<a href="http://www.flickr.com/photos/takkanm/8090496232/" title="gns-sample by takkanm, on Flickr"><img src="http://farm9.staticflickr.com/8196/8090496232_d6673d7021_m.jpg" width="240" height="58" alt="gns-sample"></a>

通知には [terminal-notifier](https://github.com/alloy/terminal-notifier/tree/master/Ruby) を使ってるのですが、これだと通知センターのタイトルとアイコンが terminal-notifier のものになるので、ここも自作できたらいいなぁと思っております。あと、リアルタイムで取得しているわけではなく 1 分間隔で監視しているので、監視間隔をもう少し変更できるといいなぁ。
