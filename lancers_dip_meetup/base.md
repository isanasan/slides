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

# もくじ

1. 課題
2. モチベーション
3. State of DevOpsの紹介
4. ケイパビリティの紹介
5. よくある疑問点

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

- Lancersプロダクト開発部QAチーム
- CakePHPのバージョンアップを担当
- DevOpsに興味関心がある

---

# 課題
<!--
_class: jukugo
-->
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

## 時限爆弾のようなリリース

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

- 今動いているものを直す必用ある？
- 効果測定どうやんの？
- 費用対効果はどれくらい？

---

# 説得失敗
<!--
_class: yojijukugo
-->

---

# モチベーション

- 推測するな計測せよ(パフォーマンスチューニングの世界の言葉)
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

- [DevOps Research and Assessment](https://www.devops-research.com/research.html)が毎年行っている調査
- ソフトウェアの開発とデリバリを高速化するプラクティスは何なのか？
- デリバリの速度はビジネスにどのような影響を与えるのか？

  ※ DORAは後にGoogleが買収した
  ※※ 2021年のレポートも[公開](https://cloud.google.com/blog/ja/products/devops-sre/announcing-dora-2021-accelerate-state-of-devops-report)されている

---
<!--
_class: yojijukugo
-->

# 調査結果

---

# 調査結果

- ソフトウェアデリバリーの尺度を定義し定量化 : **Four Keys**
- デリバリーの速度と組織のパフォーマンスとの因果関係が判明
- デリバリの速度を向上させるケイパビリティを特定

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
  margin: 10px;
  top: 250px;
}
</style>

# Four Keys

---

# Four Keysとは

デリバリのパフォーマンスを以下4つに定義した

- デプロイ頻度 : コードの変更を本番環境に適応して稼動させる頻度
- リードタイム : コードのコミットから本番稼動までの所要時間
- 平均障害復旧時間 : インシデント発生から復旧にかかる平均時間
- 変更失敗率 : 不具合が発生するリリースの確率

これを**Four Keys**と名付けた

---

# 組織のパフォーマンスとは

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

- [Google Cloud](https://cloud.google.com/architecture/devops/capabilities?hl=ja)に詳しいドキュメントがある
- 実際の改善活動はケイパビリティを実装する形で進めることになる
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
  font-size: 68px;
  position: absolute;
  top: 330px;
  left: 40px;
}
</style>

# Q: 全てのPRを同じ土俵で評価するの？

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

- デリバリのパフォーマンスは組織のパフォーマンスと因果関係がある
- 測定しているのはデリバリ、つまり開発の流量
- PRのサイズによらずスムーズにフローが流れているかが重要な観点

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

- Four Keysはデリバリの指標
- チームの評価までが最小単位
- 使えるとしたらデリバリプロセスを1人で全て担当しているケース

---

# 参考文献

[エリート DevOps チームであることを Four Keys プロジェクトで確認する](https://cloud.google.com/blog/ja/products/gcp/using-the-four-keys-to-measure-your-devops-performance)
[DevOpsの能力](https://cloud.google.com/architecture/devops/capabilities?hl=ja)
[Findy Teamsの指標を使ってチームの生産性を改善しよう](https://tech.andpad.co.jp/entry/2022/01/06/110000)
[エンジニアの活動情報からFour Keysを集計、可視化した話](https://tech.pepabo.com/2022/01/06/four-keys-dashboard/)
[ファクトから始める改善アプローチ 〜「LeanとDevOpsの科学」を実践して〜](https://speakerdeck.com/tyankamo/huakutokarashi-merugai-shan-apuroti-leantodevopsfalseke-xue-woshi-jian-site?slide=49)
