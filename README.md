# Claude Code Lab

Claude Code によるプログラム開発・テスト環境です。複数の言語に対応し、その時々のニーズに応じたテストコード・サンプルコードを実装できます。

## プロジェクト構成

```
.
├── python/              # Python テスト・開発用ディレクトリ
│   ├── requirements.txt  # Python 依存パッケージ
│   └── tests/           # テストコード
├── javascript/          # JavaScript/TypeScript 用ディレクトリ
│   ├── package.json     # npm パッケージ設定
│   └── tests/           # テストコード
├── nextjs/              # Next.js / Vercel デプロイ用ディレクトリ
│   ├── app/             # App Router pages
│   ├── public/          # Static files
│   ├── package.json     # npm パッケージ設定
│   └── .env.local.example
├── docs/                # ドキュメント
├── scripts/             # ユーティリティスクリプト
├── vercel.json          # Vercel デプロイ設定
└── README.md
```

## セットアップ

### Python 環境
```bash
cd python
pip install -r requirements.txt
```

### JavaScript/TypeScript 環境
```bash
cd javascript
npm install
```

### Next.js / Vercel デプロイ環境
```bash
cd nextjs
npm install

# ローカル環境変数の設定（必要に応じて）
cp .env.local.example .env.local
# .env.local を編集して、必要な設定を追加

# 開発サーバーを起動
npm run dev
```
開発サーバーは `http://localhost:3000` で起動します。

## テスト実行

### Python テスト
```bash
cd python
pytest tests/
```

### JavaScript テスト
```bash
cd javascript
npm test
```

## 使い方

Claude Code でこのディレクトリを開いて、言語別のディレクトリ配下にテストコード・実装コードを追加してください。

## ライセンス

MIT License
