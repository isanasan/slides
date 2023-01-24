---
marp: true
theme: test
header: "**PHP Conf 2022**"
footer: "by **＠isanasan_**"
---
<!--
_class: title
paginate: true
-->
# 開発組織の生産性を可視化する

State of DevOpsとFour Keysとは
(増補改訂版)

---
<!--
class: slides
-->
<style scoped>
h1 {
  font-size: 500px;
  left: 300px;
}
</style>

# ⚠️

---
<style scoped>
h1 {
  color: black;
  font-size: 83px;
  top: 300px;
  left: 185px;
}
</style>

# hogehuga

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
<!--
_class: sanmoji
-->
# ゴール

---
<style scoped>
p {
    font-size: 90px;
    text-align: center;
}
</style>

# ゴール

開発組織とステークホルダー間の
共通言語を獲得する

---

# 課題
<!--
_class: jukugo
-->
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

# 説得失敗
<!--
_class: yojijukugo
-->

---
<style scoped>
h1 {
  color: black;
  font-size: 150px;
  top: 280px;
  text-align: center;
}
</style>

# 推測するな計測せよ

---
<style scoped>
h1 {
  color: black;
  font-size: 140px;
  top: 280px;
  text-align: center;
}
</style>

# そうだ、計測しよう💪

---
<style scoped>
h1 {
    color: orange;
    font-size: 135px;
    text-align: center;
    position: absolute;
    padding: 40px;
    top: 190px;
    left: 24px;
}
</style>

# State of DevOps

