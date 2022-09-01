---
marp: true
theme: test
header: "**PHP Conf 沖縄 2022 懇親会LT**"
footer: "by **＠isanasan_**"
---
<!--
paginate: true
-->
<style scoped>
h1 {
  color: black;
  font-size: 160px;
}
</style>

# Rectorはいいぞ

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
<style scoped>
h1 {
  color: black;
  font-size: 160px;
}
</style>

# Rector is 何

---
<style scoped>
h1 {
  color: black;
  font-size: 110px;
}
</style>

# 自動リファクタリングツール

---
<!--
_class: jukugo
-->
# 特徴

---
<!--
class: slides
-->
<style scoped>
li {
  font-size: 51px;
  padding: 15px;
}
</style>

# 特徴

- 安全
- 便利なルールがたくさん
- PHPでルールを自作

---
<!--
_class: jukugo
-->

# 安全

---
<style scoped>
li {
  font-size: 51px;
  padding: 15px;
}
</style>

# 安全

- PHPStanの結果を利用
- PHP-ParserでASTを書き変え
- 怖い場合はdry-run

---
<style scoped>
h1 {
    color: black;
    font-size: 130px;
    top: 250px;
}
</style>

# 便利なルールがたくさん

---
<style scoped>
li {
  font-size: 51px;
  padding: 15px;
}
</style>

# 便利なルールがたくさん

- 400以上のルール
- バージョンアップのためのルールセット
- 設計を見直せるルールもある

---
<style scoped>
h1 {
    color: black;
    font-size: 150px;
    top: 250px;
}
</style>

# PHPでルールを自作

---
<style scoped>
li {
  font-size: 51px;
  padding: 15px;
}
</style>

# PHPでルールを自作

- recipe.phpに概概を書く
- generateコマンドでスケルトンを生成
- PHP-Parserの部品を組み合わせて開発

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

# やってみた

---

```php
203) cake28/Test/Case/Lib/LCore/Object/LWork/GetWorkContractTest.php:0

    ---------- begin diff ----------
@@ @@
 <?php

+namespace Test\Cake2\Case\Lib\LCore\Object\LWork;
+
 use Test\Cake2\Lib\LCakeTest;
 use Cake2\Lib\LCore\Repository\LWorkRepository;
 use Cake2\Lib\WorkContract\Enum\LWorkContractBelongToEnum;
-
 /**
  * ./cake28/Console/cake l_test ./cake28/Test/Case/Lib/LCore/Object/LWork/GetWorkContractTest.php
  */
-class GetWorkContractTest extends LCakeTest
+class GetWorkContractTest extends \Test\Cake2\Lib\LCakeTest
 {

     /**
@@ @@

         $this->WorkContract->save([
             'id' => 333,
-            'belong_to' => LWorkContractBelongToEnum::WORK,
+            'belong_to' => \Cake2\Lib\WorkContract\Enum\LWorkContractBelongToEnum::WORK,
             'belong_id' => 333,
             'client_organization_id' => 333,
             'client_user_id' => 333,
@@ @@
      */
     public function オブジェクトが取得できる()
     {
-        $work = LWorkRepository::getInstance()->get(333);
+        $work = \Cake2\Lib\LCore\Repository\LWorkRepository::getInstance()->get(333);
         $workContract = $work->getWorkContract();

         $this->assertSame(333, $workContract->clientUserId);
@@ @@
      */
     public function オブジェクトが取得できない()
```

---
<!--
_class: title
-->
<style scoped>
h1 {
  color: black;
  font-size: 160px;
}
</style>

# Rectorはいいぞ

---
<style scoped>
li {
  font-size: 51px;
  padding: 15px;
}
</style>

# Rectorはいいぞ

- 巨大リポジトリをリファクタリングできる
- 自己肯定感があがる
  - 俺TUEEEEE
- メタプログラミングとかカッコイイ
