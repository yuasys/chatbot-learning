---
tags: AdSignWeb, 開発日誌, 学習ログ
title: React入門実践編
---


# 学習記録
 ## 2021/08/12
 [![image1](https://user-images.githubusercontent.com/2534721/129269779-28ace0e6-0de3-460d-a8fb-968fd9d8db30.png)](https://youtube.com/playlist?list=PLX8Rsrpnn3IVOk48awq_nKW0aFP0MGpnn)
1.  日本一わかりやすいReact入門【実践編】の#１〜#２を学習した。
2.  実際のアプリ開発の流れで「バックエンド」から着手している点が納得できた。最終目標である「デプロイ」ができないとどうしようもないので、デプロイやデータの保存などの環境を担保してから、本題の「フロントエンド開発」に進むというやり方は大変良い。

## 2021/08/13
### [#3 Firebaseプロジェクトの作成と初めてのデプロイ](https://youtu.be/ta2m6nfYHuQ)


firebaseの設定で動画の情報は古い部分があってトラブったが、落ち着いて少しずつ確認しながらやってみたらうまく行った。

【本日の成果物】https://chatbot-demo-18799.web.app/

【本日の学習のまとめ】
- Firebaseとは
![](https://i.imgur.com/C1fTq8I.png)

- デプロイまでの流れ
![](https://i.imgur.com/BOQnV7d.png)

- デプロイの詳細手順
[この手順](https://youtu.be/ta2m6nfYHuQ?t=382)を何度も繰り返して理解を深めよう！多少やり方は古いので、自分で調べながら工夫しながらやる必要はある。
1. [プロジェクトの作成](https://youtu.be/ta2m6nfYHuQ?t=457)
1. [リソースロケーションの設定](https://youtu.be/ta2m6nfYHuQ?t=538)
1. [firestoreのモード変更](https://youtu.be/ta2m6nfYHuQ?t=634)…本日現在ではこの通りはできなかった。![](https://i.imgur.com/Z3JUo7S.png)図のように既定でCloud Firestoreになっているので、いきなり「データベースの作成」ボタンのクリックでOK
1. [パッケージのインストール](https://youtu.be/ta2m6nfYHuQ?t=727)…下記のコマンドを実行してからエディタでプロジェクトを開きpackage.jsonファイルに"firebase"の記載があることを確認する
  ```
  $ cd <プロジェクトフォルダ> #私の環境では/Users/yuasys/Desktop/chatbot-demo
  $ npm install -g firebase-tools
  $ npm install --save firebase
  ```
5. [firebase login](https://youtu.be/ta2m6nfYHuQ?t=874)
1. [firebase ini](https://youtu.be/ta2m6nfYHuQ?t=947)
1.  [firebase deploy](https://youtu.be/ta2m6nfYHuQ?t=1170)…functions/src/index.tsの一行目は必ずコメントアウトしておく
   ```
  // functions/src/index.ts
  ```
### [#4 tateの設計とクラスコンポーネントの作成](https://youtu.be/ICr32kxTjG4)

※図をクリックするとそれぞれの説明(動画)にジャンプします。

#### [データモデル設計の始め方](https://youtu.be/ICr32kxTjG4?t=113)
![](https://i.imgur.com/FHqvIx4.jpg) 

#### [ルートで管理するstate](https://youtu.be/ICr32kxTjG4?t=215)

[![](https://i.imgur.com/4AITgcg.jpg)](https://youtu.be/ICr32kxTjG4?t=238)

[![](https://i.imgur.com/zO7owjJ.jpg)](https://youtu.be/ICr32kxTjG4?t=295)


[![](https://i.imgur.com/SCm3r0m.jpg)](https://youtu.be/ICr32kxTjG4?t=357)


[![](https://i.imgur.com/xwzEYYt.jpg)](https://youtu.be/ICr32kxTjG4?t=453)

[![](https://i.imgur.com/uzQpti4.jpg)](https://youtu.be/ICr32kxTjG4?t=480)

[![](https://i.imgur.com/0modxcL.jpg)](https://youtu.be/ICr32kxTjG4?t=495)


### コーディング
#### [src/App.js](https://youtu.be/ICr32kxTjG4?t=656)


