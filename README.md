# Awesome RGB Protocol

 A curated list of RGB projects and resources 
 
 [![Awesome](https://awesome.re/badge-flat2.svg)](https://awesome.re)

 ![image](https://github.com/22388o/awesome-rgb-protocol/assets/83122757/764c7d5c-835c-4243-97f3-7d449a83ae00)


## What is RGB protocol?

RGB has appeared from the research by Peter Todd on single-use-seals and client-side-validation, which was coined in 2016-2019 by Giacomo Zucco and community into a better asset protocol for Bitcoin and Lightning network. Further evolution of these ideas led to a development of RGB into a fully-fledged smart contract system by Maxim Orlovsky, who is leading its implementation since 2019 with community participation.
 
RGB is a scalable & confidential smart contracts system for Bitcoin & lightning network. They embrace concepts of private & mutual ownership, abstraction and separation of concerns and represent "post-blockchain", Turing-complete form of trustless distributed computing which does not require introduction of "tokens".

RGB is not a token protocol. Though issuance and management of highly scalable, programmable and private assets of different sort is possible with RGB, it can be applied in many industries far beyond financial world.

As a smart contract system RGB is quite different from previous approaches, both Bitcoin-based (Colored coins, Counterparty, OMNI) and non-bitcoin (Ethereum, EOS and others):
RGB separates concept of smart contract issuer, state owners and state evolution
RGB keeps the smart contract code and data off-chain
RGB uses blockchain as a state commitment layer and Bitcoin script as an ownership control system; while smart contract evolution is defined by off-chain schema

### Potential Use Case

- Tokenized Securities
- Decentralized Exchanges
- NFTs
- Stablecoins
- Decentralized identities
- Storage
- Lending
- Atomic Swap
- Submarine Swap
- Wallets
- Explorers
- Machine Learning

## Tech Overview

Little overview around RGB 

### Core

- AluVM
- Encoding schema
- BP Core Lib
- Client-Side-Validation

### Design

In simple terms, RGB is a system that allows the user to audit a smart contract, execute it and verify it individually at any time without having an additional cost since for this it does not use a blockchain as "traditional" systems do, complex smart contracts systems were pioneered by Ethereum but due to it requires the user to spend significant amounts of gas for each operation, they never achieved the scalability they promised by consequence it never was an option to bank the users excluded from the current financial system.

Currently, the blockchain industry promotes that both the code of smart contracts and the data must be stored in the blockchain and executed by each node of the network, regardless of the excessive increase in size or the misuse of computational resources. The scheme proposed by RGB is much more intelligent and efficient since it cuts with the blockchain paradigm by having smart contracts and data separated from the blockchain and thus avoids the saturation of the network seen in other platforms, in turn it does not force each node to execute each contract but rather the parties involved which adds confidentiality to a level never seen before.

In RGB smart contract developer defines a scheme specifying rules how the contract evolves over time. The scheme is the standard for the construction of smart contracts in RGB, and both an issuer when defining a contract for issuance and a wallet or exchange must adhere to a particular scheme against which they must validate the contract. Only if the validation is correct can each party accept requests and work with the asset.

A smart contract in RGB is a directed acyclic graph (DAG) of state changes, where only a portion of the graph is always known and there is no access to the rest. The RGB scheme is a core set of rules for the evolution of this graph the smart contract starts with. Each contract participant may add to those rules (if this is allowed by the schema) and the resulting graph is built from the iterative application of those rules.


## Protocol 

- [LNP/BP Standards Association](https://github.com/LNP-BP)
- [RGB Working Group repository](https://github.com/RGB-WG) 
- [LNP/BP Association (website)](https://www.lnp-bp.org/)
- [LNP/BP Association (YouTube)](https://www.youtube.com/channel/UCK_Q3xcQ-H3ERwArGaMKsxg)
- [LNP/BP Association (Twitter)](https://twitter.com/lnp_bp)

## Resources

- [RGB FAQ](https://www.rgbfaq.com/) 
- [RGB Tech](https://rgb.tech/) 
- [RGB Info](https://rgb.info/)
- [RGB Blackpaper](https://blackpaper.rgb.tech/)
- [RGB Spec](https://spec.rgb.tech/)
- [AluVM](https://www.aluvm.org/)
- [Contractum](https://www.contractum.org/)
- [Strict types](https://www.strict-types.org/)
- [List of specifications](https://standards.lnp-bp.org/)
- [UBIDECO Institute](https://github.com/UBIDECO)
- [Archive of legacy RGB development](https://github.com/rgb-archive)
- [RGB Blueprint Old](https://rgb-org.github.io/)

## Community

- [RGB Telegram](https://t.me/rgbtelegram)
- [RGBaguette](https://t.me/rgbaguette) 
- [RGB Italia](https://t.me/rgbitalia) 
- [RGB Developers](https://t.me/RGBDevelopers)
- [RGB Twitter List](https://twitter.com/i/lists/1582840508933582849/members)
- [RGB Community (Twitter)](https://twitter.com/i/communities/1585365616743022595)

## Articles

- [Understanding the RGB protocol](https://medium.com/@FedericoTenga/understanding-rgb-protocol-7dc7819d3059)
- [A Brief Introduction To RGB Protocols](https://bitcoinmagazine.com/guides/a-brief-introduction-to-rgb-protocols)
- [With RGB, The Bitcoin Lightning Network Can Now Transfer Altcoin Assets](https://bitcoinmagazine.com/technical/how-rgb-enables-altcoins-on-bitcoin)
- [RGB Magic: Client-Side Contracts On Bitcoin](https://bitcoinmagazine.com/technical/rgb-magic-client-contracts-on-bitcoin)
- [Video Interview: Giacomo Zucco and RGB Tokens Built on Bitcoin](https://bitcoinmagazine.com/culture/video-interview-giacomo-zucco-rgb-tokens-built-bitcoin)
- [RGB And Taro, Both Putting Tokens On Bitcoin, Take Two Different Approaches To Development](https://bitcoinmagazine.com/technical/rgb-taro-putting-tokens-on-bitcoin)
- [BTC-Backed Stablecoins Will be An Integral Part Of The Bitcoin Economy](https://bitcoinmagazine.com/technical/world-needs-bitcoin-backed-stablecoins)
- [The Path To A Bitcoin Economy: Decentralized Bitcoin-Backed Credit](https://bitcoinmagazine.com/culture/decentralized-bitcoin-backed-credit)
- [Ordinals Have Proven Demand On Bitcoin, But Fees Will Push Users To Layer 2](https://bitcoinmagazine.com/culture/bitcoin-ordinal-problems-solved-by-layer-2)
- [Emergence of Token Layers on Bitcoin: Overview of Client-Side Validation, RGB and Taro](https://docsend.com/view/he8x9erkjmphphvn)
- [Understanding RGB Protocol: Everything You Need to Know](https://diba.io/blog/understanding-rgb-protocol)
- [What is the RGB Protocol on Bitcoin?](https://trustmachines.co/learn/what-is-the-rgb-protocol-on-bitcoin)
- [RGB as a Computing Platform](https://rgb.tech/blog/rgb-computing/)
- [RGB release v0.10](https://rgb.tech/blog/release-v0-10/)
- [RGB release v0.7](https://rgb.tech/blog/release-v0-7/)
- [Is Lightning Scaling Bitcoin in a Way Nobody Predicted?](https://blog.bitfinex.com/education/is-lightning-scaling-bitcoin-in-a-way-nobody-predicted/)
- [How Can RGB Improve Bitcoin?](https://blog.bitfinex.com/education/how-can-rgb-improve-bitcoin/)
- [What Does the Bitcoin DeFi Ecosystem Look Like?](https://blog.bitfinex.com/education/what-does-the-bitcoin-defi-ecosystem-look-like/)
- [Is Bitcoin Undervalued?](https://blog.bitfinex.com/education/is_bitcoin_undervalued/)
  
## Videos

- [BH2022: Smart Contracts, Bitcoin in El Salvador, Economic Empowerment and Civil Resistance ](https://www.youtube.com/watch?v=43sqrqfrD9Y)
- [RGB protocol: Asset issuance on Bitcoin and Lightning Network](https://www.youtube.com/watch?v=WBnMiHQCt6g)
- [RGB Update: Smart Contracts For Bitcoin & The Lightning Network](https://www.youtube.com/watch?v=y2Ak970WpkA)
- [SEGUNDA CAMADA do Bitcoin: Liquid Network, RSK, RGB, ARK e Lightning, GUIA dos protocolos L2 no BTC](https://www.youtube.com/watch?v=lqnsh8BWvS8)
- [RGB Protocol - Federico Tenga](https://www.youtube.com/watch?v=6fYB5vILB30)
- [Bitfinex Talks: RGB Protocol and tokenization on top of Bitcoin with Federico Tenga](https://www.youtube.com/watch?v=3tO0I-db4l4)
- [RGB Protocol: Bitcoin Lightning Smart Contracts | BitDevsLA](https://www.youtube.com/watch?v=Mkidb0wjua0)
- [What is the potential of RGB? - Olga Ukolova](https://www.youtube.com/watch?v=6vXu5xYy7I8)

## Podcast

- [SLP439 Federico Tenga – What is RGB for Bitcoin? Iris wallet](https://stephanlivera.com/episode/439/)
 
- [Maxim Orlovsky on Building RGB, Standards for BTC & LN, and Smart Contracts on Bitcoin | E108](https://www.youtube.com/watch?v=mLrKainZgAw)

## Guides

- [Scriptless Atomic Swaps](https://github.com/crisdut/lnpbp-regtest/blob/master/usecases/2_scriptless_atomic_swaps.md)
- [RGB Sandbox](https://github.com/RGB-Tools/rgb-sandbox)


## Libraries

- [RGB-lib](https://github.com/RGB-Tools/rgb-lib)
- [RGB Lib Python bindings](https://github.com/RGB-Tools/rgb-lib-python)
- [RGB Core Library](https://github.com/RGB-WG/rgb-core)
- [RGB Lib Swift bindings](https://github.com/RGB-Tools/rgb-lib-swift)
- [RGB Lib Kotlin bindings](https://github.com/RGB-Tools/rgb-lib-kotlin)
- [RGB Lib Javascript binding](https://github.com/PorticoExchange/rgb-lib-javascript)
- [BPro Library](https://github.com/pandora-prime/bpro)
- [RGB TS](https://github.com/chernyal/rgb)
- [RGB Lib Sample](https://github.com/diamondhands-rgb/rgb-lib-sample)

## Wallets

- [MyCitadel](https://mycitadel.io/) 
- [BitMask](https://bitmask.app/) 
- [Iris](https://github.com/RGB-Tools/iris-wallet-android) 
- [Shiro](https://github.com/diamondhands-dev/shiro-backend)
- [Wallby](https://wallby.app/)

## Exchanges

- [Portico Exchange](https://github.com/PorticoExchange) - DEX with Atomic transactions on Lightning Network
- [Bitswap](https://github.com/BitSwap-BiFi) - DEX AMM on RGB Protocol
- Colorshift - Exchange RGB Assets under Swiss Law
- [Bitifinex](https://www.bitfinex.com/) - Major and Old Exchange in the Bitcoin industry
- [Hodl Hodl](https://hodlhodl.com/) - P2P Lending and Exhcange
- Kaleidoscope - Decentralized exchange protocols (DEX) for Lightning with RGB and other assets

## Explorer

- [RGBex](https://rgbex.io/)

## Registries

- [RGB schemata registry](https://github.com/RGB-WG/schemata-registry)
- [Storm](https://github.com/Storm-WG)
- [Carbonado](https://github.com/diba-io/carbonado)


## Services

- [RGB Minting Service](https://github.com/LukasBahrenberg/rgb-minting-service)
- [RGB NFT Minting Service CLI](https://github.com/V0nMis3s/rgb-nft-minting-service)
- [RGB Lightning Sample](https://github.com/RGB-Tools/rgb-lightning-sample)
- [Bitcoin Pro](https://github.com/pandora-prime/bitcoin-pro)
- [RGB Proxy Server](https://github.com/grunch/rgb-proxy-server)
  
## NFTs

- [DIBA](https://diba.io/)
- [NFT Swap](https://github.com/PorticoExchange/NFT-Swap)
- [RGB Minting Service](https://github.com/LukasBahrenberg/rgb-minting-service)
- [RGB NFT Minting Service CLI](https://github.com/V0nMis3s/rgb-nft-minting-service)

## Companies working of form independent on RGB Protocol

- [RGB Tools](https://github.com/RGB-Tools)
- Portico Labs

## Comapanies support RGB Protocol 

- Portico Labs
- Bitifinex
- HodlHodl
- DIBA
- [Pandora Prime](https://pandoraprime.ch/)
- Fulgur Ventures
- Hojo Foundation

## Others things

- [Bitcoin Protocol](https://github.com/BP-WG)
- [Pandora Prime](https://github.com/pandora-prime)
- [Pandora Network](https://github.com/pandora-network)
- [Prometheus: trustless & scalable machine learning](https://github.com/Prometheus-WG)
- [LNP Node](https://github.com/LNP-WG)
- [reNostr](https://github.com/renostr)
- [Cyphernet](https://github.com/cyphernet-dao)
- Bitfrost

## Extra lists

- [Awesome RGB](https://github.com/louneskmt/awesome-rgb)
- [RGB Resources](https://github.com/fedsten/rgb-resources)

