# Section7-CSS-

CSS Selectors Demo
このプロジェクトは、CSSセレクタの基本と応用を学ぶためのデモページです。さまざまな種類のCSSセレクタ（要素型・ID・クラス・子孫・隣接・属性・疑似クラス・疑似要素など）の使い方を、実際のHTML要素にスタイルを適用することで体験的に学べる構成になっています。

🔧 使用技術
HTML5

CSS3（インライン・外部・埋め込み）

日本語コメント付きでわかりやすく記述

🧪 学べるセレクタ一覧
セレクタの種類	内容・用途の説明
ユニバーサルセレクタ (*)	すべての要素に一括指定可能（例：全体の背景色）※コメントアウト済
要素型セレクタ (button, h1など)	特定のHTML要素にスタイルを適用
IDセレクタ (#signup)	一意なID要素に適用。最も優先度が高いセレクタの一つ
クラスセレクタ (.tag)	複数の要素に適用可能な共通スタイル
子孫セレクタ (.post a)	特定の親要素配下の要素を対象にする
隣接セレクタ (h2 + button)	直後に続く兄弟要素にスタイルを適用
子セレクタ (footer > a)	直下の子要素にのみ適用
属性セレクタ (input[type="password"])	指定された属性値を持つ要素を対象にする
部分一致属性セレクタ (a[href*="google"])	属性の値の一部に文字列が含まれる要素を対象
疑似クラス (:hover, :active, :nth-of-type)	要素の状態（ホバー、クリック中、順番など）によってスタイルを変更
疑似要素 (::first-letter, ::first-line, ::selection)	テキストの一部に対してスタイルを付ける

💡 特徴的な実装
button { background-color: magenta !important; }
→ !important を使用して、他のスタイル指定より優先度を高めています。

#signup に style="color: coral" を記述
→ インラインスタイルは最も強い指定であり、!important が無い限り他のCSS指定を上書きします。

.post:nth-of-type(2n)
→ 投稿セクションに対して、2つごとに背景色を変更。

.post button:hover と .post button:active
→ マウスホバー・クリック中の状態に応じてボタンの見た目が変わります。

📂 ファイル構成
css
コピーする
編集する
.
├── index.html          ← メインHTMLファイル（CSSも内蔵）
├── app.css             ← 外部CSSファイル（読み込みだけされているが中身なしor任意で追加）
└── README.md           ← 本ファイル
🖥️ 使用方法
このリポジトリをクローンまたはダウンロード

index.html をブラウザで開くだけ！

bash
コピーする
編集する
git clone https://github.com/your-username/css-selectors-demo.git
cd css-selectors-demo
open index.html
📘 補足
このデモは、CSS学習者がセレクタの優先順位やさまざまな指定方法を視覚的に理解することを目的としています。冗長に見えるコードやコメントも、学習効果を高めるためにあえて残してあります。

📄 ライセンス
このプロジェクトはMITライセンスの下で公開されています。
