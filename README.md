# 🍅 Aurora Sauce Language

オーロラソースをテーマにした、学習用の小さなプログラミング言語処理系。

> Code it. Mix it. Taste it.

## 🚧 状態

初期開発段階です。言語仕様と実装は確定していません。

## 🧪 現在の実装範囲

- `say "...";` の字句解析・構文解析・評価
- コメント、文字列、行番号付き構文エラー
- `asl run examples/hello.asl` による実行

言語仕様と実装は初期段階です。仕様を変更する場合は、テストと `docs/ARCHITECTURE.md` を同時に更新してください。

## 🚀 セットアップ

```bash
python -m venv .venv
# macOS / Linux
source .venv/bin/activate
# Windows PowerShell
.venv\Scripts\Activate.ps1
python -m pip install -e ".[dev]"
```

## 🧪 検証

一括検証（テスト・Lint・Build）:

```sh
python scripts/verify.py
```

```bash
python -m pip install -e ".[dev]"
python -m pytest -q
ruff check .
python -m build
```

## ▶️ サンプル実行

```bash
asl run examples/hello.asl
```

## 📚 文書

- [開発ガイド](DEVELOPMENT.md)
- [テスト方針](TESTING.md)
- [アーキテクチャ](ARCHITECTURE.md)
- [セキュリティ](SECURITY.md)
- [ロードマップ](ROADMAP.md)

## 📄 ライセンス

Aurora Sauce Language は、
[Apache License, Version 2.0](LICENSE) のもとでライセンスされています。
