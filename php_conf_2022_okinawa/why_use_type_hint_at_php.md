---
marp: true
theme: test
header: "**PHP Conf 沖縄 2022**"
footer: "by **＠isanasan_**"
---
<!--
_class: title
paginate: true
-->
# 今あらためて考える

PHPに型定義をする理由

---

# 自己紹介
<!--
_class: yojijukugo
-->

<!--
class: slides
-->

---

![bg right:40%](https://user-images.githubusercontent.com/58712884/173713399-6a892196-1c13-4a44-b794-7fddd12bd431.jpg)

# いさな

- Lancersプロダクト開発部QAチーム
- CakePHPのバージョンアップを担当
- DevOpsに興味関心がある

![width:50px](https://user-images.githubusercontent.com/58712884/174742561-aadf80cc-d24d-488e-bebd-f33a8aa88de3.png) @isanasan_

![width:50px](https://user-images.githubusercontent.com/58712884/174749360-e1b1e941-8d14-4eeb-9ad9-610c12ff3176.png) @isanasan

![width:50px](https://user-images.githubusercontent.com/58712884/174750050-566537de-fabe-4a04-8b47-c14fd6b2dcae.png) @isana

---
<style scoped>
h1 {
    color: black;
    font-size: 63px;
    padding: 40px;
    top: 250px;
    left: 40px;
}
</style>

# 最近PHPの型が注目されている気がする

---
<style scoped>
h1 {
    color: black;
    font-size: 86px;
    padding: 40px;
    top: 250px;
    left: 40px;
}
</style>

# 直近の主要なカンファレンス

---
<style scoped>
h1 {
    color: black;
    font-size: 120px;
    padding: 40px;
    top: 250px;
    left: 40px;
}
</style>

# PHPer Kaigi 2022

---
<!--
_footer: "https://fortee.jp/phperkaigi-2022/proposal/38060a2f-cef3-438a-822a-044de1799bc2"
-->
<style scoped>
footer {
  left: 250px;
}
</style>

![](https://fortee.jp/phperkaigi-2022/proposal/og-image/38060a2f-cef3-438a-822a-044de1799bc2.png)

---
<!--
_footer: "https://fortee.jp/phperkaigi-2022/proposal/7a340d9f-1f46-4f72-9886-a5f599eeac1c"
-->
<style scoped>
footer {
  left: 250px;
}
</style>

![](https://fortee.jp/phperkaigi-2022/proposal/og-image/7a340d9f-1f46-4f72-9886-a5f599eeac1c.png)

---
<style scoped>
h1 {
    color: black;
    font-size: 140px;
    padding: 40px;
    top: 250px;
    left: 40px;
}
</style>

# PHP Conf 2021

---
<!--
_footer: "https://fortee.jp/phpcon-2021/proposal/a7e53ddb-09fd-404e-bb90-b5047e8994ab"
-->
<style scoped>
footer {
  left: 250px;
}
</style>

![](https://fortee.jp/phpcon-2021/proposal/og-image/a7e53ddb-09fd-404e-bb90-b5047e8994ab.png)

---
<style scoped>
h1 {
    color: black;
    font-size: 54px;
    padding: 40px;
    top: 250px;
    left: 40px;
}
</style>

# 最近PHPの静的解析も注目されている気がする

---
<style scoped>
h1 {
    color: black;
    font-size: 86px;
    padding: 40px;
    top: 250px;
    left: 40px;
}
</style>

# 直近の主要なカンファレンス

---
<style scoped>
h1 {
    color: black;
    font-size: 140px;
    padding: 40px;
    top: 250px;
    left: 40px;
}
</style>

# PHP Conf 2021

---
<!--
_footer: "https://fortee.jp/phpcon-2021/proposal/49dd21f3-769d-4170-a9a9-b1f18c4e1135"
-->
<style scoped>
footer {
  left: 250px;
}
</style>

![](https://fortee.jp/phpcon-2021/proposal/og-image/49dd21f3-769d-4170-a9a9-b1f18c4e1135.png)

---
<!--
_footer: "https://fortee.jp/phpcon-2021/proposal/b9a17925-8800-4415-9676-99a1e24d181d"
-->
<style scoped>
footer {
  left: 250px;
}
</style>

![](https://fortee.jp/phpcon-2021/proposal/og-image/b9a17925-8800-4415-9676-99a1e24d181d.png)

---
<style scoped>
h1 {
    color: black;
    font-size: 120px;
    padding: 40px;
    top: 250px;
    left: 40px;
}
</style>

# PHPer Kaigi 2021

---
<!--
_footer: "https://fortee.jp/phperkaigi-2021/proposal/35177e2b-189c-43c2-ad29-e74caf5033e7"
-->
<style scoped>
footer {
  left: 250px;
}
</style>

![](https://fortee.jp/phperkaigi-2021/proposal/og-image/35177e2b-189c-43c2-ad29-e74caf5033e7.png)

---
<style scoped>
h1 {
    color: black;
    font-size: 140px;
    padding: 40px;
    top: 250px;
    left: 40px;
}
</style>

# JetBrainsの調査

---
<!--
_footer: "https://www.jetbrains.com/ja-jp/lp/devecosystem-2019/php/ \nhttps://www.jetbrains.com/ja-jp/lp/devecosystem-2020/php/ \nhttps://www.jetbrains.com/ja-jp/lp/devecosystem-2021/php/"
-->
<style scoped>
footer {
  left: 350px;
}
table {
  text-align: center;
}

table thead th {
  font-size: 42px;
  padding-left: 55px;
  padding-right: 55px;
}

table td {
  font-size: 42px;
  padding: 21px;
}
</style>

# どんな品質ツールを使っていますか？

|      | PHPstan | Phan | Psalm | 合計 |
| ---- | ----------- | ---- | --------- | ---- |
| 2019 | 9%          | 5%   | 1%        | 15%  |
| 2020 | 11%         | 2%   | 3%        | 16%  |
| 2021 | 18%         | 2%   | 9%        | 29%  |

---
<!--
_footer: "https://www.jetbrains.com/ja-jp/lp/devecosystem-2021/php/#PHP_do-you-use-static-analysis"
-->
<style scoped>
footer {
  left: 250px;
}
table {
  text-align: center;
}

table thead th {
  font-size: 68px;
  padding-left: 55px;
  padding-right: 55px;
}

table td {
  font-size: 68px;
  padding: 21px;
}
</style>

# 静的解析を使用していますか？

| はい | いいえ | 静的解析 is 何 |
| ---- | ------ | -------------- |
| 33%  | 38%    | 28%            |

---
<style scoped>
h1 {
    color: black;
    font-size: 57px;
    padding: 40px;
    top: 250px;
    left: 40px;
}
</style>

# 最近PHPの型の表現力が上っている気がする

---

# 7.0

<style scoped>
li {
font-size: 48px;
padding: 17px;
}
</style>

- Scalar type hints

---

# 7.1

<style scoped>
li {
font-size: 48px;
padding: 17px;
}
</style>

- Nullable Types
- Void Return Type

---

# 7.4

<style scoped>
li {
font-size: 48px;
padding: 17px;
}
</style>

- Typed Property

---

# 8.0

<style scoped>
li {
font-size: 48px;
padding: 17px;
}
</style>

- Union Types

---

# 8.1

<style scoped>
li {
font-size: 48px;
padding: 17px;
}
</style>

- Pure intersection type
- Enumerations
- noreturn type

---
<!--
_class: jukugo
-->

# はい

---
<style scoped>
li {
  font-size: 48px;
  padding: 17px;
}
</style>

- 最近PHPの型が注目されている
- 最近静的解析が注目されている
- PHPの型の表現力が序々に高まっている

---
<style scoped>
h1 {
    color: black;
    font-size: 93px;
    padding: 40px;
    top: 250px;
    left: 40px;
}
</style>

# だがちょっと待って欲しい

---
<style scoped>
h1 {
    color: black;
    font-size: 93px;
    padding: 40px;
    top: 250px;
    left: 40px;
}
</style>

# PHPは弱い動的型付け言語

---
<style scoped>
li {
  font-size: 48px;
  padding: 17px;
}
</style>

# PHPは弱い動的型付け言語

- 型は実行時に決定される
- 型は文脈に応じて暗黙的に変換される

---
<!--
_class: yojijukugo
-->
# 要するに

---
<style scoped>
h1 {
    color: black;
    font-size: 110px;
    padding: 40px;
    top: 250px;
    left: 40px;
}
</style>

# 型を書かなくても動く

---
<style scoped>
h1 {
    color: black;
    font-size: 66px;
    padding: 40px;
    top: 250px;
    left: 40px;
}
</style>

# わざわざ型書いて静的解析ナンデ？？

---
<!--
_class: title
paginate: true
-->
# 今あらためて考える

PHPに型定義をする理由

---
<!--
_class: title
paginate: true
-->
# 今あらためて考える

PHPに型定義(静的解析)をする理由

---
<style scoped>
h1 {
    color: black;
    font-size: 240px;
    padding: 40px;
    top: 250px;
    left: 40px;
}
</style>

# 3つの観点

---
<style scoped>
li {
  font-size: 48px;
  padding: 17px;
}
</style>

# 3つの観点

- フィードバックサイクル
- コーディングの生産性
- コードベースのメンテナンス性

---
<!--
_class: yojijukugo
-->
# その前に

---
<style scoped>
h1 {
    color: black;
    font-size: 190px;
    padding: 40px;
    top: 250px;
    left: 40px;
}
</style>

# 静的解析とは

---
<style scoped>
li {
  font-size: 48px;
  padding: 17px;
}
</style>

# 静的解析とは

- コードを実行せずに問題点等を検出すること
- コードを実行しないため高速
- ツールを導入するだけで実行できる

---
<style scoped>
h1 {
    color: black;
    font-size: 100px;
    padding: 40px;
    top: 250px;
    left: 40px;
}
</style>

# フィードバックサイクル

---

# 不具合の発見が早いほど修正は低コスト

<!--
_footer: "https://www.luxoft-training.com/news/7-principles-of-testing-part-2/"
-->
<style scoped>
footer {
  left: 350px;
}
</style>

![bg 46% contrast:1.2](https://www.luxoft-training.com/upload/medialibrary/537/fixing_defect.jpg)

---
<style scoped>
h1 {
    color: black;
    font-size: 110px;
    padding: 40px;
    top: 250px;
    left: 40px;
}
</style>

# バグは早く見つけたい

---
<!--
_class: jukugo
-->

# 再掲

---
<style scoped>
li {
  font-size: 48px;
  padding: 17px;
}
</style>

# 静的解析とは

- コードを実行せずに問題点等を検出すること
- コードを実行しないため高速
- ツールを導入するだけで実行できる

---
<style scoped>
li {
  font-size: 48px;
  padding: 17px;
}
</style>

# つまり

- UTより実行・導入が低コスト
- UTより早いフィードバックが得られる
- UTより修正が容易

---
<style scoped>
h1 {
    color: black;
    font-size: 110px;
    padding: 40px;
    top: 250px;
    left: 40px;
}
</style>

# コーディングの生産性

---
<style scoped>
h1 {
    color: black;
    font-size: 66px;
    padding: 40px;
    top: 250px;
    left: 40px;
}
</style>

# エディタによるサポートを受けられる

---

# エディタによるサポートを受けられる

<style scoped>
li {
  font-size: 48px;
  padding: 5px;
}
</style>

- 定義ジャンプ
- ホバー表示
- 補完
- インスペクション

---
<style scoped>
h1 {
    color: black;
    font-size: 100px;
    padding: 40px;
    top: 250px;
    left: 40px;
}
</style>

# コードのメンテナンス性

---
<style scoped>
h1 {
    color: black;
    font-size: 120px;
    padding: 40px;
    top: 250px;
    left: 40px;
}
</style>

# メンテナンス性とは

---
<style scoped>
h2 {
    color: black;
    font-size: 80px;
    padding: 40px;
    top: 250px;
    left: 40px;
}
</style>

# メンテナンス性とは

## SQuaRE(JIS X 25010)

---

# メンテナンス性とは

<!-- 
_footer: "https://www.ipa.go.jp/sec/reports/20150331_1.html"
-->
<style scoped>
footer {
  left: 350px;
}
</style>

![bg 64% contrast:1.2](https://user-images.githubusercontent.com/58712884/184537577-886522dd-a880-47e9-9c60-4acbe505a7c4.jpg)

---
<style scoped>
li {
  font-size: 48px;
  padding: 4px;
}
</style>

# メンテナンス性とは

- モジュール性(modularity)
- 再利用性(reusability)
- 解析性(analysability)
- 修正性(modifiability)
- 試験性(testability)

---
<style scoped>
li {
  font-size: 48px;
  padding: 4px;
}
</style>

# メンテナンス性とは

- モジュール性(modularity)
- 再利用性(reusability)
- 🚩**解析性(analysability)**
- 🚩**修正性(modifiability)**
- 試験性(testability)

---
<style scoped>
h1 {
    color: black;
    font-size: 65px;
    padding: 40px;
    top: 250px;
    left: 40px;
}
</style>

# 解析性(analysability) ≒ 理解容易性

---
<style scoped>
h2 {
    color: black;
    font-size: 105px;
    padding: 40px;
    top: 250px;
    left: 40px;
}
</style>

# 解析性(analysability) ≒ 理解容易性

## 型定義有 > 型定義無

---
<style scoped>
h1 {
    color: black;
    font-size: 65px;
    padding: 40px;
    top: 250px;
    left: 40px;
}
</style>

# 解析性(analysability) ≒ 理解容易性

---

# 解析性(analysability) ≒ 理解容易性

![bg 20% contrast:1.2](https://pic.sopili.net/pub/emoji/noto-emoji/png/128/emoji_u1f646_200d_2642.png)

---
<style scoped>
h1 {
    color: black;
    font-size: 140px;
    padding: 40px;
    top: 250px;
    left: 40px;
}
</style>

# リファクタリング

---
<style scoped>
li {
  font-size: 48px;
  padding: 4px;
}
</style>

# リファクタリング

- IDEやエディタによるリファクタリング
- Rectorによるリファクタリング

---
<style scoped>
h1 {
    color: black;
    font-size: 160px;
    padding: 40px;
    top: 250px;
    left: 40px;
}
</style>

# 別言語への移植

---
<style scoped>
li {
  font-size: 48px;
  padding: 17px;
}
</style>

# 別言語への移植

- Scalaに移植するゾイ
- 型が分からないから移植しようがないゾイ

---
<style scoped>
h1 {
    color: black;
    font-size: 100px;
    padding: 40px;
    top: 250px;
    left: 40px;
}
</style>

# 修正性(modifiability)

---

# 修正性(modifiability)

![bg 20% contrast:1.2](https://pic.sopili.net/pub/emoji/noto-emoji/png/128/emoji_u1f646_200d_2642.png)

---
<style scoped>
li {
  font-size: 48px;
  padding: 17px;
}
</style>

# まとめ

- バグの早期発見に役立つ
- エディタの便利機機が使える
- 解析性と修正性が向上する

---

# 参考文献

[組織にテストを書く文化を根付かせる戦略と戦術（2020秋版）](https://speakerdeck.com/twada/strategy-and-tactics-of-building-automated-testing-culture-into-organization-2020-autumn-edition)

[PHPStanで始めるPHPのための静的解析](https://engineering.mercari.com/blog/entry/phpstan/)

[エディタ中中なPHP開発環環の現在](https://www.youtube.com/watch?v=LA6ZH_GdzNI&list=PLx8bw5NQypsnlh5K5LZAaFvAdxfGpt2iq&index=8)

[アジリティを支える品質特性](https://speakerdeck.com/twada/agility-and-quality-characteristics-developers-summit-2021-summer)
