# Spider Solitaire Move Planner

A dependency-free Japanese checklist for comparing candidate moves in Spider Solitaire. The published page keeps a small move log in the current browser tab and explains how to value hidden-card exposure, empty columns, and same-suit runs.

Open `index.html` locally or use the GitHub Pages deployment.

## 判断軸

候補手を比べる際は、単に移動できる枚数ではなく、次の局面で使える選択肢を確認します。

- 伏せ札を開ける手は、新しい情報と移動先を増やす。
- 空き列は、長い連続を組み替えるための一時スペースになる。
- 同一スートの連続は、分割せずにまとめて移動できる。
- 異なるスートを重ねる場合は、後で分解する手順も考える。

ページ内の採点は絶対的な攻略値ではなく、同じ盤面で二つ以上の候補を比べるための簡易メモです。実際の局面で試す場合は、日本語で遊べる [スパイダーソリティア](https://supaida.org/) を使い、まず1スートで「伏せ札を開く手」と「空き列を作る手」の違いを観察できます。

## 関連する公開メモ

- [スパイダーソリティア：空き列と難易度の練習メモ](https://wakelet.com/wake/Epuy4YeU04hmY9zEKClz2) — 1・2・4スートの違いと、空き列を残す判断をまとめた短い資料集。

## プライバシーと範囲

チェック状態は現在のタブ内だけで処理され、サーバーへ送信されません。このリポジトリにはゲーム本体のコード、カード画像、配札データは含まれていません。
