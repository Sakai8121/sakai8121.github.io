---
layout: game
title: "MECHADOOM"
order: 30
summary: "敵の包囲網を破壊する爽快感と戦略性、BitSummit GameJamゲームデザイン賞受賞 3Dメカアクション"
thumbnail: "assets/images/games/MECHADOOM_thumbnail.png"
period: "3～4か月 (大学3年 夏)"
role: "チーム制作 (メインプログラマー / 企画)"
tags: ["Unity", "C#", "3D Action", "Team Dev"]
screenshot_base: "assets/images/games/MECHADOOM_"
screenshot_count: 7
screenshot_ext: ".png"
primary_url: "https://bitsummit-gamejam.itch.io/mechadoom"
primary_label: "Play Now"
---

## 1. プロジェクト概要
* **ジャンル:** 3Dメカアクション
* **制作期間:** {{ page.period }}
* **体制・担当:** {{ page.role }}
* **使用技術:** {{ page.tags | join: ', ' }}

---

## 2. 作品概要
BitSummit GameJamにて制作した3Dメカアクションゲーム。東京の学生混成チーム（6名）で開発を行い、**ゲーム・デザイン賞(ゲームジャム内)**を受賞しました。

<img src="{{ site.baseurl }}/assets/images/games/MECHADOOM_explain.png" alt="ゲームの説明" class="img-fluid rounded shadow-sm d-block mx-auto my-3" style="max-height: 400px;">

<img src="{{ site.baseurl }}/assets/images/games/MECHADOOM_award.jpg" alt="ゲーム・デザイン賞の受賞" class="img-fluid rounded shadow-sm d-block mx-auto my-3" style="max-height: 400px;">

<img src="{{ site.baseurl }}/assets/images/games/MECHADOOM_exhibition.png" alt="展示の様子" class="img-fluid rounded shadow-sm d-block mx-auto my-3" style="max-height: 400px;">

---

## 3. ゲームの面白さのための工夫
* **「OverPower」を体現するリスクとリターン**
  GameJamのテーマ「OverPower（圧倒的な力）」に対し、単に強いだけでなく、強大な力を使うことに対する「良いリスクとリターン」を持たせた企画を設計しました。
* **包囲されるスリル（群衆UXの追求）**
  『エルデンリング』や『バイオハザード』のシステムを参考に、すべての敵が一塊になって追ってこないよう敵の行動を制御し、大勢の敵に周囲を囲まれるという緊迫した体験を提供しました。

<img src="{{ site.baseurl }}/assets/images/games/MECHADOOM_3.png" alt="プレイヤーのスキル発動の様子" class="img-fluid rounded shadow-sm d-block mx-auto my-3" style="max-height: 400px;">

---

## 4. 技術的な取り組み
* **群衆AIの制御プログラム**
  敵同士の重なりを防ぎ、プレイヤーを取り囲むように動く自律分散的な移動アルゴリズムを実装しました。
  具体的には以下のようなアルゴリズムです。
  ある一定の範囲内の敵の場合⇒プレイヤーを最短距離で追いかける
  ある一定の範囲内にいない敵の場合⇒敵からプレイヤーへ向かうベクトルを-90度~90度の範囲でランダムに変更する。<br>
  また、常に移動をさせるのではなく、ランダムなその場のアニメーションをランダムなタイミングで挟むことで様々な挙動をする敵に囲まれているような錯覚を生み出せたと思います。

* **インタフェースの活用**
  プレイヤーのスキルの中に敵を味方につけるスキルがあるのですが、IDamageインタフェースを実装していたことで、共通の処理で比較的短時間で実装することができました。

* **スキル発動時のカメラアクション**
  プレイヤーのスキル発動時にそれぞれのアクションにあったカメラ制御を実装しました。微調整を重ねてプレイヤーが映えるカメラ制御を達成しました。

---

## 5. 直面した課題と解決へのプロセス

### 課題①：チーム開発におけるコミュニケーションと連携
* **直面した問題:** 6名の混成チームで、企画・実装の大部分を担当する中で、他メンバー（特にデザイナーや別職種）とのコミュニケーションや仕様共有に難しさを感じました。
* **解決プロセス:** 目的意識を統一し、こまめな進捗共有と仕様のすり合わせを行うことで、チームとしての足並みを揃え、最終的に受賞という結果までプロジェクトを牽引しました。
* **得られた知見:** チーム開発においては、プログラムを書く能力だけでなく、他者の意図を汲み取り、自分の実装方針を分かりやすく伝えるスキルの重要性を学びました。

### 課題②：短期間での難易度調整と手触りの向上
* **直面した問題:** リスクとリターンのある企画はできたものの、限られた期間内での難易度調整や、アクションゲームとしての「手触り」のブラッシュアップに時間が足りませんでした。
* **解決プロセス:** 開発中はこの「手触り」に目を向けることが最後までできませんでした。ゲームを面白くしようと、とにかく様々な要素を追加していましたが、それよりも大事なことがあったことに気づけませんでした。
* **得られた知見:** 開発スケジュールの初期段階から、パラメータ調整や手触りのブラッシュアップに充てる反復調整期間をあらかじめ確保しておくことの必要性を痛感しました。
