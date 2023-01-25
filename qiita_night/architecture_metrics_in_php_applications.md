---
marp: true
theme: test
header: "**Qiita Night PHP**"
footer: "by **＠isanasan_**"
---
<!--
_class: title
paginate: true
-->
<style scoped>
h1 {
    font-size: 103px;
}
h2 {
    font-size: 101px;
}
</style>

# PHPアプリケーションにおける

## アーキテクチャメトリクスについて

---
<!--
class: slides
-->

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

- Lancers Productivity Team
- DevOpsに興味関心がある

![width:50px](https://user-images.githubusercontent.com/58712884/174742561-aadf80cc-d24d-488e-bebd-f33a8aa88de3.png) @isanasan_

![width:50px](https://user-images.githubusercontent.com/58712884/174749360-e1b1e941-8d14-4eeb-9ad9-610c12ff3176.png) @isanasan

![width:50px](https://user-images.githubusercontent.com/58712884/174750050-566537de-fabe-4a04-8b47-c14fd6b2dcae.png) @isana

---

<!--
_class: sanmoji
-->
# 対象者

---

<style scoped>
li {
    font-size: 80px;
    padding: 17px;
}
</style>

# 対象者

- 負債に苦しむエンジニア
- テックリード
- プレイングマネージャー

---
<style scoped>
h1 {
    color: black;
    font-size: 116px;
    top: 250px;
}
</style>

# アーキテクチャメトリクスとは

---
<style scoped>
p {
    font-size: 60px;
    text-align: center;
}
</style>

# アーキテクチャメトリクスとは

アーキテクチャの**保守性**を測定するための指標

---
<style scoped>
h1 {
    color: black;
    font-size: 268px;
    top: 210px;
}
</style>

# 保守性とは

---
<style scoped>
p {
    color: black;
    font-size: 69px;
    top: 210px;
}
</style>

# 保守性とは

システム/ソフトウェア製品品質(SQuaRE)

---
<!-- 
_footer: "https://www.ipa.go.jp/sec/reports/20150331_1.html"
-->
<style scoped>
footer {
  left: 350px;
}
</style>

# システム/ソフトウェア製品品質(SQuaRE)

![bg 64% contrast:1.2](https://user-images.githubusercontent.com/58712884/184537577-886522dd-a880-47e9-9c60-4acbe505a7c4.jpg)

---
<style scoped>
p {
    font-size:47px;
}
li {
    font-size: 40px;
}
</style>

# つまりアーキテクチャメトリクスとは

以下の項目が今どのくらいヤバいのかを数字で示すためのもの

- モジュール性
- 再利用性
- 理解容易性
- 修正性
- テスト容易性

---
<style scoped>
h1 {
    color: black;
    font-size: 310px;
    top: 190px;
    left: 270px;
}
</style>

# 🤨??

---
<style scoped>
h1 {
    color: black;
    font-size: 150px;
    top: 250px;
}
</style>

# 具体的なユースケース

---
<style scoped>
h1 {
    font-size: 230px;
    color: black;
    left: 50px;
    top: 200px;
}
</style>

# とあるサービス

---
<style scoped>
h2 {
    font-size: 114px;
    color: yellow;
    position: absolute;
    right: 50px;
}
</style>

## 疲弊した現場

![bg  brightness:0.6](https://user-images.githubusercontent.com/58712884/173767094-d3f3d09f-22cc-4b65-b0dd-21361cb1d28f.jpg)

---
<style scoped>
h2 {
    font-size: 114px;
    color: red;
    left: 50px; top: 90px;
}
</style>

## 荒みきったコード

![bg  brightness:0.6](https://user-images.githubusercontent.com/58712884/173759585-bf7a055c-34ed-41f4-ac0a-258736c24a4a.jpg)

---
<style scoped>
h2 {
    font-size: 90px;
    color: orange;
    position: absolute;
    left: 210px;
    top: 600px;
}
</style>

## 爆弾処理のようなリリース

![bg brightness:0.6](https://user-images.githubusercontent.com/58712884/173769334-6ddc7144-189c-4d7b-a21b-6bf05172023d.jpg)

---
<style scoped>
h2 {
    font-size: 90px;
    color: white;
    position: absolute;
    left: 260px;
    top: 300px;
}
</style>

## 改善したい!!!!!!!

![bg brightness:0.6](https://user-images.githubusercontent.com/58712884/173770554-1b314375-1db5-4a2c-8b4f-6a42b94c57b3.jpg)

---
<style scoped>
ul {
    font-size: 50px;
    color: white;
    position: absolute;
    left: 150px;
}
</style>

![bg brightness:0.6](https://user-images.githubusercontent.com/58712884/173771682-83ba9c8b-6451-46b3-834c-c5d753a3b1be.jpg)

- 今動いているものを直す必要ある？
- 効果測定どうやんの？
- 費用対効果はどれくらい？

---
<!--
_class: yojijukugo
-->

# 説得失敗

---
<style scoped>
h1 {
    font-size: 160px;
    color: black;
    top: 250px;
}
</style>

# 改善の黄金パターン

---
<style scoped>
li {
    font-size: 45px;
    left: 150px;
}
</style>

# 改善の黄金パターン

1. 課題を認識する
2. 課題を定量化できるメトリクス(指標)を定義し目標を決める
3. 改善施策を実施する
4. 振り返りを行う

---
<style scoped>
h1 {
    font-size: 107px;
    color: black;
    top: 290px;
}
</style>

# ソフトウェア開発の現場では?

---
<style scoped>
li {
    font-size: 56px;
    color: black;
}
</style>

# ソフトウェア開発の現場では?

- もちろんソフトウェア開発の現場でも考え方は同じ
- 特に「正確な現状把握」は必要不可欠
- パフォーマンスチューニングはその代表的な例

---
<style scoped>
h1 {
    font-size: 79px;
    color: black;
    top: 290px;
}
</style>

# アーキテクチャの保守性を改善する時は?

---
<style scoped>
h1 {
    font-size: 125px;
    color: orange;
    top: 290px;
}
</style>
<!-- _backgroundColor: "#696969" -->
# コードスメル(不吉な匂い)

![bg 35% brightness:0.6](https://m.media-amazon.com/images/I/41+4LYE83XL._SX383_BO1,204,203,200_.jpg)

---
<style scoped>
li {
    font-size: 51px;
}
</style>

# コードスメルの欠点

- 定性的指標(≒ 暗黙知)
  - 経験値に依存する
- 効果測定や優先順位付けが難しい
- 対外的な説明には使えない

---
<!--
_class: jukugo
-->
# 再掲

---
<style scoped>
li {
    font-size: 45px;
    left: 150px;
}
</style>

# 改善の黄金パターン

1. 課題を認識する
2. 課題を定量化できるメトリクス(指標)を定義し目標を決める
3. 改善施策を実施する
4. 振り返りを行う

---

<style scoped>
li {
    font-size: 45px;
}
</style>

# 改善の黄金パターン

1. 課題を認識する
   - 👆コードスメル
2. 課題を定量化できるメトリクス(指標)を定義し目標を決める
3. 改善施策を実施する
4. 振り返りを行う

---

<style scoped>
li {
    font-size: 45px;
}
</style>

# 改善の黄金パターン

1. 課題を認識する
2. 課題を定量化できるメトリクス(指標)を定義し目標を決める
    - 👆アーキテクチャメトリクス
3. 改善施策を実施する
4. 振り返りを行う

---
<style scoped>
h1 {
    font-size: 100px;
    color: orange;
    top: 290px;
}
</style>

# 定性的指標から定量的指標へ

![bg brightness:0.7](https://images.unsplash.com/photo-1567916190725-372c28edc554?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1170&q=80)

---
<!-- _class: jukugo <-->
# 利点

---
<style scoped>
li {
    font-size: 50px;
}
</style>

# 利点

- コードスメルのような暗黙知を形式知にすることが出来る
- 効果測定を行うことでフィードバックサイクルを回せる
- 測定基準を設けることで負債を未然に防ぐ

---
<style scoped>
h1 {
    font-size: 155px;
    color: black;
    top: 270px;
}
</style>

# 代表例と測定ツール

---
<style scoped>
li {
    font-size: 80px;
}
</style>

# 代表例と測定ツール

- 理解容易性に関連するメトリクス
- テスト容易性に関連するメトリクス
- その他

---
<style scoped>
li {
    font-size: 40px;
}
</style>

# 理解容易性に関連するメトリクス

- 循環的複雑度(CCN)
  - 要するに分岐の数
  - 24以上の値ではエラーレートが急速に増加すると言われている
  - 加重平均を用いることで時系列推移を計測できる

---
<style scoped>
li {
    font-size: 43px;
}
</style>

# PHPの循環的複雑度を計測するツール

- [bmitch/churn-php](https://github.com/bmitch/churn-php)
  - 変更頻度で重み付けしたCCNのスコアを計測するツール

---

# churn-php

![churn_php_output](https://user-images.githubusercontent.com/58712884/214484097-c0f3223b-665c-4355-9555-9633cfd12a44.png)

---
<style scoped>
li {
    font-size: 50px;
}
</style>

# PHPの循環的複雑度を計測するツール

- [terryyin/lizard](https://github.com/terryyin/lizard)
  - CCNを含む複数の指標で複雑さを計測するツール
  - 行数、CCN、token、引数の数を計測してくれる
  - 出力形式にxmlやhtmlを選べる

---

# lizard

```bash
==============================================================
  NLOC    CCN  token  param    function@line@file
--------------------------------------------------------------
    10      2     29      2    start_new_player@26@./html_game.c
```

---
<style scoped>
li {
    font-size: 60px;
}
</style>

# テスト容易性に関連するメトリクス

- テストカバレッジ
- テストコードとプロダクトコードの割合
- テストの実行時間

---
<style scoped>
li {
    font-size: 47px;
}
</style>

# テスト容易性を計測するツール

- [k1LoW/octocov](https://github.com/k1LoW/octocov)
  - カバレッジ、コードの割合、実行時間を全て計測できる
  - CIフレンドリー
  - PRにコメントしたり
  - 複数リポジトリの数値を収集したりできる

---

# octocov

![width:1000px](https://user-images.githubusercontent.com/58712884/214485276-e46193c6-7d62-4350-b78e-cb30054523f8.png)

---
<style scoped>
li {
    font-size: 48px;
}
</style>

# テスト容易性を計測するツール

- [edsonmedina/php_testability](https://github.com/edsonmedina/php_testability)
  - 密結合になっている箇所(new演算子とか)を数えてテスト容易性のリストを出力できる
  
---

# php_testability

![width:800px](https://camo.githubusercontent.com/f48262da1ae1d4dc41e5dea62b8469c3661405e7aac43c0a8029164d2ea057ae/687474703a2f2f7777772e6369616e65746f2e636f6d2f746573746162696c6974795f6469722e706e67)

---

# その他のもの

- 変更頻度と変更人数
  - あまりにも多くの人が頻繁に変更を加えるソースは責務が大きすぎる可能性がある
  - churn-php もこれで循環的複雑度を重み付けしている
- PRのリードタイム
  - `アーキテクチャ`のメトリクスとは言えないが、アーキテクチャメトリクスの遅行指標として扱える
  - 例えば,「理解容易性が悪化すればPRのリードタイムは伸びる」みたいな

---
<!--
_class: sanmoji
-->
# 最後に

---
<style scoped>
h1 {
    font-size: 74px;
    color: black;
    top: 300px;
}
</style>

# アーキテクチャメトリクスはめっちゃ種類ある

---
<style scoped>
li {
    font-size: 48px;
}
</style>

# アーキテクチャメトリクスはめっちゃ種類ある

- 累積コンポーネント依存度(CCD)  
- 平均コンポーネント依存度(ACD)
- 伝搬コスト(PC)
- 相対循環依存度(RC)
- 構造的負債指数(SDI)

---
<style scoped>
h1 {
    font-size: 85px;
    color: black;
    top: 300px;
}
</style>

# 現場によって抱えている課題は異なる

---
<style scoped>
h1 {
    font-size: 88px;
    color: black;
    top: 300px;
}
</style>

# あなただけのメトリクスを見つけよう

---
<style scoped>
h1 {
    font-size: 100px;
    color: black;
    top: 300px;
}
</style>

# PHPで使えるツールも沢山ある

---

# PHPで使えるツールも沢山ある

- [exakat/php-static-analysis-tools](https://github.com/exakat/php-static-analysis-tools)
  - このリポジトリにまとまっている
  - メンテされなくなったものも紛れてるので注意
- [DeGraciaMathieu/php-arguments-detector](https://github.com/DeGraciaMathieu/php-arguments-detector)
  - 引数が多すぎないかどうかをチェックするツール
- [phpmetrics/PhpMetrics](https://github.com/phpmetrics/PhpMetrics)
  - 結構色々取れるツール。
  - 結果がHTMLでしか出力できないのでCIと組み合わせたりするのはちょっと手間
  
---
<style scoped>
h1 {
    font-size: 84px;
    color: black;
    top: 300px;
}
</style>

# 測りたい指標を決めたら探してみよう

---
<!--
_class: sanmoji
-->

# まとめ

---
<style scoped>
li {
    font-size: 46px;
}
</style>

# まとめ

- 保守性を改善するときはアーキテクチャメトリクスを計測しよう
- 現場の課題に合ったメトリクスを見つけよう
- PHPの現場で使えるツールは沢山あるので探してみよう
