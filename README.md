# ATOZI PHOTO — Portfolio Site

## フォルダ構成

```
atozi-photo/
├── index.html          # メインページ
├── assets/
│   └── texture.png     # 背景テクスチャ画像（ここに配置）
├── photos/
│   ├── photo_001.jpg   # 写真ファイル（ここに配置）
│   ├── photo_002.jpg
│   └── ...
└── data/
    └── photos.json     # 写真のタイトル・説明・カテゴリ管理
```

---

## 写真を追加する方法

### 1. 写真ファイルを追加
`photos/` フォルダに画像ファイルを追加します。
- 対応形式: `.jpg` `.jpeg` `.png` `.webp`
- 推奨サイズ: 横 1200px 以上

### 2. `data/photos.json` を編集
以下の形式で1エントリを追記します：

```json
{
  "id": 7,
  "filename": "photo_007.jpg",
  "title": "写真のタイトル",
  "description": "写真の説明文をここに入力します。",
  "category": "sky"
}
```

**カテゴリの種類:**
- `sky` — 空
- `nature` — 自然
- `landscape` — 風景
- （必要に応じてカテゴリを増やすことも可能）

### 3. ナビゲーションにカテゴリを追加したい場合
`index.html` の `<nav>` 内のボタン部分にカテゴリを追記してください。

---

## 背景テクスチャの変更
`assets/texture.png` を差し替えてください（同じファイル名を維持）。

---

## GitHub Pages での公開
1. このリポジトリを GitHub にプッシュ
2. Settings → Pages → Source を `main` ブランチに設定
3. 公開完了
