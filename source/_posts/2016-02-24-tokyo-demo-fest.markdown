---
layout: post
title: "#TokyoDemoFestのGLSL Graphics Compoで3位入賞しました！"
date: 2016-02-24 08:19
comments: true
categories: 
- event
- demo
- CG
---

2016-02-20〜21に開催された[Tokyo Demo Fest 2016](http://tokyodemofest.jp/2016/)に参加して、GLSL Graphics Compoで3位入賞してきました！

Tokyo Demo Festとは、このようなイベントです（公式ページからの引用）。

> Tokyo Demo Fest は日本で唯一のデモパーティです。 デモパーティは、コンピュータを用いたプログラミングとアートに 興味のある人々が日本中、世界中から一堂に会し、 デモ作品のコンペティションやセミナーなどを行います。 また、イベント開催中は集まった様々な人たちとの交流が深められます。 

今回が初参加でしたが、本当に最高のデモフェストでした！
オーガナイザーのみなさん、参加者のみなさん、ありがとうございました！！

全体のレポートについては、@h_doxas さんの記事がとても分かりやすいので、こちらを参考にしていただければと思います。

<blockquote class="twitter-tweet" data-lang="ja"><p lang="ja" dir="ltr">WebGL 総本山を更新しました ＞ 超ハイレベルな作品が入り乱れた Tokyo Demo Fest 2016！ 大興奮の２日間をレポート！ - WebGL 総本山 <a href="https://t.co/ZeYrYoLiz2">https://t.co/ZeYrYoLiz2</a> <a href="https://t.co/e3XFwpIrCD">pic.twitter.com/e3XFwpIrCD</a></p>&mdash; h_doxas (@h_doxas) <a href="https://twitter.com/h_doxas/status/701988774117376004">2016, 2月 23</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

この記事では、GLSL Graphics Compoで発表した"Carbon"という作品の裏話と、個人的な感想を振り返ります。

# Carbon 製作秘話

Compo（コンポ）とは、一定の制約の中で映像・音楽の作品を製作し、それを見ている人たちで投票し、ランキングを作るものです。

今年のGLSL Graphics Compoでは、[GLSL sandbox](http://glslsandbox.com/)上で動作するフラグメントシェーダだけで作られた映像作品のすごさを競いました。

私は"Carbon"というタイトルで作品を提出して3位入賞しました。
GLSL Graphics Compoは他のCompoと比較してもレベルが高かったので、入賞できて嬉しいです。

<blockquote class="twitter-tweet" data-lang="ja"><p lang="ja" dir="ltr">GLSL Compo に 「Carbon」という作品を出しました！<a href="https://t.co/UOqE3FvFyW">https://t.co/UOqE3FvFyW</a><a href="https://t.co/JxkH3LtI4t">https://t.co/JxkH3LtI4t</a><a href="https://twitter.com/hashtag/TokyoDemoFest?src=hash">#TokyoDemoFest</a> <a href="https://t.co/yfkJBzQllD">pic.twitter.com/yfkJBzQllD</a></p>&mdash; がむ@TDF最高だった (@gam0022) <a href="https://twitter.com/gam0022/status/701327225224736768">2016, 2月 21</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

- [Shadertoy - Carbon \[TDF2016\]](https://www.shadertoy.com/view/MsG3Wy)
- [GLSL sandbox - Carbon](http://glslsandbox.com/e#30972.0)

今回もレイマーチングによる作品です。

距離関数（distance function）は、Mandelbox というフラクタル図形を mod でループさせただけなので、非常にお手軽です。

この作品は大会中に頑張って製作しました。製作期間はなんと1日です！
20日のお昼くらいに作り始めて、20日は徹夜で作業し、21日の13:00の提出期限のギリギリに提出しました。
提出期限5分前くらいまでバグが取れずにあたふたしていたのですが、なんとか提出できて本当に嬉しかったです。

シェーダはデバックが難しいので、バグを取るのはけっこう大変です…
今回も同名の変数を異なるスコープで宣言しているという単純なミスで30分くらい無駄にしました。気をつけましょう…

先週の [#GLSLTech](http://gam0022.net/blog/2016/02/16/glsl-tech/)の打ち上げの飲み会の際に、Mandelbox というフラクタル図形という名前を聞きました。
Mandelbox で何か作品を作るということ、完成図のイメージはだいたい決まっていたので、そこまで出戻りなどもなく、1日で完成にこぎつけることができました。

# Mr.Doob
[three.js](http://threejs.org/)の作者であり、[GLSL sandbox](http://glslsandbox.com/)の作者でもある Mr.Doob 氏と記念撮影してもらいました！

<blockquote class="twitter-tweet" data-lang="ja"><p lang="ja" dir="ltr"><a href="https://twitter.com/mrdoob">@mrdoob</a> と記念撮影！ <a href="https://twitter.com/hashtag/TokyoDemoFest?src=hash">#TokyoDemoFest</a> <a href="https://t.co/j1xwSKNamz">pic.twitter.com/j1xwSKNamz</a></p>&mdash; がむ@TDF最高だった (@gam0022) <a href="https://twitter.com/gam0022/status/702292595486040064">2016, 2月 24</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

私は英語が怪しいので、あまりコミュニケーション取れませんでしたが、@yomotsuさんに助けていただきました。
@yomotsuさんみたいにかっこ良く英語話せるようになりたいと本気で思いましたｗ
