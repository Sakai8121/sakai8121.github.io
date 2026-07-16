---
layout: game
title: "UnbelievableAntKingdom"
order: 40
summary: "連鎖爆発で設計図を強化して挑む、Google PlayおよびUnityRoomで公開中の新感覚パズルアクション"
tags: [Unity, C#, Mobile, Firebase]
thumbnail: "assets/images/games/UnbelievableAntKingdom_thumbnail.png"
screenshot_base: "assets/images/games/UnbelievableAntKingdom_"
screenshot_count: 11
screenshot_ext: ".png"
primary_url: "https://unityroom.com/games/unbelievable-ant"
primary_label: "Unityroomでプレイ"
sub_links:
  - label: "Google Play"
    url: "https://play.google.com/store/apps/details?id=com.ant.UnbelievableAntKingdom"
    icon: "fab fa-google-play"
---

## 概要
Google PlayおよびUnityRoomにて公開中の、連鎖爆発で設計図を強化する新感覚パズルアクションゲームです。「デザインが統一された、一つの完成されたアプリ」をリリースすることを目標に開発しました。鉱石以外のドット絵を自分で書き上げるなど、ビジュアル面でも一貫性を持たせる努力を行いました。

## 技術的アプローチ
* **モバイルプラットフォームへの統合開発**
  企画から実装、Google Play Consoleを用いたパブリッシング、Firebaseを用いた動的なオンラインランキング機能の実装、Unity Adsを用いた広告マネタイズ機能の実装まで、プロダクトの公開に必要な一連の開発パイプラインを一貫して構築しました。

## 課題解決（Learning & Feedback）
企画段階では共同制作者と議論を重ね、最終的に「連鎖」というコアメカニクスを基にリリースまで完遂しました。この開発時に初めて「ソフトウェア設計」の概念を知り、サークルの先輩から教えていただきながら制作しました。
最終的なコード構造自体は密結合が多く改善の余地が多く残りましたが、この「設計が甘いと後々の機能追加やバグ修正が極端に困難になる」という失敗経験こそが、その後のVContainerやリアクティブ設計などの学習意欲を高める最大の転機となりました。
