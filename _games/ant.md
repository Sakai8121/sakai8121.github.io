---
layout: game
title: "UnbelievableAntKingdom"
order: 40
summary: "連鎖爆発で設計図を強化して挑む、Google Playで公開中の新感覚パズルアクション"
thumbnail: "assets/images/games/UnbelievableAntKingdom_thumbnail.png"
period: "約1年半 (大学3年〜4年初頭)"
role: "チーム制作 (メインプログラマー / 企画)"
tags: ["Unity", "C#", "Google Play Console", "Firebase", "Addressable", "asmdef"]
screenshot_base: "assets/images/games/UnbelievableAntKingdom_"
screenshot_count: 11
screenshot_ext: ".png"
primary_url: "https://unityroom.com/games/unbelievable-ant"
primary_label: "Play (Web)"
sub_links:
  - label: "Google Play"
    url: "https://play.google.com/store/apps/details?id=com.ant.UnbelievableAntKingdom"
    icon: "fab fa-google-play"
---

## 1. プロジェクト概要
* **ジャンル:** 2Dパズルアクション
* **制作期間:** {{ page.period }}
* **体制・担当:** {{ page.role }}
* **使用技術:** {{ page.tags | join: ', ' }}

---

## 2. 作品概要
Google PlayおよびUnityRoomにて公開中のパズルアクションゲームです。「デザインが統一された、一つの完成されたアプリ」をリリースすることを目標に開発し、連鎖爆発の爽快感をコアメカニクスに据えています。探索シーンの鉱石以外はすべて自分でドット絵を作りました。

---

## 3. ゲームの面白さのための工夫

* **連鎖爆発がもたらすカタルシス**
  
  共同制作者との議論を重ね、「連鎖」というメカニクスを中心にゲームシステムを構築しました。

---

## 4. 技術的な取り組み

* **モバイルプラットフォーム向けSDK連携**
  
  Google Play Consoleでのリリース手順の確立に加え、Firebaseを用いたリアルタイムオンラインランキング、および広告SDKの実装を一貫して行いました。

* **大規模な開発に向けた設計**
  
  長期的な開発になることが予想されていたため、アセット参照を柔軟にする目的で「Addressable」。コンパイル時間の短縮や循環参照を防ぐために「asmdef」、クラス同士の結合を弱くするために「VContainer」を初めて導入することに挑戦しました。

---

## 5. 直面した課題と解決へのプロセス

### 課題①：コード設計の欠如による技術的負債の蓄積
* **直面した問題:** 開発当時「ソフトウェア設計」に対する知識がほとんどない状態で実装を進めたため、開発終盤でコードが密結合になり、新機能の追加やバグ修正が極めて困難になる事態に陥りました。
* **解決プロセス:** サークルの先輩から設計の概念を教わりながら何とかリリースまで完遂させましたが、コード自体は綺麗とは言えない状態で着地しました。
* **得られた知見:** この失敗経験が、のちのDIやMVPパターンの学習に向かう最大の原動力となり、「設計の重要性」を肌で学ぶ大きな転機となりました。
