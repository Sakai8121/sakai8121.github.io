---
layout: game
title: "RatioPuzzle"
order: 150
summary: "「がむしゃらな実装力」だけでゲームを構築した、プログラマーとしての最初の一歩である2DパズルRPG"
tags: [Unity, C#, 2D Puzzle]
thumbnail: "assets/images/games/RatioPuzzle_thumbnail.png"
screenshot_base: "assets/images/games/RatioPuzzle_"
screenshot_count: 3
screenshot_ext: ".png"
primary_url: "/games/RatioPazleWebgl/"
primary_label: "ブラウザでプレイ"
---

## 概要
プログラミングとUnityを学習し始めて最初に完成させた、自分の開発における原点・記念碑となる2DパズルRPG作品です。「比（Ratio）」をテーマにし、直感的にすばやく比を合わせる爽快なパズル体験を目指しました。

## 技術的アプローチ
* **限られた技術スタックにおけるアイデアの実装**
  開発当時は、配列を可変長に扱う `List` やオブジェクト指向のクラス設計すら知らず、がむしゃらに「自分の脳内にあるパズル仕様をどうにかしてスクリプトに落とし込む」という愚直な実装を貫きました。

## 課題解決（Learning & Feedback）
とにかく直感的で深く考えずに遊べて爽快感のあるパズルを目指しましたが、実際に他人にプレイしてもらった際、「比」という数学用語が説明文に入っただけでプレイヤーが難しそうな印象を持ってしまうという「ビジュアル伝達上の課題」を発見しました。
数字や計算でパズルを見せるのではなく、比の増減を「風船の膨らみ具合」などのような視覚的かつ直感的な演出に翻訳してあげることで、プレイヤーの脳の認知障壁を取り除くことができるという、ゲームプログラマー（ビジュアルエンジニア）としてのUXデザインの原点を学びました。
