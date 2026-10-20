# Portfolio（静的サイト）

HTML / CSS / JavaScript のみ。ビルド不要で、GitHub Pagesにそのまま置けます。

## ファイル構成
```
index.html            本文（文章・セクション）
assets/css/style.css  デザイン（色は先頭の :root で変更）
assets/js/config.js   名前・SNSリンク（最初に編集）
assets/js/main.js     アニメーション・ナビ・隠しコマンド
```

## ローカルで確認
`index.html` をブラウザで開くだけ。または `python3 -m http.server 8000` → http://localhost:8000

## 編集方法
- 名前・GitHub・LinkedIn: `assets/js/config.js`（空にすると「準備中」表示）
- WiCON2025の作品名・目的・技術: `index.html` の `TODO` を検索して書き換え
- 作品画像: `assets/img/` に置き、`index.html` の `IMAGE COMING SOON` 部分を `<img>` に差し替え（実物のみ使用）
- 配色: `style.css` 冒頭の `--accent` など
- 公開前に `<title>` / `og:*` の「あなたの名前」と、公開URL・OGP画像（TODO）を設定

## GitHub Pagesで公開
1. GitHubで新規リポジトリを作成（`<ユーザー名>.github.io` にするとルートURLで公開）
2. このフォルダの中身をリポジトリ直下に置いて push
3. Settings → Pages → Source: `Deploy from a branch` / Branch: `main` `/ (root)`
4. 数分後に表示されます

## 今後の改善案
作品画像・デモ動画の追加／WiCON詳細の記述／OGP画像／ブログや制作ログ／英語版ページ／Lighthouseでの計測
