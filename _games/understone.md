---
layout: game
title: "宇宙の果てでも石をめくる"
order: 110
summary: "短期間でのビルドアップと成長曲線設計に挑んだ、Unity1Weekパズルアクション"
tags: [Unity, C#]
thumbnail: "assets/images/games/understone_thumbnail.png"
screenshot_base: "assets/images/games/UnderStone_"
screenshot_count: 0
primary_url: "https://unityroom.com/games/understone"
primary_label: "Unityroomでプレイ"
---

## 概要
前作『分身サバイバー』の反省を踏まえ、1週間（Unity1Week「めくる」）で制作した作品です。スコアを競う形式にし、短いゲーム時間の中でどんどん成長していくカタルシスをゲームデザインの主軸に据えました。

## 技術的アプローチ
* **短いプレイサイクルにおける成長曲線のパラメータ制御**
  プレイヤーがプレイの過程で飽きずに、指数関数的にインフレーションしていく成長感覚（スコアアップ）を体感できるように、ゲームスピードと難易度パラメーターをミリ単位で微調整しました。

## 課題解決（Learning & Feedback）
分身サバイバーの反省を活かし高評価ランキング入りを目指したものの、目標を達成できませんでした。
原因として、「プレイヤーの予測を良い意味で裏切る、ゲームとしての心地よいサプライズ（驚き）や認知変化」が不足しており、プレイヤーの想像の範囲内に収まるプレイ感覚になってしまったと自己分析。この反省は、ただ手触りが良く綺麗なシステムを組むだけではなく、コンテンツとしての「一工夫」や「フック」を意識するきっかけとなりました。
