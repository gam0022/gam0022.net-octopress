---
layout: page
title: "@daigoroubot"
date: 2012-12-10 11:12
comments: true
sharing: true
footer: true
---

# 大五郎BOTとは？

知っている人は知っているTwitterBotです。

マルコフ連鎖で適当につぶやいたりリプをしたり、挨拶や任意のキーワードに反応します。

つくば市の天気予報機能、電卓機能、n進数変換器など便利な機能を搭載しています。

[大五郎（Ｕ＾ω＾）BOT (@daigoroubot)](https://twitter.com/daigoroubot)

# 機能紹介

## つくば市の天気予報機能

### 例

* `@daigoroubot 天気`=> `今日のつくばの天気は、晴れなのだ。最高気温9℃なのだ。http://goo.gl/IPAuV`
* `@daigoroubot 明日 天気`=> `明日のつくばの天気は、晴れなのだ。最高気温9℃、最低気温-1℃なのだ。http://goo.gl/IPAuV`

### 解説

つくば市の天気予報機能なので、*茨城県つくば市の天気にしか対応していません*。

(今日|明日|明後日)のつくば市の天気に対応しています。

日を省略した場合、午後3時までは今日の天気、それより後は明日の天気を教えてくれます。

天気の情報は、livedoorの[Weather Hacks](http://weather.livedoor.com/weather_hacks/)
から取得しています。

## 電卓機能

### 例

* `@daigoroubot 1+1`=> `2`
* `@daigoroubot ３たす３は？` => `6`
* `@daigoroubot 2**10 #べき乗` => `1024`
* `@daigoroubot √ 5`=> `2.23606797749979`
* `@daigoroubot ∑(1..10)` => `55`
* `@daigoroubot ⅞ * ⅔`=> `0.5833333333333333`
* `@daigoroubot (0..10).inject([1, 1]) {|fib, i| fib << fib[i] + fib[i+1] }` => `[1, 2, 3, 5, 8, 13, 21, 34, 55, 89, 144, 233]`
* `@daigoroubot PI` => `3.141592653589793`
* `@daigoroubot sin(PI)` => `1.2246063538223773e-16`

### 解説

基本的にはirbみたいな感じに使ってください。

技術的な点だと、Rubyのセーフレベル4 + CleanroomでSandbox環境を作って`eval`して、
スレッドを使って設定した時間でタイムアウトするようになっています。

## n進数変換器

### 例

* `@daigoroubot 1024 2進数` => `1024 = 10000000000(2進数) 1024(2進数) = 2`
* `@daigoroubot 1024を2進数に` => `1024 = 10000000000(2進数)`
* `@daigoroubot ffは16進数で` => `ff(16進数) = 255`

### 解説

なんと2進数から36進数までに対応しています！

# 開発方法など

大五郎はRuby1.9.3で開発されており、月額490円のVPS上で動いています。

* 直前の2単語によるマルコフ連鎖。
* 泥臭いアルゴリズムによって語尾の「なのだ」を実装。
* 他のbotに比べれば、設定ファイルでけっこう柔軟に設定できる感じの設計。

ソースコードは[github](https://github.com/gam0022/daigoroubot)に置いてます。
