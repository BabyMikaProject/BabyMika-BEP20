# BabyMika

// Website: http://Babymika.xyz
// Telegram: http://t.me/officialBabyMika

The contract takes a 10% fee:
 - 4% is redistributed to all holders
 - 3% is added to the V2 LP pool
 - 1.5% is added to the DAO Treasury fund
 - 1.5% is added to the Buy Back fund

## Overview of Contract Functions:

1. Add & Remove Blacklist 
2. Include & Exclude Rewards (Excluding other contracts fron getting Reflextion)
3. SetFee - Special Fees for other Contracts (CEX, Marketplace, Mikaverse, and Etc)
4. SetFees - There is no max TX amount and the total fees can be set to at most 10%
5. Add New Pair Address - Adding New BSC pair to BBMK
6. BuyBack Configuration - Setting for Auto BuyBack
7. SwapAndLiquify - Setting Auto Swap 50% Token to BNB and add to Liquidity Pool 

## Setting up your workspace

1. run 'npm install' in your workspace
2. run Ganache and setup a workspace
3. run 'npm test' in your workspace

### Deploying locally

For testing:
1. run 'npx ganache-cli --deterministic --allowUnlimitedContractSize --networkId 2'
2. run 'npx truffle migrate --network test'

For development:
1. run 'npx ganache-cli --deterministic --allowUnlimitedContractSize --networkId 1 -p 7545'
2. run 'npx truffle migrate --network develop'

## Deploying on Smart Chain Testnet 

0. Create a wallet and get some BNB from the faucet: https://testnet.binance.org/faucet-smart
1. Copy secrets.env.template to secrets.env and set values
2. Run 'npx truffle compile'
3. Run 'npx truffle migrate --network bsctestnet'
4. Smart contract should now be deployed.
5. Verify the contract
6. Run 'npx truffle run verify BabyMika@0x0000TOKENADDRES0000 --network bsctestnet

## Running scripts

0. Run 'npx truffle exec scripts/script.js --network bsctestnet'


## License

WTFPL

