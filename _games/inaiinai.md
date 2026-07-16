---
layout: game
title: "いないいないばあの達人"
order: 70
summary: "MVPアーキテクチャとUniRxの導入、保守性の高いコード設計にフォーカスしたパズルアクション"
tags: [Unity, C#, MVP Pattern, UniRx]
thumbnail: "assets/images/games/いないいないばあの達人_thumbnail.png"
screenshot_base: "assets/images/games/いないいないばあの達人_"
screenshot_count: 4
screenshot_ext: ".png"
primary_url: "https://unityroom.com/games/proinaiinaibaa"
primary_label: "Unityroomでプレイ"
---

## 概要
Unity1Week（お題：「ない」）参加作品。「シンプルな操作で最大限の面白さを」をテーマに制作。短期間で、かつこれまでの自分の実装手法を大きく進化させる「設計パターンの学習」に強くフォーカスして開発しました。

## 技術的アプローチ
* **MVP（Model-View-Presenter）パターンの実践**
  Unity開発でスパゲティになりがちだったMonobehaviour主導のコードを見直し、状態を管理する「Model」、描画に徹する「View」、両者を仲介する「Presenter」の3つに責務を明確に分離しました。
* **UniRxを用いたリアクティブプログラミング**
  Presenterにおける各種ゲームシーケンスやViewの変更通知を **UniRx** を用いたストリームで構築。イベント駆動型にすることで、クラス間の結合を徹底して排除しました。

## 課題解決（Learning & Feedback）
1週間という短いサイクルの中で設計パターンを適用することは開発速度の面で負荷がかかりましたが、最終的にロジックと描画の責務が完全に分離されたため、コードの可読性とデバッグ性が劇的に向上しました。「正しい設計は、デバッグ時間を削減し最終的に開発スピードを向上させる」という真理を実証する好例となりました。
