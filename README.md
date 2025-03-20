# ERC6268-Sample

ERC6268 調査用のリポジトリ

## 動かし方

- セットアップ

  `.env`を作成して環境変数を貼り付けること

  ```bash
  cp .env.example .env
  ```

  ```txt
  PRIVATE_KEY=""
  ARBITRUM_ETHERSCAN_KEY=""
  BASESCAN_API_KEY=""
  ```

- フォーマッター適用

  ```bash
  bun run format
  ```

- インストール

  ```bash
  bun install
  ```

- コンパイル

  ```bash
  bun run compile
  ```

- テスト

  ```bash
  bun run test
  ```
