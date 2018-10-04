# Clean Architecture
# 定期輪読会

### Chapter.15 - 17

</br>

2018-10-11

@orepuri

---

## Chapter15. アーキテクチャとは?

---

<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter15. アーキテクチャとは?
</div>
</br>


## ソフトウェアアーキテクト

</br>

最高のプログラマ

生産性を最大化する設計にチームを導く


---

<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter15. アーキテクチャとは?
</div>
</br>


## アーキテクチャ

</br>

それを構築した人が与えたシステムの形状

システムをコンポーネントに分割し </br>
うまく配置して相互通信できるようにする

---

<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter15. アーキテクチャとは?
</div>
</br>


## アーキテクチャ

</br>

システムの開発, デプロイ, 運用, 保守 (ライフサイクル) を容易にする

システムの動作に影響を与えるものではない

---

<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter15. アーキテクチャとは?
</div>
</br>


## 開発

</br>

開発が難しいソフトウェアはライフライムが短く不健全

アーキテクチャによって開発しやすくするシステムにすべき

アーキテクチャの決定はチーム構成によって異なる

---

<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter15. アーキテクチャとは?
</div>
</br>


## デプロイ

</br>

システムが効果を生み出すためにデプロイ可能な状態にする

デプロイコストが高いとシステムの有用性は低下

単一のアクションで簡単にデプロイできるようにする

---

<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter15. アーキテクチャとは?
</div>


## 運用

</br>

アーキテクチャの運用への影響は他と比べ小さい

運用の課題はハードウェアの変更で解決できる  (SWコスト > HWコスト)

優れたアーキテクチャはシステムの運用方法が明確

システムの理解が容易になり, 開発や保守に役立つ

---

<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter15. アーキテクチャとは?
</div>

## 保守

</br>


最もコストがかかる (人的リソースの消費)

主なコストは洞窟探検とリスク

---

<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter15. アーキテクチャとは?
</div>

## 保守

</br>

洞窟探検 = 既存のソフトウェアを理解してどう修正するか決める

リスク = 間違った修正をして意図しない欠陥を生む

</br>

よいアーキテクチャはコストを大幅に低下させる


---

<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter15. アーキテクチャとは?
</div>

## 選択肢を残す
</br>

ソフトウェアの2つの価値

構造(アーキテクチャ)の価値 > 振る舞いの価値

</br>

ソフトウェアの柔軟性はアーキテクチャに大きく依存する

柔軟性を維持するには, できるだけ長い期間</br>多くの選択肢を残しておく

---

<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter15. アーキテクチャとは?
</div>

## 選択肢を残す
</br>

残すべき選択肢 = 重要でない詳細

</br>

ソフトウェアの2つの要素

○ 方針 = ビジネスのルールや手順(システムの価値)

✕ 詳細 = IOデバイス, DB, Web, サーバ, フレームワークなど

---

<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter15. アーキテクチャとは?
</div>

## 選択肢を残す
</br>

アーキテクトの目的は, *方針*とは無関係に詳細を決めながら</br>*方針*を最も重要と認識するシステムの形状を作ること

---

<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter15. アーキテクチャとは?
</div>

## 選択肢を残す
</br>

詳細の決定を延期や留保することができる

適切に作るための情報が多く手に入る

</br>

すでに決定していたら?

優秀なアーキテクト「まだ決まってない」

---

<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter15. アーキテクチャとは?
</div>

## 選択肢を残した場合の例
</br>

デバイス非依存

ダイレクトメール

物理アドレス

---

<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter15. アーキテクチャとは?
</div>

## 15章 まとめ
</br>

アーキテクチャとはそれを構築した人が与えたシステムの形状

システムの開発, デプロイ, 運用, 保守をサポートするもの

システムの振る舞いには影響しない

</br>

優れたアーキテクトは方針と詳細を分離する

詳細の決定をできるだけ延期する

---

## Chapter16. 独立性

---
<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter16. 独立性
</div>

## アーキテクチャがサポートすべきこと
</br>

ユースケース

システムの運用

システムの開発

システムのデプロイ

---

<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter16. 独立性
</div>

## ユースケース
</br>

ユースケース = システムの意図

アーキテクチャはシステムの振る舞いに大きな影響を与えない

