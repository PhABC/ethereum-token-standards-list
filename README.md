#### ethereum-token-standards-list
Exhaustive list of all token related standards proposed for the Ethereum network. Feel free to create pull requests or open an issue if you would like to add new or missed token standards to this list. Feel free to also suggests better description and other relationships between standards. Many of the descriptions are taken from the proposals themselves. 


# List of Ethereum Tokens Standards
## ERC-20 : Standard Token ([ERC-20](https://github.com/ethereum/EIPs/blob/master/EIPS/eip-20.md))
Standard API for fungible tokens, including transfer and balance tracking functionalities. 

## ERC-223 : Protecting Users From Accidental Contract Transfers ([ERC-223](https://github.com/ethereum/EIPs/issues/223))
ERC20 token standard is leading to money losses for end users. The main problem is lack of possibility to handle incoming ERC20 transactions, that were performed via transfer function of ERC20 token. ERC-223 describes standard functions a token contract and contract working with specified token can implement to prevent accidentally sends of tokens to contracts and make token transactions behave like ether transactions.

## ERC-667 : transferAndCall Token Standard ([ERC-667](https://github.com/ethereum/EIPs/issues/677))
`transferAndCall` behaves similarly to transfer(address,uint256,bytes), but allows implementers to gain the functionality without the risk of inadvertently locking up tokens in non-ERC223 compatible contracts. It is distinct from ERC223's transfer(address,uint256,bytes) only in name, but this distinction allows for easy distinguishability between tokens that are ERC223 and tokens that are simply ERC20 + ERC667.

## ERC-721 : Non-fungible Token Standard ([ERC-721](https://github.com/ethereum/EIPs/blob/master/EIPS/eip-721.md))
While fungible tokens can be divided, non-fungible tokens (NFTs) can not.  NFTs can be owned and transacted by individuals as well as consigned to third party brokers/wallets/auctioneers ("operators"). NFTs can represent ownership over digital or physical assets.

## ERC-777 : Operator Based Token Standard ([ERC-777](https://github.com/ethereum/EIPs/issues/777))
Instead of using `uints` for approving third parties to transfer tokens on the users behalf, ERC-777 proposes to use a boolean mapping between users and operators. This simplifies the language, the approval process and decreases gas cost. 

## ERC-809 : Renting Standard for Rival, Non-Fungible Tokens ([ERC-809](https://github.com/ethereum/EIPs/issues/809))
Rival good: a good is rival if its consumption by one individual prevents simultaneous consumption by other individuals. For example, driving a car is rival but watching the sunset is non-rival.

Non-Fungible good: a good is non-fungible if it is not interchangeable. For example, cars are non-fungible but Ether is fungible.

ERC-809 allows an owner to rent access to their rival NFTs using a standard set of commands, thus allowing users to view all past and current rental agreements from a single wallet interface.

## ERC-827 : transferFromAndCall & approveAndCall ([ERC-827](https://github.com/ethereum/EIPs/issues/827)) 
Extension to ERC-20 standard while building on ERC-667 proposal. 

## ERC-864 : NFTs Shared Ownership ([ERC-864](https://github.com/ethereum/EIPs/issues/864))
This proposal aims to enable shared ownership of NFTs natively in the NFT contract. 

## ERC-865 : DelegatedTransfer ([ERC-865](https://github.com/ethereum/EIPs/issues/865))

## ERC-874 : Weighted Non Fungible Tokens ([ERC-874](https://github.com/ethereum/EIPs/pull/874))

## ERC-918 : Minable Token Standard ([ERC-918](https://github.com/ethereum/EIPs/pull/918))

## ERC-965 : sendByCheque ([ERC-965](https://github.com/ethereum/EIPs/issues/965))

## ERC-981 : Barter Token Standard ([ERC-981](https://github.com/ethereum/EIPs/issues/981))

## ERC-994 : Delegated Non-Fungible Token Standard ([ERC-994](https://github.com/ethereum/EIPs/issues/994))

## ERC-996 : ([ERC-996](https://github.com/ethereum/EIPs/issues/995))

## ERC-998 : Composable Non-Fungible Token Standard ([ERC-998](https://github.com/ethereum/EIPs/issues/998))

## ERC-1003 : Safe Transfer To Contract Extension ([ERC-1003](https://github.com/ethereum/EIPs/issues/1003))
