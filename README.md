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

- ERC1155WithLock コントラクトをデプロイする

  ```bash
  bun run deploy:ERC1155WithLockModule --network baseSepolia
  ```

- verify

  ```bash
  bun run verify chain-<チェーンID>
  ```

- NFT をミント

  ```bash
  bun run mint --to 0x51908F598A5e0d8F1A3bAbFa6DF76F9704daD072 --id 0 --network baseSepolia
  ```

- NFT を Lock する

  ```bash
  bun run lock --id 0 --network baseSepolia
  ```

- NFT を unLock する

  ```bash
  bun run unlock --id 0 --network baseSepolia
  ```

- NFTを移転する。

  ```bash
  bun run transfer --to 0x1295BDc0C102EB105dC0198fdC193588fe66A1e4 --id 0 --amount 1 --network baseSepolia
  ```

## デプロイしたコントラクト

[baseSepolia - 0xfebc75a0e80dc910ee2535c3e11cd6a1f6cfcd1c](https://sepolia.basescan.org/address/0xfebc75a0e80dc910ee2535c3e11cd6a1f6cfcd1c)

## 参考文献

- [EIPS6268](https://eips.ethereum.org/EIPS/eip-6268)
- [[ERC6268] ERC1155 形式の NFT を SBT にする仕組みを理解しよう！](https://qiita.com/cardene/items/5ac107681eac3328258d)
