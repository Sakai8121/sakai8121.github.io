---
layout: game
title: "DarkFactory"
order: 20
summary: "Steamでのリリースを目指す。UE製オンライン協力Friendslopゲームの開発"
thumbnail: "assets/images/games/DarkFactory_thumbnail.png"
period: "制作中 (大学4年夏ごろから)"
role: "チーム制作 (メインプログラマー / 企画)"
tags: ["Unreal Engine 5", "C++", "Steamworks", "Multiplayer"]
screenshot_base: "assets/images/games/DarkFactory_"
screenshot_count: 0
screenshot_ext: ".png"
primary_url: "https://store.steampowered.com/app/3893390/DarkFactory"
primary_label: "Steam Page"
---

## 1. プロジェクト概要
* **ジャンル:** オンライン協力型闇工場シミュレーション
* **制作期間:** {{ page.period }}
* **体制・担当:** {{ page.role }}
* **使用技術:** {{ page.tags | join: ', ' }}

---

## 2. 作品概要
Steamでの商業リリースを前提に開発中の、闇工場シミュレーションゲームです。「実際にSteamで売れるクオリティ」と「収益化」を明確な目標として設定しています。ゲーム性は『Repo』や『Peak』のような協力プレイ作品を参考とし、友達と悪事をはたらいているようなマルチプレイ体験を目指しています。

<div class="ratio ratio-16x9 my-4 rounded shadow-sm overflow-hidden border">
  <iframe src="https://www.youtube.com/embed/videoseries?list=PLfuG9F8-oQEU" title="ゲーム紹介再生リスト" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</div>

<!-- 見どころピックアップ -->
<p class="fw-bold mt-5 mb-3">🎬 見どころピックアップ（※その他の動画は上のプレイヤー内から確認できます）</p>
<div class="row g-3 mb-5">
  <div class="col-6 col-md-4">
    <a href="https://youtu.be/M8MIkDDJqUM" target="_blank" class="text-decoration-none">
      <img src="https://img.youtube.com/vi/M8MIkDDJqUM/mqdefault.jpg" class="img-fluid rounded border shadow-sm" alt="怠惰な調査員">
      <p class="small text-dark fw-bold mt-2 mb-0">① 怠惰な調査員</p>
    </a>
  </div>
  <div class="col-6 col-md-4">
    <a href="https://youtu.be/dOZrAGpZ_ks" target="_blank" class="text-decoration-none">
      <img src="https://img.youtube.com/vi/dOZrAGpZ_ks/mqdefault.jpg" class="img-fluid rounded border shadow-sm" alt="調査員との会話システム">
      <p class="small text-dark fw-bold mt-2 mb-0">② 調査員との会話システム</p>
    </a>
  </div>
  <div class="col-6 col-md-4">
    <a href="https://youtu.be/fmK-L7FXZl4" target="_blank" class="text-decoration-none">
      <img src="https://img.youtube.com/vi/fmK-L7FXZl4/mqdefault.jpg" class="img-fluid rounded border shadow-sm" alt="調査員のラグドール化">
      <p class="small text-dark fw-bold mt-2 mb-0">③ 調査員のラグドール化</p>
    </a>
  </div>
  <div class="col-6 col-md-4">
    <a href="https://youtu.be/Rc5PUpeg2Rc" target="_blank" class="text-decoration-none">
      <img src="https://img.youtube.com/vi/Rc5PUpeg2Rc/mqdefault.jpg" class="img-fluid rounded border shadow-sm" alt="設置系アイテム">
      <p class="small text-dark fw-bold mt-2 mb-0">④ 設置系アイテム</p>
    </a>
  </div>
  <div class="col-6 col-md-4">
    <a href="https://youtu.be/-H71rd-8esk" target="_blank" class="text-decoration-none">
      <img src="https://img.youtube.com/vi/-H71rd-8esk/mqdefault.jpg" class="img-fluid rounded border shadow-sm" alt="アイテム箒">
      <p class="small text-dark fw-bold mt-2 mb-0">⑤ アイテム箒</p>
    </a>
  </div>
  <div class="col-6 col-md-4">
    <a href="https://youtu.be/92wdTx40lAg" target="_blank" class="text-decoration-none">
      <img src="https://img.youtube.com/vi/92wdTx40lAg/mqdefault.jpg" class="img-fluid rounded border shadow-sm" alt="裏取引システム">
      <p class="small text-dark fw-bold mt-2 mb-0">⑥ 裏取引システム</p>
    </a>
  </div>
</div>

---

## 3. ゲームの面白さのための工夫

* **友達とドタバタふざけ合える「Friendslop」体験の追求**
  本作は、単に効率を追い求める厳密な工場ビルドゲームではありません。過酷なノルマを達成するために手段を選ばず、時には友達と足を引っ張り合いながらドタバタと攻略する「Friendslop（マルチプレイでわいわいふざけ合える楽しさ）」のゲームデザインを重視しています。完璧な最適化よりも、ハプニングやアクシデント自体を笑い合えるプレイ体験を目指しています。

