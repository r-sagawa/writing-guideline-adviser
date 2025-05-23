# ローカル LLM によるライティングガイドライン準拠の文言提案

ローカル LLM と VSCode の拡張機能を用いて、ライティングガイドラインに準拠した UI 文言の修正案を提案してもらう方法です。

会社貸与の PC スペックでは満足に動かせないかもしれません。

## 環境構築

### Ollama のインストール

```bash
curl -fsSL https://ollama.com/install.sh | sh
```

### Ollama で扱うモデルのインストール

特に違いがわからないので llama3:8B を。

```bash
ollama pull llama3:8B
```

### VSCode 拡張機能 Continue をインストール

マーケットプレイスで Continue を探してインストール。ローカル利用の場合はサインイン不要です。

#### Continue の設定

`config.toml` の {{YOUR_PATH}}を適当なパスに書き換え、`.continue` 配下に置く。