ただし, アーキテクチャレベルでシステムの意図がわかるように</br>振る舞いを明らかにすること

振る舞いがシステムのトップレベル要素に現れる</br>(クラス, 関数, モジュールなど)


---

<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter16. 独立性
</div>

## 運用
</br>

システムの運用において本質的な役割を果たす

ユースケースに対してスループットや応答時間など</br>求められる性能をサポートしなければならない

</br>

そのための決定は選択肢として残しておく

適切なコンポーネントに分割しておくことで, ニーズに合わせて</br>複数プロセス/スレッド/マイクロサービスへ移行できる


---

<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter16. 独立性
</div>

## 開発
</br>

開発環境のサポートにおいて重要な役割を果たす

</br>

**コンウェイの法則**

システムを設計する組織は, 組織のコミュニケーション構造を</br>
コピーした構造設計を生み出す

---

<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter16. 独立性
</div>

## 開発
</br>


チームや利害関係の多い組織

システムもお互いへの干渉が強くなる

</br>

独立して動けるチーム

システムも独立して開発できるようになる


---

<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter16. 独立性
</div>

## デプロイ
</br>

構築後すぐにデプロイできること

そのために適切にコンポーネントに分割すること

---

<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter16. 独立性
</div>

## 選択肢を残す (2回目)
</br>

すべての懸念を解決するコンポーネント構造の</br>バランスをとることは難しい

</br>

しかし, バランスをうまく取ることができる原則はある

この原則によって, システムを独立したコンポーネントに分割し</br>
できるだけ長時間, 多くの選択肢を残すことができる

---

<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter16. 独立性
</div>

## レイヤーの切り離し
</br>

すべてのユースケースを把握することはできないが</br>
システムの基本的な意図はわかっている

</br>

SRP(単一責任の原則)とCCP(閉鎖性共通の原則)を使用する

異なる理由で変更されるものを分離

同じ理由で変更されるものをまとめる

---

<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter16. 独立性
</div>

## レイヤーの切り離し
</br>

異なる理由で変更されるもの

UI/DB/ビジネスルールなど

</br>
ビジネスルールの中でも分離

アプリケーションと密接なもの(入力フィールドの検証など)

ドメインと密接なもの(口座の利益計算, 在庫計算など)

</br>
水平レイヤーで分離

---

<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter16. 独立性
</div>

## ユースケースの切り離し
</br>

注文入力システムに注文を追加する

注文を削除する

</br>

異なる頻度と理由で変更される

システムの水平レイヤーを薄く垂直にスライスする

注文入力システムに注文を追加するUIと注文を削除するUIを分離する

---

<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter16. 独立性
</div>

## 切り離しのイメージ

<img src="images/pic1.png" style="width:50%;"/>


---

<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter16. 独立性
</div>

## 切り離し方式
</br>

ユースケースの分離: 高スループットと低スループットに分離可能

UI/DB/ビジネスルールの分離: 異なるサーバで実行する可能

ユースケースの切り離しは運用の役に立つ

切り離し方式も選択肢の一つ

---

<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter16. 独立性
</div>

## 独立した開発が可能
</br>

コンポーネントの明確な切り離しはチーム間の干渉を緩和する

UIチームがビジネスルールチームに影響を与えることはない

注文追加のユースケースのチームが</br>注文削除のユースケースのチームの邪魔はしない

---

<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter16. 独立性
</div>

## 独立デプロイ可能性
</br>

レイヤーやユースケースの切り離しはデプロイも柔軟にする

特定のレイヤーやユースケースをホットスワップすることもできる

---

<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter16. 独立性
</div>

## 重複
</br>

本物の重複: あるインスタンスに変更があれば</br>それらのコピーも同じ変更をする必要がある

偶然の重複: 重複していたコードが異なる進化を遂げて</br>まったく違うものになる場合

似ているというだけで重複を排除してはいけない</br>(画面構成やアルゴリズム, DB)

本物の重複かどうか見分けること

---

<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter16. 独立性
</div>

## 切り離し方式(再び)
</br>

ソースコードレベル

あるモジュールへの変更が, 他のモジュールの変更や</br>再コンパイルにつながらないようにする

例: Ruby Gems

コンポーネント間の通信は関数呼び出し

---

