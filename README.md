# Smart Page Extractor

![Screenshot](images/screenshot.png)

投資ニュースをMarkdown形式で保存し、Obsidianで管理するためのChrome拡張です。

---

## 主な機能

- Web記事をMarkdown形式で保存
- 銘柄コードを自動抽出
- 銘柄別インデックスノートを生成
- Obsidianとの連携に対応

---

## 対応サイト

- 株探（Kabutan）の注目記事  
https://kabutan.jp/news/marketnews/?category=9

---

# Obsidianの準備

本ツールを利用する前に、ObsidianのインストールとREST APIプラグインの設定を行ってください。

---

## 1. Obsidianをインストール

Obsidian公式サイト：  
https://obsidian.md/
1. 公式サイトからObsidianをダウンロードしてインストールしてください。
2. Vault（保管庫）を新規作成して、Obsidianで保管庫を開いてください。

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
4. 本拡張のフォルダを指定する
5. Chrome拡張の設定画面でObsidianのAPIキーを入力

---

## 記事の保存方法

1. 株探の注目ニュースページを開く
2. Chrome拡張を開く
3. 「記事を保存」を押す
4. MarkdownファイルがObsidian Vault内へ保存される
5. 「銘柄別インデックス」を押すと銘柄別インデックスノートも自動生成される

