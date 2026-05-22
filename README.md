# Smart Page Extractor

投資ニュースやWeb記事を自動で構造化し、Obsidianの知識ベースへ変換するためのChrome拡張です。

記事抽出・銘柄検出・ノート生成を自動化し、「読む投資情報」を「再利用できる投資データ」へ変換します。

![Screenshot](images/screenshot.png)
![Screenshot](images/obsidian.png)

---

## 主な機能

- Web記事をMarkdown形式で保存
- 銘柄コードを自動抽出
- 銘柄別インデックスノートを生成
- Obsidian Vaultへ直接ノート保存

---

## 対応サイト

- 株探（Kabutan）の注目ニュース系ページ
  
https://kabutan.jp/news/marketnews/?category=9

---

## ダウンロード

GitHub Releases から最新版をダウンロードしてください。

---

# Obsidianの準備

本ツールを利用する前に、ObsidianのインストールとREST APIプラグインの設定を行ってください。

---

## 1. Obsidianをインストール

Obsidian公式サイト：  
https://obsidian.md/

1. 公式サイトからObsidianをダウンロードしてインストール
2. Vault（保管庫）を新規作成して開く

---

## 2. Community Plugins（コミュニティプラグイン）を有効化

1. Obsidian左下の「設定（歯車アイコン）」を開く
2. 「コミュニティプラグイン」を開く
3. 「コミュニティプラグインを有効化」を押す（無効化されている場合）

---

## 3. Local REST API & MCP Server をインストール

1. 「コミュニティプラグイン」画面で「閲覧」を押す
2. 検索欄で `REST` と入力
3. `Local REST API & MCP Server` を選択
4. 「インストール」を押す
5. 「有効化」を押す

---

## 4. HTTPS証明書をインストール

1. Obsidian設定 → `Local REST API & MCP Server` を開く
2. `this certificate` リンクをクリックして証明書ファイルをダウンロード
3. ダウンロードした `.crt` ファイルをダブルクリック
4. 「証明書のインストール」を押す
5. 「現在のユーザー」を選択して「次へ」
6. 「証明書をすべて次のストアに配置する」を選択
7. 「参照」 → 「信頼されたルート証明機関」を選択
8. 「次へ」 → 「完了」を押す
9. セキュリティ警告が表示された場合は「はい」を選択
10. 「インポートは正常に完了しました」が表示されれば完了

---

## 5. APIキーを確認

1. Obsidian設定 → 「コミュニティプラグイン」
2. `Local REST API & MCP Server` を開く
3. 表示されるAPIキーをコピー

このAPIキーをChrome拡張側へ設定してください。

---

# Chrome拡張のインストール

1. Chromeで `chrome://extensions/` を開く
2. 右上の「デベロッパーモード」をONにする
3. 「パッケージ化されていない拡張機能を読み込む」を選択
4. ダウンロードしたZIPファイルを展開し、展開後のフォルダを指定する
5. Chrome拡張の設定画面でObsidianのAPIキーを入力

---

## 記事の保存方法

1. 株探の注目ニュースページを開く
2. Chrome拡張を開く
3. 「記事を保存」を押す
4. MarkdownファイルがObsidian Vault内へ保存される
5. 「銘柄別インデックス」を押すと、銘柄別インデックスノートが自動生成される

---

## こんな方におすすめ

- 投資ニュースをあとから見返したい
- Obsidianで投資メモを管理したい
- 銘柄ごとにニュースを整理したい
- AI分析用のMarkdownデータを蓄積したい
