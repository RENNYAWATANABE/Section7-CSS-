# Section7-CSS-

# CSS Selectors Demo

このプロジェクトは、**さまざまなCSSセレクタの使い方を実演するための学習用サンプル**です。HTMLに対してCSSを適用することで、セレクタの種類や優先順位、疑似クラス・疑似要素の動作を視覚的に確認できます。

---

## 🔧 使用技術

- HTML5
- CSS3（内部スタイル中心、インライン・外部CSSも使用可能）
- コメント付きでわかりやすいコード構成

---

## 🎯 学べるCSSセレクタ

| セレクタの種類              | 説明 |
|-----------------------------|------|
| `*`（ユニバーサル）         | すべての要素を選択（今回はコメントアウト済み） |
| `button`（要素型）          | 指定のHTMLタグにスタイル適用 |
| `#signup`（ID）             | 一意な要素にスタイル適用。優先度が高い |
| `.tag`（クラス）            | 複数の要素に共通スタイルを適用 |
| `.post a`（子孫）           | 親要素内の特定の子要素にスタイル |
| `h2 + button`（隣接）       | `h2`直後の`button`だけにスタイル適用 |
| `footer > a`（子セレクタ）  | `footer`直下の`a`タグのみに適用 |
| `input[type="password"]`（属性） | `type="password"`の`input`要素に適用 |
| `a[href*="google"]`（部分一致） | `href`属性に`google`を含む`a`要素に適用 |
| `.post button:hover`（疑似クラス） | マウスホバー時にスタイル変更 |
| `.post button:active`（クリック時） | ボタン押下時にスタイル変更 |
| `.post:nth-of-type(2n)`（奇数・偶数） | 2番目ごとに背景色変更 |
| `h2::first-letter`（疑似要素） | 見出しの最初の1文字を装飾 |
| `p::first-line` / `p::selection` | 段落の最初の行や選択範囲に装飾 |

---

## 💡 ポイント解説

- `!important` を使ったスタイルは**IDやクラス指定よりも強い**。
- `#signup` に直接指定された `style="color: coral"` は**インラインスタイルのため最優先**。
- 疑似クラス `:hover` や `:active` により、ユーザーの操作に応じたスタイル変更が可能。
- 疑似要素 `::first-letter`, `::selection` によって文字の一部だけに装飾を適用できる。

---

## 📁 ファイル構成

.
├── index.html # メインHTMLファイル（スタイルも含まれている）
├── app.css # 外部CSS（リンクされているが未使用）
└── README.md # 本ドキュメント

---

## 🖥️ 使い方

1. このリポジトリをクローンまたはZIPでダウンロードします。

```bash
git clone https://github.com/your-username/css-selectors-demo.git
cd css-selectors-demo

2. index.html をブラウザで開くと、動作を確認できます。

📄 ライセンス
MIT License
自由にご利用ください。

🙋‍♂️ 補足
このページはCSSの学習目的で作成されています。見た目や構造よりも、セレクタごとの違いや効果が分かることを重視しています。