<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter16. 独立性
</div>

## 切り離し方式(再び)
</br>

バイナリコードレベル

あるモジュールへの変更が, 他のモジュールの再ビルドや</br>デプロイにつながらないようにする

例: Jar, DDL, 共有ライブラリ

コンポーネント間の通信は関数呼び出しもしくは</br>プロセス間通信, ソケット, 共有メモリなど

---

<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter16. 独立性
</div>

## 切り離し方式(再び)
</br>

サービスレベル

例: マイクロサービス

コンポーネント間の通信はネットワークパケット

---

<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter16. 独立性
</div>

## 切り離し方式(再び)
</br>


プロジェクト初期の段階で判断するのは難しい

プロジェクトのライフサイクルによって最適な方式もかわる

---

<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter16. 独立性
</div>

## 切り離し方式(再び)
</br>

作者おすすめの方法

</br>

サービスレベルの分離ができそうなところまでコンポーネントを分離

分離はするが, 実際はソースコードレベルまでにしておく

開発/デプロイ/運用の問題が多くなれば</br>デプロイやサービスレベルに変更する

状況に応じて変更できるようにすること(戻すことも含む)

---

<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter16. 独立性
</div>

## 16章 まとめ
</br>

システムの切り離し方式は時間とともに変化する

優秀なアーキテクトはそうした変化を予見して適切に進める


---

## Chapter17. バウンダリー: 境界線を引く

---

<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter17. バウンダリー: 境界線を引く
</div>

## バウンダリー

</br>

ソフトウェアアーキテクチャとは境界線を引く技芸

ソフトウェアの要素を分離し, お互いがわからないように制限する

---

<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter17. バウンダリー: 境界線を引く
</div>

## アーキテクチャの目的を妨げるもの
</br>

結合

特に早すぎる決定との結合

</br>

早すぎる決定 = システムのビジネス要件と関係ない決定

フレームワーク/DB/Webサーバ/ユーティリティライブラリ/DI, etc

---
<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter17. バウンダリー: 境界線を引く
</div>

## 実例

悲しい結合の物語

高度なアーキテクチャを早く導入しすぎて失敗した話

</br>

NetNesse

DBの決定を遅らせることで成功した話


</br>

---
<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter17. バウンダリー: 境界線を引く
</div>

## あなたの境界線は何か?</br>いつ境界線を引くのか?
</br>

「重要なもの」と「重要でないもの」の間

ビジネスルールとUI

ビジネスルールとDB

UIとDB

---
<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter17. バウンダリー: 境界線を引く
</div>

## あなたの境界線は何か? </br>いつ境界線を引くのか?
</br>

データベースはビジネスルールにとって重要ではない

ビジネスルールが知る必要があるのはデータの永続化の機能が</br>あるということだけ

永続化がどう実装されているかは重要ではない


---
<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter17. バウンダリー: 境界線を引く
</div>

## 入力と出力
</br>

IOは無関係の原則

</br>

UIはビジネスルールに依存するが, ビジネスルールはUIに依存しない

重要なのはビジネスルール

---
<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter17. バウンダリー: 境界線を引く
</div>

## プラグインアーキテクチャ
</br>

他のコンポーネントを追加するパターン

UIやDBはプラグインとして置き換え可能

---
<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter17. バウンダリー: 境界線を引く
</div>

## プラグインの戦い
</br>

ReSharper vs Visual Studio

RsSharperがVisual Studioに依存しているため</br>Visual StudioテームはReShaperを無効化できる

逆はできない

---
<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter17. バウンダリー: 境界線を引く
</div>

## プラグインの戦い
</br>

境界線は変更の軸があるところに引く

境界線を挟んだコンポーネントはそれぞれの変更頻度や理由が違う

UIとビジネスルールは異なる時間や頻度で変更される

---

<div style="text-align: right; font-size: 15px; padding-bottom: 50px;">
  Chapter17. バウンダリー: 境界線を引く
</div>

## 17章 まとめ
</br>

境界線を引くにはまずコンポーネントに分割する

どれかがコアのビジネスルールのコンポーネントになる

コアのビジネスに直接関係しないコンポーネント（UIやDB）は</br>プラグインにしておく

これはDIPとSAPを適用したもの(詳細=実装が抽象に依存)になる
