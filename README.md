# ProfitPig - $PIG
This repository hosts all ProfitPig Smart Contracts.

## Smart Liquidity Oracle System (SOLS)
ProfitPig is proudly the first to release a BEP-20 token that uses Time-Weighted Average Price (TWAP) to build liquidity and price floor. The ProfitPig token (PIG) implements a 12% tax on sells, allocated evenly to **_BuybackAndBurn, AutoLiquidity_** and **BUSD rewards**__. The token contract periodically fetches and updates the ProfitPig TWAP through the PigTWAP.sol contract, and compares the value with a previously stored TWAP. The increase, or decrease, in TWAP over the period represents trend direction. If TWAP increases, the contract auto-adds liquidity to the trading pair to increase price floor and decrease sell impact. 

ProfitPig calculates and fetches TWAP using the Uniswap V2 Oracle. Learn more about oracles here: https://docs.uniswap.org/contracts/v2/concepts/core-concepts/oracles
