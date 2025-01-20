---
title: "【生成AI】Dify×スプレッドシートで情報収集を自動化しよう｜Difyラボ｜AIの活用事例研究🤖"
source: "https://note.com/dify_lab/n/n84f418838dc8"
author:
  - "[[Difyラボ｜AIの活用事例研究🤖]]"
published: 2024-12-21
created: 2025-01-08
description: "情報収集に時間がかかっていませんか？  「大量の企業リストをもとに、各企業の生成AI活用事例を調べたい」 そんなリサーチ作業も、ノーコードで簡単に自動化できる方法があるんです！  「Dify」と「スプレッドシート」簡単に連携できるChrome拡張機能 \"スプシディファイ\" を使えば、たった一つのボタン操作で、大量の情報をスピーディーに集めて整理できる仕組みが簡単に作れます！ ※動画は速度を速めています 情報収集における課題  情報収集で多くの人が感じている大きな課題。それは「時間がかかること」です。  必要な情報を探すのは、ビジネスにおいて欠かせない作業です。でも、そのリサーチに時間を"
tags:
  - "clippings"
---
**情報収集に時間がかかっていませんか？**

「大量の企業リストをもとに、各企業の生成AI活用事例を調べたい」  
そんなリサーチ作業も、**ノーコードで簡単に自動化**できる方法があるんです！

「Dify」と「スプレッドシート」簡単に連携できるChrome拡張機能 "**スプシディファイ**" を使えば、たった一つのボタン操作で、大量の情報をスピーディーに集めて整理できる仕組みが簡単に作れます！

