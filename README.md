# All files with extracted token holders are located in this repository.

## Migration data
Total number of accounts: **21016**
Total sum of tokens: **29622067581238053773524138**
RootHash: **E4DBC69BF2783B81B0423DA3F5B684C1D37CCFAE798474525C4001DB42C67669**

## Infura
All files including **infura** in the name are from scripts run against infura node.
There are two files - sorted and unsorted.

## ETH Node
All files including **eth-node** in the name are from scripts run against our own spawn parity node.
There are two files - sorted and unsorted.

## Final Token Holders
Both files **final-token-holders-sorted.json** and **final-token-holders-sorted-upperCase.json** contain the all token holders and their amounts, which will be able to migrate tokens. From these files are exluced accounts that are contracts and accounts with **0** balance. All accounts that were duplicated are merged with summed balances. 

## Accounts sent tokens directly to ERC20 Contract
The file **accounts-to-ERC20-contract** contains all accounts that have sent their tokens directly to the ERC20 contract. Accounts with zero balance are removed, duplicates are merged.

## Accounts sent tokens to the Token Burner Contract
The file **accounts-to-TokenBurner-contract** contains all accounts that have sent their tokens directly to the ERC20 contract. Accounts with zero balance are removed, duplicates are merged.


## Migration Data Generation
The migration data can be generate from one of these files **final-token-holders-sorted.json** and **final-token-holders-sorted-upperCase.json**.  Those files are generated when merging one of the following **db-eth-node-JSON**, **db-infura-JSON** together with **accounts-to-ERC20-contract** and **accounts-to-TokenBurner-contract**. Accounts with **0** balances are removed, duplicated accounts are merged with summed balances. The file is then sorted again.