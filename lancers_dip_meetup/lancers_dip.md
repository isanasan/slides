---
marp: true
theme: test
header: "**Lancers × dip**"
footer: "by **＠isanasan_**"
---
<!--
_class: title
paginate: true
-->
# 開発組織の生産性を可視化する

State of DevOpsとFour Keysとは

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

# 三宅 勇魚

- Lancersプロダクト開発部QAチーム
- CakePHPのバージョンアップを担当
- DevOpsに興味関心がある

![width:50px](https://user-images.githubusercontent.com/58712884/174742561-aadf80cc-d24d-488e-bebd-f33a8aa88de3.png) @isanasan_

![width:50px](https://user-images.githubusercontent.com/58712884/174749360-e1b1e941-8d14-4eeb-9ad9-610c12ff3176.png) @isanasan

![width:50px](https://user-images.githubusercontent.com/58712884/174750050-566537de-fabe-4a04-8b47-c14fd6b2dcae.png) @isana

---

# 本題
<!--
_class: jukugo
-->

---

# その前に
<!--
_class: yojijukugo
-->

---

# 課題
<!--
_class: jukugo
-->
---
<style scoped>
h1 {
    font-size: 170px;
    color: black;
    left: 50px;
    top: 250px;
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
    left: 100px;
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
    font-size: 240px;
    color: black;
    top: 250px;
}
</style>

# と言う訳で

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

# モチベーション

---
<style scoped>
li {
font-size: 50px;
padding: 30px;
}
</style>

- 推測するな計測せよ
- 開発組織の生産性についても同じでは？
- 生産性を定義してモニタリングしよう

---
<style scoped>
h1 {
    color: orange;
    font-size: 136px;
    text-align: center;
    position: absolute;
    padding: 40px;
    top: 250px;
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
_class: jukugo
-->
# 余談

---
<style scoped>
li {
font-size: 50px;
padding: 30px;
}
</style>

- DORAは後にGoogleが買収した
- 2021年のレポートも[公開](https://cloud.google.com/blog/ja/products/devops-sre/announcing-dora-2021-accelerate-state-of-devops-report)されている

---
<!--
_class: yojijukugo
-->

# 調査結果

---

# 調査結果

<style scoped>
li {
font-size: 48px;
padding: 17px;
}
</style>

- ソフトウェアデリバリーの尺度を定義し定量化
- デリバリーとビジネスの因果関係が判明
- デリバリを向上させるケイパビリティを特定

---
<style scoped>
h1 {
  color: black;
  font-size: 360px;
  text-align: center;
  padding: 60px;
}
</style>

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

<!--
_class: jukugo
-->

# 解説

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
  color: black;
  font-size: 84px;
  text-align: center;
  margin: 10px;
  top: 250px;
}
</style>

デリバリのパフォーマンスを測定する4つの尺度

---
<!--
_class: number
-->

# (1)

---
<style scoped>
h1 {
  color: black;
  font-size: 200px;
  top: 230px;
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
  font-size: 200px;
  top: 230px;
  left: 40px;
}
</style>

# リードタイム

---
<style scoped>
p {
  color: black;
  font-size: 112px;
  text-align: center;
}
</style>

コードのコミットから
本番稼動までの
所要時間

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
  color: black;
  font-size: 140px;
  text-align: center;
}
</style>

不具合が発生する
リリースの確率

---

# 品質とスピードにトレードオフは無い

> ハイパフォーマーは4つすべての尺度で計測結果が抜きん出ていた
p27 "調査結果から見えてきたもの" より

![width:200px](https://images-na.ssl-images-amazon.com/images/I/81VLedmhM5L.jpg)

---
<style>
table {
  text-align: center;
}

table thead th {
  padding: 15px;
}

table td {
  font-size: 21px;
  padding: 20px;
}
</style>

| metric       | elite                 | high             | middle              | low            |
| ------------ | --------------------- | ---------------- | ------------------- | -------------- |
| デプロイ頻度 | オンデマンドに1日数回 | 1週間から月に1回 | 1ヶ月から6ヶ月に1回 | 6ヶ月に1回未満 |
| リードタイム | 1時間以内             | 1日から1週間     | 1ヶ月から6ヶ月      | 6ヶ月以上      |
| MTTR         | 1時間以内             | １日以内         | 1日から1週間        | 6ヶ月以上      |
| 変更失敗率   | 0~15%                 | 16%-30%          | 16%-30%             | 16%-30%        |

---

# 組織のパフォーマンスとは

<style scoped>
li {
font-size: 48px;
padding: 17px;
}
</style>

- 収益性
- 市場占有率
- 生産性

---
<style scoped>
h1 {
  color: black;
  font-size: 176px;
  text-align: center;
  top: 250px;
  left: 45px;
}
</style>

# ケイパビリティ

---

# ケイパビリティとは

Four Keysの改善効果が高いことが特定されている組織の能力

![image](https://user-images.githubusercontent.com/58712884/173997864-d28bcfb2-e1f8-4fa1-94d0-c8f5ac602b08.png#center)

---

# ケイパビリティとは

<style scoped>
li {
font-size: 48px;
padding: 17px;
}
</style>

- [Google Cloud](https://cloud.google.com/architecture/devops/capabilities?hl=ja)に詳しいドキュメントがある
- ケイパビリティを実装する形で改善していく
- 日々更新されている

---
<!--
_class: jukugo
-->

# 事例

---

# Four Keysを用いて開発組織の生産性を可視化した国内の事例

- [newspicks](https://tech.uzabase.com/entry/2022/01/21/113604)
- [はてな](https://developer.hatenastaff.com/entry/2021/03/04/093000)
- [GMOぺぱぼ](https://tech.pepabo.com/2022/01/06/four-keys-dashboard/)

ここに紹介した事例の他にも多くの企業でFour Keysが採用されている。
生産性可視化におけるデファクトスタンダードと言っても良い。

---

# 疑問
<!--
_class: jukugo
-->

---
<style scoped>
h1 {
  color: black;
  font-size: 57px;
  position: absolute;
  top: 330px;
  left: 40px;
}
</style>

# Q: 開発者の増減についてはどう考えたら良い？

---
<style scoped>
h1 {
  color: black;
  font-size: 90px;
  position: absolute;
  top: 330px;
  left: 70px;
}
</style>

# A: `d/d/d`を算出しましょう

---
<!--
_class: tweet
_footer: "https://twitter.com/hiroki_daichi/status/1100381137929625600?ref_src=twsrc%5Etfw"
-->

![bg height: 60%](https://user-images.githubusercontent.com/58712884/173750561-55839aec-f199-4a5c-a471-4ee6dd7fa85a.png)

---
<style scoped>
h1 {
  color: black;
  font-size: 62px;
  position: absolute;
  top: 330px;
  left: 40px;
}
</style>

# Q: どうやってFour Keysを運用にのせる？

---
<style scoped>
h1 {
  color: black;
  font-size: 220px;
  position: absolute;
  top: 250px;
  left: 40px;
}
</style>

# A: 信頼貯金

---

# A: 信頼貯金

- 4つの指標全てを同時に改善するのは難しい(予算とか工数とか)
  - まずは可視化
  - 一つの指標に的を絞って分かりやすい成果を出す
  - 結果を出して信頼してもらう
- 経営と接続して成果を定期的に報告する
- こういうのは「やっていき」が大切

---
<style scoped>
h1 {
  color: black;
  font-size: 66px;
  position: absolute;
  top: 330px;
  left: 40px;
}
</style>

# Q: 全ての作業を同じ土俵で評価するの？

---
<style scoped>
h1 {
  color: black;
  font-size: 220px;
  position: absolute;
  top: 250px;
  left: 40px;
}
</style>

# A: 結論YES

---

# A: 結論YES

<style scoped>
li {
font-size: 44px;
padding: 17px;
}
</style>

- デリバリは組織のパフォーマンスと因果関係がある
- 測定しているのはデリバリ、つまり開発の流量
- スムーズにフローが流れているかが重要な観点

---
<style scoped>
h1 {
  color: black;
  font-size: 48px;
  position: absolute;
  top: 300px;
  left: 30px;
}
</style>

# Q: 現場は具体的に何をしたら良いのかよくわかりません

---

# A: 実際の運用は以下のようなイメージ

- 部の目標としてFour Keysを設定する
- チーム毎にFour Keysに関連する数値を目標として定める
  - 例: PRオープンからmasterマージまでの時間を50%削減する
- 具体的な取り組みは27ケイパビリティを参考にする

---
<style scoped>
h1 {
  color: black;
  font-size: 105px;
  position: absolute;
  top: 300px;
  left: 45px;
}
</style>

# Q: 人事評価には使える？
  
---
<style scoped>
h1 {
  color: black;
  font-size: 95px;
  position: absolute;
  top: 300px;
  left: 45px;
}
</style>

# A: 使わない方が良いと思う

---

# A: 使わない方が良いと思う

<style scoped>
li {
font-size: 48px;
padding: 17px;
}
</style>

- Four Keysはデリバリの指標
- チームの評価までが最小単位
- 使えるとしたら一人チームの場合

---

# まとめ

<style scoped>
li {
font-size: 48px;
padding: 17px;
}
</style>

- Four Keysを測定しよう
- ケイパビリティを実装しよう
- 改善効果を測定してPDCAを回そう

---

# 参考文献

[エリート DevOps チームであることを Four Keys プロジェクトで確認する](https://cloud.google.com/blog/ja/products/gcp/using-the-four-keys-to-measure-your-devops-performance)
[DevOpsの能力](https://cloud.google.com/architecture/devops/capabilities?hl=ja)
[Findy Teamsの指標を使ってチームの生産性を改善しよう](https://tech.andpad.co.jp/entry/2022/01/06/110000)
[エンジニアの活動情報からFour Keysを集計、可視化した話](https://tech.pepabo.com/2022/01/06/four-keys-dashboard/)
[ファクトから始める改善アプローチ 〜「LeanとDevOpsの科学」を実践して〜](https://speakerdeck.com/tyankamo/huakutokarashi-merugai-shan-apuroti-leantodevopsfalseke-xue-woshi-jian-site?slide=49)
