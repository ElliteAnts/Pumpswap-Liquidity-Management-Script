# PumpSwap Liquidity Management Scripts

This repository contains TypeScript scripts for interacting with the [PumpSwap](https://pump.fun/) AMM protocol on Solana. The scripts allow you to create a pool, add liquidity, and withdraw liquidity using environment variables for configuration.

## Project Structure

### Core Scripts
- `src/createPool.ts` — Create a new PumpSwap pool with initial liquidity.
- `src/addLiq.ts` — Add liquidity to an existing pool.
- `src/withdrawLiq.ts` — Withdraw LP tokens from a pool.

### Environment Variables

Create a `.env` file in the project root with the following variables:

```**Example:**
SOLANA_RPC_URL=https://api.mainnet-beta.solana.com
WALLET_SECRET_KEY=Your_Wallet_Privatekey
BASE_MINT=
QUOTE_MINT=
BASE_DECIMALS=9
QUOTE_DECIMALS=6
INITIAL_BASE=10 // UI amounts, not lamports
INITIAL_QUOTE=0.001 // UI amounts, not lamports
ADD_LIQ_AMOUNT=0.001 // UI amounts, not lamports
WITHDRAW_LP_AMOUNT=0.001 // UI amounts, not lamports
POOL_INDEX=0
```
Replace the values with your own configuration.


## Setup

1. **Install dependencies:**
   `yarn`
2. **Build the script**
   `yarn run build`
3. **Create a pool**
   `yarn run create`
4. **Add Liquidity to the created pool**
   `yarn run deposit`
5. **Withdraw LP token from the pool**
   `yarn run withdraw`

## Transaction History

### CreatePoolTx: 
[https://solscan.io/tx/CZe675tm9FooE3Vb7EpjXgRAThiwsdM76zkMUudMRh6jjHnenF47FoXqynoct5gGoQ53vKqGxoGkPZ1bzJrDCp5](https://solscan.io/tx/CZe675tm9FooE3Vb7EpjXgRAThiwsdM76zkMUudMRh6jjHnenF47FoXqynoct5gGoQ53vKqGxoGkPZ1bzJrDCp5)
### PoolKey: 
[BeFYKqPUwpJDbhHHG3ugFWexUPct3FNhpHdZPdbFEMd1](https://solscan.io/account/BeFYKqPUwpJDbhHHG3ugFWexUPct3FNhpHdZPdbFEMd1)
### AddLiqTx: 
[https://solscan.io/tx/2EhhZigxynH1rfAT7NRFmf37jSihPPBTYrcsaDddP9gjq4kBkrCL7LyFc7ATuxtFkcEMJfmdpF8jBidXpNxkf9Yi](https://solscan.io/tx/2EhhZigxynH1rfAT7NRFmf37jSihPPBTYrcsaDddP9gjq4kBkrCL7LyFc7ATuxtFkcEMJfmdpF8jBidXpNxkf9Yi)
### WithdrawLiqTx:
[https://solscan.io/tx/3UX1A7TuiZWvFs5b4cdJgKG9me9WkV5ufN5bvkNGrbWRqLNHptQAWhXVuHyjCC6DFmV5PeqKnsyGoaePDc4fR5Wj](https://solscan.io/tx/3UX1A7TuiZWvFs5b4cdJgKG9me9WkV5ufN5bvkNGrbWRqLNHptQAWhXVuHyjCC6DFmV5PeqKnsyGoaePDc4fR5Wj)

## Contact
For a new feature integration, you can contact [me](https://t.me/idioRusty) on the Telegram
