# Kazuki Kurata - Portfolio

このリポジトリは、Kazuki KurataさんのWeb Developerポートフォリオサイトです。

## GitHub Pagesでの公開手順

### 1. GitHubリポジトリの作成

1. [GitHub](https://github.com)にログイン
2. 右上の「+」ボタンをクリックし、「New repository」を選択
3. リポジトリ名を入力（例: `portfolio`）
4. 「Public」を選択
5. 「Create repository」をクリック

### 2. ファイルのアップロード

**重要: プロフィール画像の準備**
- 顔写真を `profile.jpg` という名前で保存してください
- 推奨サイズ: 500px × 500px 以上の正方形
- ファイル形式: JPG, PNG, WebP など

以下の2つの方法があります:

#### 方法A: GitHubのWeb画面から直接アップロード

1. 作成したリポジトリのページで「uploading an existing file」をクリック
2. `index.html` と `profile.jpg`（あなたの顔写真）をドラッグ&ドロップ
3. 「Commit changes」をクリック

#### 方法B: Git コマンドラインを使用

```bash
# リポジトリをクローン
git clone https://github.com/[あなたのユーザー名]/portfolio.git
cd portfolio

# index.html と profile.jpg をコピー
# (ダウンロードした index.html とあなたの顔写真 profile.jpg をこのフォルダに配置)

# Git に追加してコミット
git add index.html profile.jpg
git commit -m "Add portfolio website"
git push origin main
```

### 3. GitHub Pagesを有効化

1. リポジトリの「Settings」タブをクリック
2. 左サイドバーの「Pages」をクリック
3. 「Source」セクションで、以下を設定:
   - Branch: `main`
   - Folder: `/ (root)`
4. 「Save」をクリック

### 4. サイトの確認

数分後、以下のURLでサイトが公開されます:

```
https://[あなたのGitHubユーザー名].github.io/portfolio/
```

## カスタマイズ方法

### プロフィール画像の変更

HTMLファイル内の画像ファイル名を変更できます:

```html
<img src="profile.jpg" alt="Kazuki Kurata" class="profile-image">
```

- 別のファイル名を使用する場合は `src="profile.jpg"` の部分を変更
- 例: `src="my-photo.png"` など
- 画像を使用しない場合は、この `<img>` タグごと削除してください

### 連絡先の追加

HTMLファイルの `<div class="contact-info">` セクションに、SNSリンクなどを追加できます:

```html
<div class="contact-info">
    <a href="mailto:kuratakazuki00@gmail.com">kuratakazuki00@gmail.com</a> | 
    <a href="https://github.com/yourusername" target="_blank">GitHub</a> |
    <a href="https://linkedin.com/in/yourusername" target="_blank">LinkedIn</a>
</div>
```

### 色のカスタマイズ

CSSの以下の部分を変更すると、サイト全体の色を変更できます:

- メインカラー: `#3498db` (青色の部分)
- テキストカラー: `#2c3e50` (濃いグレー)
- 背景色: `#f8f9fa` (薄いグレー)

### スキルの追加・削除

`<div class="skills-grid">` セクション内の `<div class="skill-tag">` を追加・削除して、スキルをカスタマイズできます。

## トラブルシューティング

### サイトが表示されない場合

- GitHub Pagesの設定を確認
- ファイル名が `index.html` であることを確認
- ブランチ名が正しく設定されているか確認（`main` または `master`）
- 数分待ってから再度アクセス

### カスタムドメインを使用したい場合

1. Settings > Pages > Custom domain にドメイン名を入力
2. DNSプロバイダーでCNAMEレコードを設定

## ライセンス

このポートフォリオサイトは個人使用のためのものです。

---

作成日: 2025年11月
