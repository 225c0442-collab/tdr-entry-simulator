# TDR エントリーシミュレーター

東京ディズニーリゾート公式アプリの「エントリー受付」「スタンバイパス」「ディズニー・プレミアアクセス（DPA）」などの操作フローを、スマートフォン画面（375px）で再現した静的シミュレーターです。

## デモ

- http://class.tama.net/~p225C0442/cafe-map/tdr-entry-simulator/

## 特徴

- 単一の `index.html` で動作（ビルド不要）
- Tailwind CSS（CDN）＋ Noto Sans JP
- 画像素材は使わず、アイコンや背景はすべて SVG / CSS で描画
- 日付選択、チケット選択、エントリー受付、スタンバイパス、DPA、プライオリティ・シーティングなどの画面遷移を再現

## 使い方

`index.html` をブラウザで開くだけで動作します（ローカルファイルでも可）。

開発中に簡易サーバーを使う場合:

```sh
# このフォルダで
python -m http.server 8000
# → http://localhost:8000
```

## デプロイ

```sh
scp index.html p225C0442@class.tama.net:~/public_html/cafe-map/tdr-entry-simulator/
```

## 構成

```
.
├── index.html   # アプリ本体（HTML / CSS / JavaScript）
└── README.md
```

## 注意

本アプリは個人が操作フローを練習・確認するための非公式シミュレーターです。実際の予約・購入はできません。東京ディズニーリゾートおよび各社の商標・著作物とは関係ありません。
