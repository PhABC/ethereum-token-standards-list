#### ethereum-token-standards-list
Exhaustive list of all token related standards proposed for the Ethereum network. Feel free to create pull requests or open an issue if you would like to add new or missed token standards to this list. Feel free to also suggests better description and other relationships between standards. Many of the descriptions are taken from the proposals themselves. 

To contribute, please follow the [list element template](https://github.com/PhABC/ethereum-token-standards-list/blob/master/.github/NEW_LIST_ELEMENT_TEMPLATE.md) before making a pull requests. You can also open an issue if you disagree with some of the information in this list.

# List of Ethereum Tokens Standards
## ERC-20 : Standard Fungible Token ([EIP-20](https://github.com/ethereum/EIPs/blob/master/EIPS/eip-20.md))
Standard API for fungible tokens, including transfer and balance tracking functionalities. 

## ERC-223 : Protecting Users From Accidental Contract Transfers ([ERC-223](https://github.com/ethereum/EIPs/issues/223))
ERC20 token standard is leading to money losses for end users. The main problem is lack of possibility to handle incoming ERC20 transactions, that were performed via transfer function of ERC20 token. ERC-223 describes standard functions a token contract and contract working with specified token can implement to prevent accidentally sends of tokens to contracts and make token transactions behave like ether transactions.

#### Related to:
+ [ERC-667](https://github.com/ethereum/EIPs/issues/667)
+ [ERC-827](https://github.com/ethereum/EIPs/issues/827)
+ [ERC-995](https://github.com/ethereum/EIPs/issues/995)
+ [ERC-1003](https://github.com/ethereum/EIPs/issues/1003)

## ERC-667 : transferAndCall Token Standard ([ERC-667](https://github.com/ethereum/EIPs/issues/677))
`transferAndCall` behaves similarly to transfer(address,uint256,bytes), but allows implementers to gain the functionality without the risk of inadvertently locking up tokens in non-ERC223 compatible contracts. It is distinct from ERC223's transfer(address,uint256,bytes) only in name, but this distinction allows for easy distinguishability between tokens that are ERC223 and tokens that are simply ERC20 + ERC667.

#### Strongly Related to:
+ [ERC-223](https://github.com/ethereum/EIPs/issues/223)
+ [ERC-827](https://github.com/ethereum/EIPs/issues/827)
+ [ERC-995](https://github.com/ethereum/EIPs/issues/995)
+ [ERC-1003](https://github.com/ethereum/EIPs/issues/1003)

## ERC-721 : Non-fungible Token Standard ([EIP-721](https://github.com/ethereum/EIPs/blob/master/EIPS/eip-721.md))
While fungible tokens can be divided, non-fungible tokens (NFTs) can not.  NFTs can be owned and transacted by individuals as well as consigned to third party brokers/wallets/auctioneers ("operators"). NFTs can represent ownership over digital or physical assets.

## ERC-777 : Operator Based Token Standard ([ERC-777](https://github.com/ethereum/EIPs/issues/777))
Instead of using `uints` for approving third parties to transfer tokens on the users behalf, ERC-777 proposes to use a boolean mapping between users and operators. This simplifies the language, the approval process and decreases gas cost.

#### Related to:
+ [EIP-20](https://github.com/ethereum/EIPs/blob/master/EIPS/eip-20.md)

## ERC-809 : Renting Standard for Rival, Non-Fungible Tokens ([ERC-809](https://github.com/ethereum/EIPs/issues/809))
Rival good: a good is rival if its consumption by one individual prevents simultaneous consumption by other individuals. For example, driving a car is rival but watching the sunset is non-rival.

Non-Fungible good: a good is non-fungible if it is not interchangeable. For example, cars are non-fungible but Ether is fungible.

ERC-809 allows an owner to rent access to their rival NFTs using a standard set of commands, thus allowing users to view all past and current rental agreements from a single wallet interface.

## ERC-827 : transferFromAndCall & approveAndCall ([ERC-827](https://github.com/ethereum/EIPs/issues/827)) 
Extension to ERC-20 standard while building on ERC
-667 proposal. 

#### Strongly related to:
+ [ERC-223](https://github.com/ethereum/EIPs/issues/223)
+ [ERC-667](https://github.com/ethereum/EIPs/issues/667)
+ [ERC-995](https://github.com/ethereum/EIPs/issues/995)
+ [ERC-1003](https://github.com/ethereum/EIPs/issues/1003)

## ERC-864 : NFTs Shared Ownership ([ERC-864](https://github.com/ethereum/EIPs/issues/864))
This proposal aims to enable shared ownership of NFTs natively in the NFT contract. 

#### Related to:
+ [EIP-721](https://github.com/ethereum/EIPs/blob/master/EIPS/eip-721.md)

#### Strongly related to :
+ [ERC-981](https://github.com/ethereum/EIPs/issues/981)

## ERC-865 : TransferPreSigned ([ERC-865](https://github.com/ethereum/EIPs/issues/865))
This proposal describes one standard function a token contract can implement to allow a user to delegate transfer of tokens to a third party. The third party pays for the gas, and takes a fee in tokens.

#### Related to:
+ [EIP-20](https://github.com/ethereum/EIPs/blob/master/EIPS/eip-20.md)

#### Strongly related to:
+ [ERC-965](https://github.com/ethereum/EIPs/issues/965)

## ERC-874 : Weighted Non Fungible Tokens ([ERC-874](https://github.com/ethereum/EIPs/pull/874))
Not all NFTs are created equal. Nothing exists to distinguish one NFT from another. Weight allows a DAO or other external actors to recognize some value for unique asset holdings.

#### Related to:
+ [EIP-721](https://github.com/ethereum/EIPs/blob/master/EIPS/eip-721.md)

## ERC-918 : Minable Token Standard ([EIP-918](https://github.com/ethereum/EIPs/blob/master/EIPS/eip-918.md))
A specification for a standardized Mineable Token that uses a Proof of Work algorithm for distribution.

#### Related to:
+ [EIP-20](https://github.com/ethereum/EIPs/blob/master/EIPS/eip-20.md)

## ERC-965 : sendByCheque ([ERC-965](https://github.com/ethereum/EIPs/issues/965))
This proposal aims to allow pre-signing messages that will permit third parties to execute a token transfer without the original sender needing to do an on-chain transaction in the first place. The sender would simply need to sign a message and the third party would call `sendByCheque()` with the signature.

#### Related to:
+ [EIP-20](https://github.com/ethereum/EIPs/blob/master/EIPS/eip-20.md)

#### Strongly related to:
+ [ERC-865](https://github.com/ethereum/EIPs/issues/865)

## ERC-981 : Partial Ownership Standard ([ERC-981](https://github.com/ethereum/EIPs/issues/981))
This proposal serves to describe a new Ethereum Interface for issuing tokens for asset owners who come to a marketplace with a finite quantity of their asset to trade, representing 100% ownership of that particular issue. They then choose to divide the asset into divisible units that increase fungibility of that asset.

#### Related to:
+ [EIP-721](https://github.com/ethereum/EIPs/blob/master/EIPS/eip-721.md)

#### Strongly related to : 
* [ERC-864](https://github.com/ethereum/EIPs/issues/864). 

## ERC-994 : Delegated Non-Fungible Token Standard ([ERC-994](https://github.com/ethereum/EIPs/issues/994))
Delegated Non-Fungible Tokens (DNFTs) are a proposed extension of the ERC721 standard designed with the use case of Ethereum-based registration of land and physical property in mind. NFTs are arranged in a federated, tree-like format (similar to DNS) where NFTs can delegate and sub-contract NFTs within a certain geospace.

Unlike digital assets (like CryptoKitties) physical property requires more than just an accurate identification in a database- it also requires legal validity within the context of physical sovereignty. DNFT zones can established by land registry authorities as a root DNFT encompassing a wide area, and can delegate DNFTs as subdivisions of the root zone to existing property holders as a way to upgrade land registries. 

#### Related to:
+ [EIP-721](https://github.com/ethereum/EIPs/blob/master/EIPS/eip-721.md)

#### Related to:
+ [ERC-998](https://github.com/ethereum/EIPs/issues/998)
+ [ERC-1155](https://github.com/ethereum/EIPs/issues/1155)

## ERC-995 : Pre and Post Transfer Calls ([ERC-995](https://github.com/ethereum/EIPs/issues/995))
This standard provides an augmented token transfer functionality besides legacy proven ERC20 functionality. It allows to execute calls on transfers and approvals both before and after tokens are transferred regardless if the receiving address is a contract or not.

#### Strongly related to:
+ [ERC-223](https://github.com/ethereum/EIPs/issues/223)
+ [ERC-667](https://github.com/ethereum/EIPs/issues/667)
+ [ERC-827](https://github.com/ethereum/EIPs/issues/827)
+ [ERC-1003](https://github.com/ethereum/EIPs/issues/1003)

## ERC-998 : Composable Non-Fungible Token Standard ([ERC-998](https://github.com/ethereum/EIPs/issues/998))
A standard extension for any non-fungible token to own another non-fungible ERC-721 or standard fungible ERC-20 tokens. Transferring the token composition means transferring the entire hierarchy of items. For example, a cryptokitty may own a scratching post and a feeding dish; the dish may contain some amount of fungible “chow” tokens.

#### Related to :
+ [EIP-20](https://github.com/ethereum/EIPs/blob/master/EIPS/eip-20.md)
+ [EIP-721](https://github.com/ethereum/EIPs/blob/master/EIPS/eip-721.md)

#### Strongly related to:
+ [ERC-994](https://github.com/ethereum/EIPs/issues/994)
+ [ERC-1155](https://github.com/ethereum/EIPs/issues/1155)

## ERC-1003 : Safe Transfer To Contract Extension ([ERC-1003](https://github.com/ethereum/EIPs/issues/1003))
Instead of approving a contract to spend tokens on users behalf, ERC-1003 proposes a standard interface to first deposit to the token contract and then send to the destination contract.

#### Related to :
+ [EIP-20](https://github.com/ethereum/EIPs/blob/master/EIPS/eip-20.md)

#### Strongly related to:
+ [ERC-223](https://github.com/ethereum/EIPs/issues/223)
+ [ERC-667](https://github.com/ethereum/EIPs/issues/667)
+ [ERC-827](https://github.com/ethereum/EIPs/issues/827)
+ [ERC-995](https://github.com/ethereum/EIPs/issues/995)

## ERC-1067 : Upgradeable Token Contract Standard ([ERC-1067](https://github.com/ethereum/EIPs/issues/1067))
The following proposal describes a more distributed token contract architecture that has a simple upgrade-ability protocol and allows to bring in new functions after being deployed.

#### Related to :
+ [EIP-20](https://github.com/ethereum/EIPs/blob/master/EIPS/eip-20.md)

## ERC-1132 : Token Locking Capability Standard ([ERC-1132](https://github.com/ethereum/EIPs/issues/1132))
This proposal provides basic functionality to time-lock tokens within a contract for multiple utilities without the need of transferring tokens. It also allows fetching token balances of locked and unlocked tokens (tokens available for transfer).

#### Related to :
+ [EIP-20](https://github.com/ethereum/EIPs/blob/master/EIPS/eip-20.md)

## ERC-1155 : Multi-Tokens Standard ([ERC-1155](https://github.com/ethereum/EIPs/issues/1155))
Contract that keep tracks of multiple token balances and ownership to improve batch transfer efficiency. 

#### Related to :
+ [EIP-20](https://github.com/ethereum/EIPs/blob/master/EIPS/eip-20.md)
+ [EIP-721](https://github.com/ethereum/EIPs/blob/master/EIPS/eip-721.md)

#### Strongly related to:
+ [ERC-994](https://github.com/ethereum/EIPs/issues/994)
+ [ERC-998](https://github.com/ethereum/EIPs/issues/998)

## ERC-1190 : Non-Fungible Royalty Token Standard ([ERC-1190](https://github.com/ethereum/EIPs/issues/1190))
A standard interface for non-fungible tokens that pay royalties for a digital asset to the original creator(s) and/or owner(s).

#### Related to :
+ [EIP-721](https://github.com/ethereum/EIPs/blob/master/EIPS/eip-721.md)

