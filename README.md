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

- ERC1155WithLockコントラクトをデプロイする

  ```bash
  bun run deploy:ERC1155WithLockModule --network baseSepolia
  ```

- verify

  ```bash
  bun run verify chain-<チェーンID>
  ```

## デプロイしたコントラクト

[baseSepolia - 0xfebc75a0e80dc910ee2535c3e11cd6a1f6cfcd1c](https://sepolia.basescan.org/address/0xfebc75a0e80dc910ee2535c3e11cd6a1f6cfcd1c)

## 参考文献

- [EIPS6268](https://eips.ethereum.org/EIPS/eip-6268)
- [[ERC6268] ERC1155形式のNFTをSBTにする仕組みを理解しよう！](https://qiita.com/cardene/items/5ac107681eac3328258d)