![画像](https://assets.st-note.com/production/uploads/images/166623772/picture_pc_e31db1cb28c2f47d8b52c249f2976a6f.gif?width=1200)

※動画は速度を速めています

## 目次

## 情報収集における課題

情報収集で多くの人が感じている大きな課題。それは「時間がかかること」です。

必要な情報を探すのは、ビジネスにおいて欠かせない作業です。でも、そのリサーチに時間を取られすぎてしまうと、他の仕事に手が回らなくなることもありますよね。

例えば、こんなプロセスを一つ一つこなすだけでも、あっという間に時間が過ぎていきます：

- インターネットで検索して、複数の情報を比較
- 信頼できるデータかどうかをチェック
- 必要な情報をまとめて、整理し、あとで使いやすい形に整える

![画像](https://assets.st-note.com/img/1734760100-RstF4d9Z5T6hpiljkmoWyxcI.png?width=1200)

これをすべて人の手でやるのは、本当に骨が折れる作業です。これを解決する方法を、次の章でご紹介します！

## 生成AIを活用した解決策

そんなときこそ頼りになるのが**生成AI**です。これまで手作業で何時間もかかっていたリサーチ作業も、生成AIを活用することですぐに終わらせることができます。

生成AIを活用した情報収集のメリット：

1. **情報収集のスピードアップ**  
AIが指定したキーワードや質問に基づいて、必要な情報をネット上から素早く収集してくれます。もう、検索画面を何時間も眺める必要はありません。
2. **データの整理もお任せ**  
収集した情報を自動的にスプレッドシートに整理して保存できます。これにより、データを後で探す手間も省けます。
3. **繰り返し使える仕組み**  
一度設定すれば、毎回同じリサーチ作業を自動化できます。「また同じような内容を調べないと…」というストレスから解放されます。

![画像](https://assets.st-note.com/img/1734760573-PBy0RCJhsXmnIF4aqT56lD1w.png?width=1200)

中でも注目なのが、**Dify**というサービスです。Difyとはオープンソースの生成AIアプリ開発プラットフォームです。幅広い用途で使える生成AIアプリをノーコードで作ることができます。

DifyとGoogleスプレッドシートを組み合わせることで、情報収集の自動化を実現します。

## Difyワークフローの構築

今回作成するワークフローの全体像はこちらです！  
企業名の一覧から、その企業の生成AI活用事例を調査するワークフローです。

![画像](https://assets.st-note.com/img/1734760984-EchPgN0ROQWVqwBHLtU51SCG.png?width=1200)

ワークフローの全体像

作成手順を解説しますが、「自分で作成するのは面倒くさい」という方はこちらのDSLファイルを活用してください。

上記ファイルをダウンロードした後、Difyにログインし、「スタジオ」ページにアクセスします。  
「DSLからファイルをインポート」を選択し、先ほどのファイルをアップロードすることで、今回作成したツールを利用できます。

![画像](https://assets.st-note.com/img/1734761035-2u9TECFsAgjVO1HXakJzN8KL.png?width=1200)

それでは、Difyワークフローの作成方法を解説します！

### 1\. アプリの作成

[Dify](https://dify.ai/jp)でアカウント作成、またはログインします。  
「スタジオ」を選択し、「最初から作成」をクリックします。

![画像](https://assets.st-note.com/img/1734761494-QqZjin6fmKcRxYba5VEyX1s0.png?width=1200)

アプリの種類は「ワークフロー」を選択します。  
アプリの名前を記入し、「作成する」をクリックします。

![画像](https://assets.st-note.com/img/1734761582-UG8uBc7jNzwbIsAEeg5i4VrF.png?width=1200)

### 2\. 開始ブロックの設定

開始ブロックを選択し、「+」をクリックします。

![画像](https://assets.st-note.com/img/1734762465-hm2CxGpyRY3qVJH4wZ6slrKc.png?width=1200)

フィールドタイプは「短文」を選択します。  
変数名とラベル名を記入し、「保存」をクリックします。

この入力フィールドには、情報検索に使うキーワードが入力されます（本記事の場合は企業名が入ります！）。

![画像](https://assets.st-note.com/img/1734762543-wCZF4XUB9KsaRM0gdDPYhNQc.png?width=1200)

### 3\. 情報収集するブロックの追加

「Perplexity Search」というブロックを追加します。

![画像](https://assets.st-note.com/img/1734762688-KplsZx4OEIgSoBQTGChqz9eX.png?width=1200)

Perplexityは、Web上の情報を検索し、まとめてくれるツールです。  
Difyで使えるWeb検索ツールとその使い分けについては、こちらで解説しています。

---

**Perplexity Searchを初めて使う場合**

Perplexity Searchを初めて使う場合は、APIキーの設定が必要です。

Perplexity Searchブロックを選択し、「承認するには」をクリックします。

![画像](https://assets.st-note.com/img/1734765764-gqpF94PckWERjTd0JDN2GAe8.png?width=1200)

「取得方法」をクリックします。

![画像](https://assets.st-note.com/img/1734766104-EqTDrNb8ZYd6Ln2Gc1A0XIus.png?width=1200)

Perplexityの設定画面からAPIキーを発行してコピーします。  
APIキーの発行方法は、[こちらの記事](https://note.com/saitohtm/n/n3f17923dbe88#485ac7ea-6e0c-4749-99f8-c42971d1e6d7)も参考にしてみてください！

![画像](https://assets.st-note.com/img/1734766291-6lM54S3bTXux9InVP0EtrOdK.png?width=1200)

Difyの画面に戻り、APIキーを入力して、「保存」をクリックします。

![画像](https://assets.st-note.com/img/1734766401-xVZ5g8i20nbCXTIMfHyEvWKY.png?width=1200)

---

Perplexity Searchブロックを選択し、Queryを入力します。  
今回は、企業の生成AI活用事例を調査したいので、画像のように「/query"の生成AI活用事例をまとめて（もしあればDifyの活用事例がいいな）"」と入力します。

![画像](https://assets.st-note.com/img/1734763010-CWLjuOtrQ6I4GDyhnPgf5R7q.png?width=1200)

また、検索途中にエラーが発生した際でも、ワークフローが止まらないようにエラー処理を行います。  
エラー処理を選択し、「エラーブランチ」をクリックします。

![画像](https://assets.st-note.com/img/1734763222-qu3EtKI1kLn25c6gpAyOTfGj.png?width=1200)

試しに、「トヨタ」というキーワードでテスト実行してみると、次のような結果になります🚗

![画像](https://assets.st-note.com/img/1734763432-juBFQMIk09yDGRN4Z2dTglAt.png?width=1200)

### 4\. 検索結果の処理

PERPLEXITY SEARCHブロックの出力結果をスプレッドシートに保存しやすいように加工します。

「JSON Parse」ブロックを2つ追加し、それぞれ「content」「citations」と名付けます。

- contentは、PERPLEXITYの検索結果を受け取るブロック
- citationsは、PERPLEXITYが検索したWebページのURL（情報ソース）を受け取るブロック

です。

![画像](https://assets.st-note.com/img/1734763533-hFyP36n2wIz5gxqD7Jiers0m.png?width=1200)

contentと名付けたJSON Parseブロックを選択し、  
JSON dataに、PERPLEXITY SEARCHブロックの出力（text）  
JSON filterに、"content"  
と入力します。

![画像](https://assets.st-note.com/img/1734763727-30gwe6pNSqF5KQzlvbGd12Lt.png?width=1200)

次に、citationsと名付けたJSON Parseブロックを選択し、  
JSON dataに、PERPLEXITY SEARCHブロックの出力（text）  
JSON filterに、"citations"  
と入力します。

![画像](https://assets.st-note.com/img/1734763817-ZDJ07NU6u4ezLqVAQrFBYyWh.png?width=1200)

さらに、変数集約器ブロックを追加し、  
contentと名付けたJSON Parseブロックと、PERPLEXITY SEARCHブロックのエラーブランチから接続します。

変数集約器ブロックを選択し、  
「変数を代入する」を画像のように記入します。

![画像](https://assets.st-note.com/img/1734764870-9kVZE8b7wSAKnhWpMT5B1GUu.png?width=1200)

### 5\. 終了ブロックの追加

終了ブロックを追加し、  
変数集約器ブロックと、citationsと名付けたJSON Parseブロックから接続します。

![画像](https://assets.st-note.com/img/1734765033-IBFJ8xjMqym6o32nZvYAhLea.png?width=1200)

終了ブロックを選択し、「+」をクリックして出力変数を2つ追加します。  
contentという変数に、変数集約器の出力を、  
citationsという変数に、citationsと名付けたJSON Parseブロックの出力を記載します。

![画像](https://assets.st-note.com/img/1734765170-TAcWpmCOjhw8trqsXE9VxGki.png?width=1200)

Dify画面右上の「公開する」を選択し、「公開」または「更新」をクリックしたらDifyワークフローは完成です！

![画像](https://assets.st-note.com/img/1734765521-gA6aXkEfsIBv20QxJCbuj8Yq.png?width=1200)

テスト実行すると、下記のように、情報収集結果とその情報ソースが確認できます！

![画像](https://assets.st-note.com/img/1734768680-S0rJHdwvKbk9GLRZxg7uNesW.png?width=1200)

## Difyとスプレッドシートの連携

先ほど作成したDifyのワークフローを、スプレッドシートから呼び出し、生成AIに情報収集してもらったデータをスプレッドシートに保存します！

### 1\. スプレッドシートの用意

A列に企業名が記載されたスプレッドシートを用意します。B、C列は、列の名前だけ入力しておきます。

A列に記載の企業名は、[日本企業時価総額上位ランキング](https://www.nikkei.com/marketdata/ranking-jp/market-cap-high/) [-](https://www.nikkei.com/marketdata/ranking-jp/market-cap-high/) [日本経済新聞](https://www.nikkei.com/marketdata/ranking-jp/market-cap-high/)を参考に記載しました！

![画像](https://assets.st-note.com/img/1734766734-7QvOEygaxMA9cSDNLF4oTI8U.png?width=1200)

### 2\. DifyのAPIキーの発行

Dify画面の「APIアクセス」を選択し、「APIキー」をクリックします。  

![画像](https://assets.st-note.com/img/1734766996-C4scyMIvta9FDnO0fqrNG6mS.png?width=1200)

「新しいシークレットキーを生成」をクリックし、生成されたキーをコピーしておきます。

![画像](https://assets.st-note.com/img/1734767080-jxG97EcJ0wi8FNbM2TBd63Wv.png?width=1200)

### 3\. スプシディファイのインストール

スプシディファイは、私たちが開発したコーディング不要でDifyとスプレッドシートを連携できるChrome拡張機能です！

下記リンクにアクセスし、「Chromeに追加」をクリックします。

![画像](https://assets.st-note.com/img/1734767498-2zcIhFKrOQqxHS1WJGA4Vl9Y.png?width=1200)

「スプシディファイ」を追加しますか？  
が表示されたら、「拡張機能を追加」をクリックします。

![画像](https://assets.st-note.com/img/1734767512-c5DMB68yZY4iRn0uxaLgdEIG.png?width=1200)

### 4\. スプシディファイの初期設定

画面右上のパズルアイコンをクリックし、スプシディファイを選択します。  
（ピン留めしておくと便利です！）

![画像](https://assets.st-note.com/img/1734767737-F2v9GgCcfmXdAhuRpIZTQer6.png?width=1200)

メールアドレスを入力し、「サインアップ」をクリックします。

![画像](https://assets.st-note.com/img/1734767850-Mnc5hq4tduHXgWkfmFISzELU.png?width=1200)

画像のように表示されたら初期設定は完了です！

![画像](https://assets.st-note.com/img/1734767899-FQiJoKG5aXASLy0Zhf6IOlHj.png?width=1200)

### 5\. スプシディファイに処理を追加する

「+」をクリックし、先ほどコピーしたDifyのAPIキーを入力します。

![画像](https://assets.st-note.com/img/1734768105-qsQPZnSbkj5gArBUc9Ei7RhT.png?width=1200)

Difyに入力するための企業名が記載された範囲と、  
Difyの出力である情報収集結果と情報ソースを記入する範囲を指定します。

![画像](https://assets.st-note.com/img/1734768461-pOIek21vgt9ScJBuMPlFR50V.png?width=1200)

Difyの入出力の変数名を、それぞれ記入します。

![画像](https://assets.st-note.com/img/1734769046-orvD6hJVS0cAsaxyb2juOKwn.png?width=1200)

### 6\. 処理の実行

「実行」をクリックします。

![画像](https://assets.st-note.com/img/1734769406-XdkD7Bs1xF6WobHKGhtEICO5.png?width=1200)

初回実行時は、認証が求められます。  
Googleアカウントを選択し、「許可」をクリックします。

![画像](https://assets.st-note.com/img/1734769621-n4I1lAxEfTPVdoeqgjW5HaYz.png?width=1200)

![画像](https://assets.st-note.com/img/1734769656-fsIwD5Re4rvXHmkGxaJNBStp.png?width=1200)

以上で、全て完了です！

![画像](https://assets.st-note.com/production/uploads/images/166623977/picture_pc_6f7d4059b58dc1f6a9a9eae88496644d.gif?width=1200)

※動画は速度を速めています

## まとめ

本記事で紹介した「Dify」と「スプレッドシート」、そして便利なChrome拡張機能「**スプシディファイ**」を活用すれば、ボタンひとつで情報収集と整理を自動化できます！  
手間のかかるリサーチ作業を効率化し、本当に注力したい業務に時間を使えるようにしていきましょう！！

スプシディファイはまだまだリリースしたばかりのプロダクトです。スプシディファイに関するご意見ご要望は下記よりお寄せください。