---
marp: true
theme: test
header: "**PHP Conf 沖縄 2022**"
footer: "by **＠isanasan_**"
---
<!--
paginate: true
-->
<style scoped>
h1 {
  color: black;
  font-size: 69px;
}
p {
  color: black;
  font-size: 50px;
  text-align: center;
}
</style>

# 「LeanとDevOpsの科学」を実践して

LancersのDevOps的取り組みとこれから

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

# PHP要素はまったく無いです

---
<style scoped>
li {
  font-size: 44px;
}
</style>

# おしながき

0. 自己紹介&会社紹介
1. 課題
2. 前提知識
3. やったこと
4. これから
5. まとめ&最後に

---

# 自己紹介
<!--
_class: yojijukugo
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

# 会社紹介
<!--
_class: yojijukugo
-->

---

![PHP カンファレンス沖縄2022_告知スライド pptx pptx](https://user-images.githubusercontent.com/58712884/185841885-b778b487-05cb-4900-be42-2c11b9b7094f.png)

---

![PHP カンファレンス沖縄2022_告知スライド pptx pptx (1)](https://user-images.githubusercontent.com/58712884/185629674-2cefae46-eaf0-487c-80d3-8d0bd169d4ad.png)

---
<!--
_class: jukugo
-->
# 課題

---
<style scoped>
h1 {
  color: black;
  font-size: 95px;
  top: 300px;
  left: 40px;
}
</style>

# 開発組織の生産性がわからない

---
<style scoped>
li {
  font-size: 51px;
  padding: 15px;
}
</style>

# 開発組織の生産性がわからない

- 生産性を計測していない
- そもそも生産性の定義がわからない

---
<style scoped>
h1 {
  color: black;
  font-size: 95px;
  top: 300px;
  left: 130px;
}
</style>

# 施策の効果測定ができない

---
<style scoped>
li {
  font-size: 51px;
  padding: 15px;
}
</style>

# 施策の効果測定ができない

- 成功したか否か？その原因は？
- 横展開するべきか否か？それは何故か？
- 継続するか否か？その根拠は？

---
<style scoped>
h1 {
  color: black;
  font-size: 83px;
  top: 300px;
  text-align: center;
}
</style>

# 改善提案しても議論が空中戦になる

---
<style scoped>
li {
  font-size: 51px;
  padding: 15px;
}
</style>

# 改善提案しても議論が空中戦になる

- 今のままでも問題無くない？
- 効果測定どうやんの？
- 費用対効果はどれくらい？

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
<!--
_class: yojijukugo
-->
# 前提知識

---
<style scoped>
li {
  font-size: 51px;
  padding: 15px;
}
</style>

# 前提知識

- LeanとDevOpsの科学
- Four Keys
- 27のケイパビリティ

---
<style scoped>
p {
  font-size: 53px;
  text-align: center;
  top: 250px;
}
</style>

# LeanとDevOpsの科学

開発組織の生産性について
調査結果を解説した本

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

# Four Keys

<style scoped>
p {
  font-size: 83px;
  text-align: center;
  top: 250px;
}
</style>

デリバリのパフォーマンスを測定する4つの尺度

---
<style scoped>
li {
  font-size: 51px;
}
</style>

# Four Keys

- デプロイ頻度
- リードタイム
- 平均障害復旧時間
- 変更失敗率

---
<style scoped>
p {
  color: black;
  font-size: 71px;
  text-align: center;
  margin: 10px;
  top: 250px;
}
</style>

# 27のケイパビリティ

Four Keysの改善効果が高いことが特定されている組織の能力

---
<!--
_footer: "https://cloud.google.com/architecture/devops"
-->
<style scoped>
footer {
  left: 400px;
}
</style>

# 27のケイパビリティ

![width:960px bg](https://user-images.githubusercontent.com/58712884/185543671-d50cd3e6-abb5-45e6-94cd-ab8fb54a301c.png)

---
<style scoped>
h1 {
    color: black;
    font-size: 230px;
    padding: 40px;
    top: 170px;
    left: 155px;
}
</style>

# やったこと

---
<style scoped>
li {
  font-size: 51px;
  padding: 10px;
}
</style>

# やったこと

- Four Keys計測のためのデータ基盤の構築
- ダッシュボードを作成して可視化
- 目標を設定し運用開始
- 勉強会の開催

---
<!--
_footer: "https://developer.hatenastaff.com/entry/2021/03/04/093000"
-->
<style scoped>
footer {
  left: 400px;
}
</style>

# 計測のためのデータ基盤の構築

![bg width:60%](https://user-images.githubusercontent.com/58712884/185623882-0f014bf4-3c2f-4800-98c3-ad3e75fc3bb9.png)

---

# 計測のためのデータ基盤の構築

![bg width:760px](diagram.drawio.svg)

---
<!--
_footer: "https://github.com/isanasan/pull-request-analysis-sample"
-->
<style scoped>
footer {
  left: 350px;
}
</style>

# 計測のためのデータ基盤の構築

![bg width:800px](https://user-images.githubusercontent.com/58712884/185732166-d32e9ef2-a901-4ea8-9a84-9ebe517dfee3.png)

---

# ダッシュボードを作成して可視化

![bg width:1000px](https://user-images.githubusercontent.com/58712884/185625647-b86bbb30-0d34-4046-88be-8cc1e724a38a.png)

---
<!--
_footer: "https://speakerdeck.com/uzabasetech/18-e-5-uzabase-gao-shan-wen-debusamideng-tan-zi-liao"
-->
<style scoped>
footer {
  left: 220px;
}
</style>

# 目標を設定し運用開始

![bg width:820px](https://user-images.githubusercontent.com/58712884/185628357-b43b1a32-3723-432d-9a1b-209c23ba69c8.png)

---
<style scoped>
li {
  font-size: 51px;
  padding: 10px;
}
</style>

# 目標を設定し運用開始

- 年間目標はデプロイ頻度昨年度比2倍
- CEO含む経営層が参加するMTGで進捗報告
- 報告する際は総デプロイ数ベース

---
<style scoped>
li {
  font-size: 51px;
  padding: 10px;
}
</style>

# 勉強会の開催

- ケイパビリティについての解像度を高める
- ディスカッションでケイパビリティの実態を調査
- ボトムアップの改善に繋げる

---
<!--
_class: yojijukugo
-->
# これから

---
<style scoped>
li {
  font-size: 51px;
  padding: 10px;
}
</style>

# これから

- ケイパビリティの実態調査および実装
- 収集したメトリクスの利活用
- 品質に関するメトリクスの収集

---
<style scoped>
li {
  font-size: 51px;
  padding: 10px;
}
</style>

# ケイパビリティの実態調査および実装

- CIの実行時間短縮
- Value Streem mapの作成
- アーキテクチャの改善

---
<style scoped>
li {
  font-size: 51px;
  padding: 10px;
}
</style>

# 収集したメトリクスの利活用

- 事業部毎やチーム毎にメトリクスをレポート
- ヒストグラム解析などの踏み込んだ分析

---
<style scoped>
li {
  font-size: 51px;
  padding: 10px;
}
</style>

# 品質に関するメトリクスの収集

- MTTR
- 変更失敗率
- SLI/SLO

---
<!--
_class: sanmoji
-->
# まとめ

---
<style scoped>
li {
  font-size: 51px;
  padding: 10px;
}
</style>

# まとめ

- 開発組織のメトリクスを測定できるようにした
- 目標を設定して運用を開始した
- 現場への啓蒙と実態の調査を継続中

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
  top: 220px;
  text-align: center;
  left: 5px;
}
</style>

# トップダウンとボトムアップ両方から改善していく💪

---
<style scoped>
h1 {
  color: black;
  font-size: 145px;
  top: 280px;
  text-align: center;
}
</style>

# WE ARE HIRING

---

![](https://user-images.githubusercontent.com/58712884/185629682-40fbdc6d-1fcf-4892-bc44-c918e45dde63.png)

---

# 参考資料

[CTOとして招聘されて1年でDX Criteriaを大幅改善するために追求した唯一の成果指標](https://speakerdeck.com/uzabasetech/18-e-5-uzabase-gao-shan-wen-debusamideng-tan-zi-liao)
[Pull Requestから社内全チームの開発パフォーマンス指標を可視化し、開発チーム改善に活かそう](https://developer.hatenastaff.com/entry/2021/03/04/093000)
[ファクトから始める改善アプローチ 〜「LeanとDevOpsの科学」を実践して〜](https://speakerdeck.com/tyankamo/huakutokarashi-merugai-shan-apuroti-leantodevopsfalseke-xue-woshi-jian-site)
