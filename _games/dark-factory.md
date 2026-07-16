---
layout: game
title: "DarkFactory"
order: 10
summary: "査察官から違法アイテムを隠避するオンライン協力型ステルス工場シミュレーション（Steam商用リリース向け開発）"
tags: [Unreal Engine 5, C++, Multiplayer, Steamworks]
thumbnail: "assets/images/games/DarkFactory_thumbnail.png"
screenshot_base: "assets/images/games/DarkFactory_"
screenshot_count: 0
primary_url: "https://store.steampowered.com/app/3893390/DarkFactory"
primary_label: "Steamストアページ"
---

## 概要
Steamでの商業リリースを前提に開発中の、闇工場シミュレーションゲームです。「実際に売れるクオリティ」と「収益化」を明確な目標として設定しています。ゲーム性は『Repo』や『Peak』のような協力プレイ作品を参考とし、友達と悪事をはたらいているようなハラハラするマルチプレイ体験を目指しています。

## 技術的アプローチ
* **C++とBlueprintの効率的な使い分け**
  ゲーム全体のパフォーマンス向上と、マルチプレイ時におけるパケット負荷・チート耐性を意識し、ゲームの根幹ロジックや拡張性が必要となるシステムはC++側で堅牢に定義し、グラフィック表現やパラメータ調整といったイテレーション速度を重視する箇所をBlueprintで行うモジュール設計を徹底しました。
* **コンポーネント指向による拡張設計**
  多様な「違法アイテム」や「調査員の巡回・捜査行動」の挙動に柔軟なバリエーションを持たせるため、コンポーネント指向を用いた拡張性の高い設計パターンを導入しました。

## 課題解決（Learning & Feedback）
Unreal Engine 5での大規模マルチプレイ開発は初の挑戦であり、独学での開発のため学習と並行しながらの進行は多くの苦労を伴いました。
特にマルチプレイにおけるアイテムの同期や同期ズレ、ペイロード構造体を用いた安全なデータパケット通信の実装などは、試行錯誤を繰り返しながら仕様を落とし込みました。この経験を通じて、ネットワーク通信の基礎理論とUEにおける実践的なアーキテクチャの重要性を体得することができました。