* **緊張感を生み出すゲームサイクルと「リスク・リターン」設計**
  ノルマを達成することで資金を獲得し、プレイヤーは「手持ちアイテム」や「工場設置型アイテム」を購入できます。設置型アイテムで闇工場を自由にカスタマイズし、手持ちアイテムを駆使してさらなる密輸や不正取引を行い、収益を最大化していくのが基本サイクルです。
  しかし、このサイクルを阻む最大のリスクとして、粗悪品を摘発しにくる「調査員」の襲来が発生します。
  違法なアイテムを「隠す」のか、リスクを冒して「奪い返す」のか、それとも「調査員自体を排除（！）する」のか。プレイヤーの選択によって、ハイリスクの裏に莫大なリターンが待つ、中毒性の高いゲームサイクルを設計しました。

* **単調な往復作業を排除するレベルデザイン**
  工場内のレイアウトカスタマイズが本作の強みですが、プレイヤーの導線が「生産機械と換金所をただ往復するだけの単調なルート」に固定化されるのを防ぐ工夫を施しました。
  具体的には、壁際に裏取引ができる「窓」を配置し、さらにメインの換金所とは真反対のエリアに、リスクはあるが緊急取引が可能なサブ換金所を2箇所設置しています。これにより、調査員の動きを読みつつ「最短安全ルートを取るか、それとも危険を冒して裏取引の窓や遠くのサブ換金所で一攫千金を狙うか」といった、マップ構造を活かした動的なルート選択と駆け引きが生まれるように設計しました。
  
---

## 4. 技術的な取り組み

* **C++とBlueprintの役割を明確に分けたアーキテクチャ**
  基盤となるロジックやパフォーマンスが要求される処理はすべてC++で堅牢に実装し、それらを関数としてBlueprintに公開する構造を徹底しています。これにより、ゲームの処理フロー全体がBlueprint上で視覚的に俯瞰しやすくなり、開発効率とパフォーマンスを両立させる技術的アプローチをとっています。

* **拡張性と保守性を両立したアイテム・AIのクラス設計**
  多様な『アイテム』や『調査員』の行動パターンを追加しやすいよう、コンポーネント指向を活用した設計を行っています。
  『アイテム』は仕様のバリエーションが多岐にわたるため、深い継承関係（ベースクラス）は作らず、インターフェース経由で共通の処理を定義し、実際の実装は各コンポーネントに持たせることで、仕様変更やバグ修正に強い設計としています。
  一方で『調査員（AI）』は、基本のBehavior Tree（ビヘイビアツリー）を用意し、個別の挙動はSubTreeで上書きする構成です。これにより開発側が挙動を作りやすくなるだけでなく、プレイヤー視点でも「敵の行動に大まかな共通のルール（予兆）」を感じ取れるようになり、理不尽さのないゲームプレイに繋がる良い設計であると考えています。

* **ペイロード構造体を用いた実装と保守性の向上**
  マルチプレイにおけるデータ同期処理を実装する際、引数の追加や変更に柔軟に対応できるよう、送信するデータを「ペイロード構造体（Struct）」としてひとまとめにする設計を採用しています。これは単なる通信のためではなく、開発者視点で「ネットワーク同期の実装・保守のしやすさ」を格段に向上させるための工夫です。

<!-- Google Docsリンクの埋め込み -->
<div class="mt-4 p-4 bg-light rounded border shadow-sm">
  <h5 class="fw-bold mb-2"><i class="fas fa-file-alt me-2"></i>開発ドキュメント（メモ）</h5>
  <p class="small text-muted mb-3">
    ※以下は開発中に思考を整理するために書いた「自分用のメモ」です。非常に乱雑な状態（汚い状態）ですが、生の試行錯誤の過程として公開しています。
  </p>
  <a href="https://docs.google.com/document/d/1yFV498ijZ95qtn0hRJWfNzQ0VF59iZOjnyCFvVRirQk/edit?usp=sharing" target="_blank" class="btn btn-outline-secondary btn-sm">
    設計ドキュメント（Google Docs）を見る
  </a>
</div>

---

## 5. 直面した課題と解決へのプロセス

### 課題①：独学でのUnreal Engineマルチプレイ実装手法の選定
* **直面した問題:** UEでの開発、マルチプレイ機能の実装、Steamリリースという複数の高いハードルに同時進行で挑戦したため、特にデータ同期のアーキテクチャにおいて、どのような手法を用いるべきか学習コストと実装方針の壁に直面しました。
* **解決プロセス:** まずAIを活用して実装手法の選択肢を幅広く洗い出し、その後、公式ドキュメントや技術記事でそれぞれのメリット・デメリットを自ら比較検証して方針を決定しました。現在も開発中であるため、この技術選定が最終的に正しかったかは今後の検証次第ですが、未知の技術に対する論理的な「アタリの付け方」としてプロセスを確立しています。

### 課題②：大量に生成される製品オブジェクトのネットワーク同期負荷
* **直面した問題:** 工場シミュレーションという性質上、マルチプレイ環境下で大量の製品（アクター）が生成・稼働するため、すべてをそのままネットワーク同期すると通信帯域を圧迫し、処理落ちや同期ズレが発生する強い懸念があります。
* **解決プロセス:** 現在、技術と仕様の両面から対応方針を立てて開発を進めています。技術面では「プレイヤーに関与しないオブジェクトの同期を切る」や「UEのMassEntity（ECSアーキテクチャ）の導入」を候補として検証予定です。また、仮に技術的な限界に達した場合は、「大量のオブジェクトを視覚的なコンテナにまとめて単一のデータとして扱う」など、仕様（ゲームデザイン）のレイヤーで負荷を吸収する方針を検討しています。