![bg 44% brightness:0.7 contrast:1.2](https://user-images.githubusercontent.com/58712884/173779572-40b2ad4d-f52e-485d-8bcf-1afa4fb20740.png)

---

# Stete of DevOpsとは

<style scoped>
li {
font-size: 47px;
padding: 17px;
}
</style>

- [DevOps Research and Assessment](https://www.devops-research.com/research.html)による調査
- デリバリの速度がビジネスに与える影響
- 開発とデリバリを高速化する方法

---
<!--
_footer: "https://www.devops-research.com/research.html"
-->
<style scoped>
li {
  font-size: 50px;
  padding: 30px;
}
footer {
  left: 400px;
}
</style>

# Stete of DevOpsとは

- レポートはGoogle Cloudのサイトから参照できる

---
<!--
_class: yojijukugo
-->

# 調査結果

---

# 調査結果

<style scoped>
li {
font-size: 50px;
padding: 17px;
}
</style>

- デリバリーの尺度を定義し定量化 = Four Keys
- デリバリを向上させる方法を特定 = Capabilities
- デリバリと組織のパフォーマンスの因果関係を立証

---
<!--
_class: sanmoji
-->
# さらに

---
<style scoped>
p {
  font-size: 86px;
  text-align: center;
}
</style>

デリバリのパフォーマンスと
品質の間に
**トレードオフは無い**ことを
つきとめた

---

# PIXTAのCTOやさいちさんのコメント

>技術の正しいことの実践っていうのが、
最終的な経営的な成果に繋がっているっていうのを示した
<texta.fm #5 by やさいち>

![height:250px](https://pixta.co.jp/assets/corporate/officers/y_gotou-c65c8e1ac375a17b0275cd3bb6b6a3065d1a4417e7fc6898e2ec57b516d21cd8.jpg)

---
<!--
_class: jukugo
-->

# 書籍

---

# 書籍 : LeanとDevOpsの科学

上述の調査結果に加えて
調査・研究手法を紹介、解説した書籍。

![bg left:40%](https://images-na.ssl-images-amazon.com/images/I/81VLedmhM5L.jpg)

---
<style scoped>
blockquote {
  margin: 1.5em 0;
  font-size: .95em;
}
</style>

# Martin Fowlerのコメント

>心から推薦できるITデリバリの測定手法の解説本
**-ひと握りの分析者のバラバラの体験談に基づいた本より遥かに優れた本-**
が誕生したのである。
<本書によせて by Martin Fowler>

![MartinFowler](https://user-images.githubusercontent.com/58712884/173469650-e9aaa294-0338-49f7-8875-1682f331bacb.jpg)

---
<style scoped>
h1 {
  color: black;
  font-size: 220px;
  text-align: center;
  position: absolute;
  top: 250px;
  left: 60px;
}
</style>

# Four Keys

---

# Four Keysとは

<style scoped>
p {
  font-size: 85px;
  text-align: center;
}
</style>

デリバリのパフォーマンスを測定する
4つの尺度

---
<!--
_class: number
-->

# (1)

---
<style scoped>
h1 {
  color: black;
  font-size: 240px;
  top: 190px;
  left: 40px;
}
</style>

# デプロイ頻度

---
<style scoped>
p {
  color: black;
  font-size: 120px;
  text-align: center;
}
</style>

コードの変更を
本番環境に適応して
稼動させる頻度

---
<!--
_class: number
-->

# (2)

---
<style scoped>
h1 {
  color: black;
  font-size: 280px;
  top: 160px;
  left: 40px;
}
</style>

# リードタイム

---
<style scoped>
p {
  font-size: 112px;
  text-align: center;
}
</style>

コードのコミットから
本番稼動までの
所要時間

---
<style scoped>
p {
  font-size: 70px;
}
</style>

⚠️開発ブランチのfirst commitから⚠️
⚠️デプロイされるまでの時間ではない⚠️

---
<!--
_class: number
-->

# (3)

---
<!--
_class: yojijukugo
-->

# MTTR

---
<style scoped>
p {
  color: black;
  font-size: 112px;
  text-align: center;
}
</style>

インシデント発生から
復旧にかかる平均時間

---
<!--
_class: number
-->

# (4)

---
<style scoped>
h1 {
  color: black;
  font-size: 240px;
  top: 230px;
  left: 40px;
}
</style>

# 変更失敗率

---
<style scoped>
p {
  font-size: 108px;
  text-align: center;
}
</style>

デプロイ起因で
本番障害が発生する割合

---
<style scoped>
li {
  font-size: 40px;
}
</style>

# Four Keys

## スピードのメトリクス

- デプロイ頻度
- リードタイム

## 品質のメトリクス

- MTTR
- 変更失敗率

---

# 品質とスピードにトレードオフは無い

> ハイパフォーマーは4つすべての尺度で計測結果が抜きん出ていた
p27 "調査結果から見えてきたもの" より

![width:200px](https://images-na.ssl-images-amazon.com/images/I/81VLedmhM5L.jpg)

---
<style scoped>
table {
  text-align: center;
}
table thead th {
  padding: 60px;
  padding-top: 20px;
  padding-bottom: 20px;
}
table td {
  font-size: 21px;
  padding: 27px;
}
</style>

| metric       | elite                 | high             | middle              | low            |
| ------------ | --------------------- | ---------------- | ------------------- | -------------- |
| デプロイ頻度 | オンデマンドに1日数回 | 1週間から月に1回 | 1ヶ月から6ヶ月に1回 | 6ヶ月に1回未満 |
| リードタイム | 1時間以内             | 1日から1週間     | 1ヶ月から6ヶ月      | 6ヶ月以上      |
| MTTR         | 1時間以内             | １日以内         | 1日から1週間        | 6ヶ月以上      |
| 変更失敗率   | 0~15%                 | 16%-30%          | 16%-30%             | 16%-30%        |

---
<!--
_footer: "https://tech.andpad.co.jp/entry/2022/03/08/110000"
-->
<style scoped>
footer {
  left: 400px;
}
li {
  font-size: 48px;
  padding: 30px;
}
</style>

# Four Keysの有用性

- 現場から遠い立場の人が現状を理解する助けになる
- 組織に合わせて指標の定義を拡張できる
- 指標をハックすることが難しい

---
<!--
_class: yojijukugo
-->
# ところで

---
<style scoped>
p {
  font-size: 108px;
  text-align: center;
}
</style>

State of DevOpsは
あくまでも学術的な研究と
その結果にすぎない

---
<style scoped>
p {
  font-size: 86px;
  text-align: center;
}
</style>

この知識を利用して
自分たちの利益に繋げていきたい

---
<style scoped>
h1 {
  color: black;
  font-size: 150px;
  top: 230px;
}
</style>

# 実際どうやんの？🤔

---
<style scoped>
li {
  font-size: 48px;
  padding: 30px;
}
</style>

# Four Keysの計測って実際どうやんの？

- SaaSを使う
- ツールを使う
- システムを自前で構築する

---
<style scoped>
li {
  font-size: 48px;
  padding: 30px;
}
</style>

# SaaSを使う

- Findy Teams
- LinearB

---
<!--
_footer: "https://findy-teams.com/"
-->
<style scoped>
footer {
  left: 490px;
}
</style>

# Findy Teams

![width:890px](https://pbs.twimg.com/media/Fb77142aQAIlJxm?format=png&name=large#center)

---
<!--
_footer: "https://linearb.io/"
-->
<style scoped>
footer {
  left: 530px;
}
</style>

# LinearB

![](https://linearb.io/wp-content/uploads/app-showcase-DORA-metrics.svg#center)

---
<style scoped>
li {
  font-size: 50px;
  padding: 5px;
}
</style>

# ツールを使う

- [hmiyado/four-keys](https://github.com/hmiyado/four-keys)
- [Trendyol/four-key](https://github.com/Trendyol/four-key)
- [GoogleCloudPlatform/fourkeys](https://github.com/GoogleCloudPlatform/fourkeys)
- [shibayu36/merged-pr-stat](https://github.com/shibayu36/merged-pr-stat)
- [isanasan/dmps](https://github.com/isanasan/dmps)

---

# システムを自前で構築する

![bg width:760px](../php_conf_2022_okinawa/diagram.drawio.svg)

---
<!--
_footer: "https://developer.hatenastaff.com/entry/2021/03/04/093000"
-->
<style scoped>
footer {
  left: 400px;
}
</style>

# システムを自前で構築する

![bg width:60%](https://user-images.githubusercontent.com/58712884/185623882-0f014bf4-3c2f-4800-98c3-ad3e75fc3bb9.png)

---
<!--
_footer: "https://github.com/isanasan/pull-request-analysis-sample"
-->
<style scoped>
footer {
  left: 350px;
}
</style>

# システムを自前で構築する

![bg width:800px](https://user-images.githubusercontent.com/58712884/185732166-d32e9ef2-a901-4ea8-9a84-9ebe517dfee3.png)

---
<style scoped>
li {
  font-size: 50px;
  padding: 5px;
}
</style>

# Four Keysはどうやって運用したらよいのか

- SREの指標と関連付けて運用する
- 財務諸表と関連付けて運用する
- 経営層を巻き込む

---
<!--
_footer: "[SREで開発を加速させる class SRE implements DevOps (WEB+DB PRESS Vol.129 株式会社技術評論社)](https://gihyo.jp/magazine/wdpress/archive/2022/vol129)"
-->
<style scoped>
p {
  text-align: center;
  font-size: 65px;
  padding: 10px;
}
footer {
  left: 230px;
}
</style>

# SREの指標と関連付けて運用する

デプロイ頻度 × 変更失敗率 × MTTR
= 変更起因障害の予想時間

---
<!--
_footer: "[SREで開発を加速させる class SRE implements DevOps (WEB+DB PRESS Vol.129 株式会社技術評論社)](https://gihyo.jp/magazine/wdpress/archive/2022/vol129)"
-->
<style scoped>
p {
  text-align: center;
  font-size: 45px;
  padding: 5px;
}
footer {
  left: 230px;
}
</style>

# SREの指標と関連付けて運用する

エラーバジェット × ウィンドウサイズ × 変更起因障害の割合
= 変更起因障害の許容時間

---
<!--
_footer: "[SREで開発を加速させる class SRE implements DevOps (WEB+DB PRESS Vol.129 株式会社技術評論社)](https://gihyo.jp/magazine/wdpress/archive/2022/vol129)"
-->
<style scoped>
p {
  font-size: 44px;
  text-align: center;
}
footer {
  left: 230px;
}
</style>

# SREの指標と関連付けて運用する

許容時間と予想時間を比較すれば改善のための議論ができる

---
<!--
_class: gomoji
-->
# 財務諸表🤔

---
<!--
_footer: "https://twitter.com/yamotty3/status/1342258793644617730?s=20&t=fHD6r1cAhRzfJf9De3-8jA"
-->
<style scoped>
footer {
  left: 230px;
}
</style>

# 財務諸表と関連付けて運用する

![width:840px](https://user-images.githubusercontent.com/58712884/191947289-9811d9e4-b239-45e2-abaa-3297a0ff783c.png#center)

---
<!--
_footer: "[texta.fm #6. 1on1 in Public](https://anchor.fm/textafm/episodes/6--1on1-in-Public-e1078pn)"
-->

<style scoped>
li {
  font-size: 40px;
  padding: 5px;
}
footer {
  left: 480px;
}
</style>

# 財務諸表と関連付けて運用する

- **PL(損益計算書)**
  - 企業の損失と利益を計算する表
- **BS(賃借対照表)**
  - 財産や残高、借入金などの一覧表

---
<!--
_footer: "[texta.fm #6. 1on1 in Public](https://anchor.fm/textafm/episodes/6--1on1-in-Public-e1078pn)"
-->
<style scoped>
footer {
  left: 480px;
}
</style>

# 財務諸表と関連付けて運用する

- **デプロイ頻度**
  - 人的資本の効率
  - デプロイ頻度を上げると資本を調達している訳ではないが資本効率が向上する
- **リードタイム**
  - 広義でみれば人権費や機会創出の指標
- **MTTR**
  - 売上そのものに関連する指標
- **変更失敗率**
  - 無価値なデプロイ = 人的資本の無駄使い

---
<!--
_footer: "[texta.fm #6. 1on1 in Public](https://anchor.fm/textafm/episodes/6--1on1-in-Public-e1078pn)"
-->
<style scoped>
table {
  margin: auto;
  margin-top: 0%;
  font-size: 50px;
}
footer {
  left: 480px;
}
</style>

# 財務諸表と関連付けて運用する

| 財務諸表                     | メトリクス                   |
| ---------------------------- | ---------------------------- |
| PL（損益計算書）             | リードタイム, MTTR |
| BS（貸借対照表）             | デプロイ頻度, 変更失敗率 |

---
<style scoped>
li {
  font-size: 40px;
  padding: 5px;
}
</style>

# 経営層を巻き込む

- 目標設定する(デプロイ頻度昨年度比2倍)
- 経営層が参加するMTGで進捗報告

---
<!--
_footer: "[「LeanとDevOpsの科学」を実践して LancersのDevOps的取り組みとこれから](https://speakerdeck.com/isanasan/lancers-devops-efforts-and-the-future)"
-->
<style scoped>
footer {
  left: 340px;
}
</style>

# 経営層を巻き込む

![width:900px](https://user-images.githubusercontent.com/58712884/189591645-2ec1f345-b6ff-4b30-9fa3-208e3f398dd1.png#center)

---
<!--
_class: jukugo
-->

# はい

---
<!--
_class: yojijukugo
-->
# 計測方法

---
<!--
_class: yojijukugo
-->
# わかった

---
<!--
_class: yojijukugo
-->
# 運用方法

---
<!--
_class: yojijukugo
-->
# わかった

---
<style scoped>
p {
  color: black;
  font-size: 120px;
  top: 230px;
}
</style>

Four Keysの改善って
実際どうやんの？🤔

---
<style scoped>
h1 {
  color: black;
  font-size: 113px;
  top: 280px;
}
</style>

# DevOps Capabilities

---
<style scoped>
p {
  color: black;
  font-size: 76px;
  text-align: center;
}
</style>

# DevOps Capabilitiesとは

Four Keysの改善効果が高いことが
特定されている組織の能力

---

# DevOps Capabilitiesとは

<style scoped>
li {
font-size: 48px;
padding: 17px;
}
</style>

- 4つのカテゴリーに分類されている。
- [Google Cloud](https://cloud.google.com/architecture/devops/capabilities?hl=ja)に詳しいドキュメントがある
- 継続的に更新されている(現在は27個)

---

# DevOps Capabilitiesとは

![width:1070px](https://user-images.githubusercontent.com/58712884/185543671-d50cd3e6-abb5-45e6-94cd-ab8fb54a301c.png#center)

---
<style scoped>
li {
  font-size: 48px;
  padding: 17px;
}
</style>

# DevOps Capabilities を実装していく

- どのようなアウトカムを得たいのかから逆算する
- ケイパビリティについても現状を可視化する
- ボトムアップでできることは現場に任せる

---
<!--
_footer: "https://www.devops-research.com/research.html"
-->
<style scoped>
  footer {
    left: 400px;
  }
</style>

# どのようなアウトカムを得たいのかから逆算する

![width:600px](https://user-images.githubusercontent.com/58712884/189790336-9bac6a1b-13eb-4f0c-b599-b6246120fe5a.png#center)

---
<!--
_footer: "[ファクトから始める改善アプローチ 〜「LeanとDevOpsの科学」を実践して〜](https://speakerdeck.com/tyankamo/huakutokarashi-merugai-shan-apuroti-leantodevopsfalseke-xue-woshi-jian-site)"
-->
<style scoped>
footer {
  left: 370px;
}
li {
  font-size: 48px;
  padding: 17px;
}
</style>

# ケイパビリティについても現状を可視化し実装する

- ケイパビリティは定量的だったり定性的だったりする
- サーベイを実施することでケイパビリティを可視化する

---
<style scoped>
li {
  font-size: 48px;
  padding: 17px;
}
</style>

# ボトムアップでできることは現場に任せる

- 勉強会を開催して啓蒙する
- チームで自立して実践できる項目はいくつかある
  - Value Streem Mapping
  - Trunk Base開発

---
<!--
_class: sanmoji
-->
# まとめ

---
<style scoped>
li {
  font-size: 44px;
  padding: 17px;
}
</style>

# まとめ

- Four Keysを計測して開発組織の生産性を可視化しよう
- いろんな観点からFour Keysを運用しよう
- DevOps Capabilitiesを実装して改善しよう

---
<!--
_class: sanmoji
-->
# 最後に

---
<style scoped>
blockquote {
  margin: 1.5em 0;
  font-size: 41px;
}
</style>

# 最後に

>組織を変えようと思ったら上からも下からも変えなきゃいけない。
<名無しさんのポッドキャスト #9 by ryuzee>

![width:200px](https://www.ryuzee.com/images/th_ryuzee002.png)

---
<style scoped>
h1 {
  color: black;
  font-size: 121px;
  top: 140px;
  text-align: center;
  left: 5px;
}
</style>

# トップダウンとボトムアップ両方から改善していこう💪

---

# 参考文献

[エリート DevOps チームであることを Four Keys プロジェクトで確認する](https://cloud.google.com/blog/ja/products/gcp/using-the-four-keys-to-measure-your-devops-performance)
[DevOpsの能力](https://cloud.google.com/architecture/devops/capabilities?hl=ja)
[Findy Teamsの指標を使ってチームの生産性を改善しよう](https://tech.andpad.co.jp/entry/2022/01/06/110000)
[エンジニアの活動情報からFour Keysを集計、可視化した話](https://tech.pepabo.com/2022/01/06/four-keys-dashboard/)
[SREで開発を加速させる class SRE implements DevOps (WEB+DB PRESS Vol.129 株式会社技術評論社)](https://gihyo.jp/magazine/wdpress/archive/2022/vol129)
[Mackerel開発チームのリードSREが考える働き方と組織作り](https://speakerdeck.com/masayoshi/developers-summit-2021-summer?slide=34)
[ファクトから始める改善アプローチ 〜「LeanとDevOpsの科学」を実践して〜](https://speakerdeck.com/tyankamo/huakutokarashi-merugai-shan-apuroti-leantodevopsfalseke-xue-woshi-jian-site?slide=49)
[texta.fm #5. Accelerate](https://anchor.fm/textafm/episodes/5--Accelerate-ethnjo)
[texta.fm #6. 1on1 in Public](https://anchor.fm/textafm/episodes/6--1on1-in-Public-e1078pn)
