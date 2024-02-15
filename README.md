# Awesome RGB Protocol 🟢🔵🔴⚡🪙

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
- Tokenized Real State
- Bitcoin as Collateral
- Decentralized Exchanges (AMM, liquidity pool)
- NFTs
- NFT Marketplace
- NFT auction
- Crowdfunding
- Stablecoins (aka. Centralized like USDC and USDT)
- Stablecoins algorithm
- Sythentic stablecoins
- Decentralized identities
- Storage
- Lending
- Atomic Swap
- Submarine Swap
- Wallets
- Explorers
- Machine Learning
- Mint Services
- Social media (accepting payments via Stablecoins or tokens)
- DAOs
- Muti-layer network
- Multisig complex with Miniscript and more
- Scale Layer 1 with Prime, Abraxis
- Compatible with sidechains
- Lightning Service Provider for RGB Assets
- Lightning Nodes
- Virtual Machine (AluVM)
- OTC Exchange
- Cloud Service
- APIs
- Domains names
- LN derivations
- Multipeer channels with Bifrost
- Trustless pegin/pegout by Radiant
- Multichain
- GameFi
- Metaverse
- RWAs
- Compatible with DLCs, Taproot...
- Marketplace for RGB20 assets
- Centralized Exchanges
- Asset Management
- Custodial services
- Derivatives
- Mint services
 
## Status software

Since was released [RGB v0.10](https://rgb.tech/blog/release-v0-10/) anyone can build applications on protocol without breaking consensus or other problems

Developers, companies and users can release products on mainnet (knowing risks involved)

LNP/BP Association is woking in the next version, RGB v0.11, which v0.10 isn't compatible and [will have Liquid](https://x.com/lnp_bp/status/1747930079252951058?s=20),  a sidechain created by the Blockstream and is more stable than v0.10.
## Tech Overview

Little overview around RGB 

![image](https://github.com/22388o/awesome-rgb-protocol/assets/83122757/1fd0399f-58f5-4955-a405-74175d01b609)


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

### Understanding LNP/BP Libraries

-  [BP (Bitcoin Protocol)](https://github.com/BP-WG):

*BP STD: Modern & lightweight implementation of bitcoin standards without rust-bitcoin/miniscript dependencies 

*BP Wallet:  Modern, lightweight & standard-compliant bitcoin wallet runtime & cli without rust-bitcoin dependencies 

*BP Node:  Daemons and tools for Bitcoin transaction index 

*BP Core: Consensus data structures and client-side-validation library for bitcoin protocol 
 
-  [RGB](https://github.com/RGB-WG): 
  
*RGB Core: Consenus  and validation

*RGB STD: WASM and low-level integrations

*RGB Schemata: Standard RGB schemata and schema compiler

*RGB: Command-line tool and  wallet runtime library for desktop and mobile integration

-  [LNP (Lightning Network Protocol)](https://github.com/LNP-WG):
  
*LNP Core: Lightning Network Protocol core library

*LN Types:  Common Rust Lightning Network types 

*LN Node:  Lightning network protocol daemon (suitable for generalized Lightning Network) 

*Lightning Encoding:  Rust implementation of lightning network encoding as defined by BOLTs 

-  [Prometheus](https://github.com/Prometheus-WG):

*Prometheus Spec:  Cryptoeconomically-safe trustless high-load computing on top of Bitcoin 

-  [Storm](https://github.com/Storm-WG):

*Storm Core:  Core components for building storm LNP channels & applications 

*Storm Stored: Storage daemon for Storm and other LNP/BP nodes - an embeddble microservice frontend for different storage backends 

*Storm Node:  Extension daemons for LNP Node implementing Storm protocol 

*Storm Spec:  Specification for Storm: L2/L3 distributed storage and messaging with economic incentivisation leveraging LNP/BP ecosystem 

-  [LNP/BP](https://github.com/LNP-BP):

*LNPBPs:  LNP/BP standards for bitcoin layer 2 & 3 protocols 

*Presentations:  Slides, visuals and video links that explain Bitcoin L2/L3 technological stack development, curated by LNP/BP Standards Association 

*Client Side Validation:  Standard implementation of client-side-validation APIs 

*Rust LNBP:  Library implementing LNPBP standards related to client-side-validation paradigm 

*Invoices:  Libraries for universal LNP/BP invoices covering Bitcoin, LN & RGB (LNPBP-38 standard)

*Docker:  Docker containers by LNP/BP Standards Association 

*Layer1:  Paper on new bitcoin layer 1 design 

- [Strict Types](https://github.com/strict-types):

*Strict Types:  Rust implementation of strict encoding schema library 

*Strict Encoding:  Protobufs for functional programming 

*Spec:  Strict encoding specification 

*Registry:  Registry of strict type libraries 

- [AluVM](https://github.com/AluVM):

*Rust Aluvm:  Rust implementation of AluVM (RISC functional machine) 

*Alure:  AluVM runtime with I/O extensions (like JRE) 

*Aluasm:  AluVM assembler 

*AluVM spec:  Specification of AluVM (algorithmic logic unit VM), its bytecode and assembly language 

### External LNP/BP Libraries

Several teams are working indepent libraries

### [RGB Tools](https://github.com/RGB-Tools)

- RGB Lib: Rust library which provides tools to build cross-platform RGB compatible wallets in a simple fashion, without having to worry about Bitcoin and RGB internals.
  
- RGB Sandbox:RGB sandbox and demo based on RGB version 0.10
  
- RGB Lib Phython: Python library, rgb-lib, for the rgb-lib Rust library, which is included as a git submodule
  
- RGB Lib Stress Test: CLI command to test a few scenarios involving transfers of RGB20 assets between multiple wallets
  
- RGB Lib Swift:  Swift library RgbLib, for the rgb-lib Rust library, which is included as a git submodule
  
- RGB Lib Klottin:  Android library, rgb-lib-android, for the rgb-lib Rust library, which is included as a git submodule
  
- Faucet RGB: Faucets for wallets using RG20 tokens

### Main RGB Standards

- [RGB20: Fungible Assets](https://standards.lnp-bp.org/rgb/lnpbp-0020)
- [RGB21: NFTs Collectibles](https://standards.lnp-bp.org/rgb/lnpbp-0021)
- [RGB22: Digital Identity](https://standards.lnp-bp.org/rgb/lnpbp-0022)
- [RGB23: Audit Logs](https://standards.lnp-bp.org/rgb/lnpbp-0023)
- [RGB24: Domain Names](https://standards.lnp-bp.org/rgb/lnpbp-0024)
- [RGB25: Collectible assets interface](https://github.com/LNP-BP/LNPBPs/blob/master/lnpbp-0025.md)
  

## Protocol 

- [LNP/BP Standards Association](https://github.com/LNP-BP)
- [RGB Working Group repository](https://github.com/RGB-WG)
- [BP Working Group repository](https://github.com/BP-WG)
- [LNP Working Group repository](https://github.com/LNP-WG)
- [Storm Working Group repository](https://github.com/Storm-WG)
- [Prometheus Working Group repository](https://github.com/Prometheus-WG)
- [Strict Types Working Group repository](https://github.com/strict-types)
- [Alu Virtual Machine Working Group repository](https://github.com/AluVM)
- [reNostr Working Group repository](https://github.com/renostr)
- [LNP/BP Association (website)](https://www.lnp-bp.org/)
- [LNP/BP Association (YouTube)](https://www.youtube.com/channel/UCK_Q3xcQ-H3ERwArGaMKsxg)
- [LNP/BP Association (Twitter)](https://twitter.com/lnp_bp)
- [LN/BP Association (Telegram channel)](https://t.me/lnp_bp)

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
- [RGB Blueprint](https://blackpaper.rgb.tech/design/design-principles)
- [bitcoin-dev Trustless 2-way-peg without softfork](https://lists.linuxfoundation.org/pipermail/bitcoin-dev/2023-September/021948.html)
- [bitcoin-dev New BIP to align descriptors, xpub derivation and miniscript](https://lists.linuxfoundation.org/pipermail/bitcoin-dev/2023-September/021946.html)
- [Writing simple contract](https://rgb.tech/program/rust/#basics)
- [Prime resources by LNP/BP Association](https://x.com/lnp_bp/status/1721193382838501866?s=20)
- [RGB Blueprint (technical documentation)](https://github.com/RGB-WG/blueprint)

## Community

- [RGB Telegram](https://t.me/rgbtelegram)
- [RGBaguette](https://t.me/rgbaguette) 
- [RGB Italia](https://t.me/rgbitalia) 
- [RGB Developers](https://t.me/RGBDevelopers)
- [RGB Twitter List](https://twitter.com/i/lists/1582840508933582849/members)
- [RGB Community (Twitter)](https://twitter.com/i/communities/1585365616743022595)
- [RGB Reddit](https://www.reddit.com/r/RGB_protocol/)
- [RGB OGs](https://t.me/RGB_TA_OGs)
- [RGB Chinese group](https://t.me/+sawAp0ZBjWQzOWJl)
- [Single Use Seals](https://t.me/SingleUseSeal)
- [Pepe RGB](https://t.me/pepe_rgb)
- [Bitlight Labs](https://t.me/Bitlightlabs)
- [Pandora Prime](https://t.me/pandoraprime)
- [MyCitadel](https://t.me/mycitadel)
- [DIBA, BitMask & Carbonado](https://t.me/tryDIBA)
- [Iris Wallet](https://t.me/IrisWallet)
- [Peper Friends](https://t.me/pepperfriends)
- [RGBDoge Community](https://t.me/RGB_Doge)
- [UTXO Labs](https://t.me/UTXOLabs)
- [DaPangDunCrypto](https://twitter.com/DaPangDunCrypto) (chinese influencers)

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
- [RGB v0.10 becomes stable](https://rgb.tech/blog/release-v0-10-stable/)
- [Is Lightning Scaling Bitcoin in a Way Nobody Predicted?](https://blog.bitfinex.com/education/is-lightning-scaling-bitcoin-in-a-way-nobody-predicted/)
- [How Can RGB Improve Bitcoin?](https://blog.bitfinex.com/education/how-can-rgb-improve-bitcoin/)
- [What Does the Bitcoin DeFi Ecosystem Look Like?](https://blog.bitfinex.com/education/what-does-the-bitcoin-defi-ecosystem-look-like/)
- [Is Bitcoin Undervalued?](https://blog.bitfinex.com/education/is_bitcoin_undervalued/)
- [CoinEx Institution｜A Brief Analysis of RGB: A Scalable, Confidential Smart Contract Protocol Built on Bitcoin](https://coinex.medium.com/coinex-institution-a-brief-analysis-of-rgb-a-scalable-confidential-smart-contract-protocol-built-bc883829af51)
- [What is the RGB Protocol on Bitcoin?](https://trustmachines.co/learn/what-is-the-rgb-protocol-on-bitcoin/)
- [The RGB Network](https://thebitcoinmanual.com/blockchain/rgb-chain/)
- [Explaining RGB Protocol Exploring a New Second Layer for Bitcoin Asset Issuance](https://blocking.net/40648/rgb-protocol-is-a-new-second-layer-for-issuing-bitcoin-assets/)
- [How RGB Colors Coins in Secret](https://cryptoquick.com/files/How%20RGB%20Colors%20Coins%20in%20Secret.pdf)
- [Driving Mass Adoption of Crypto: How the RGB Protocol is Illuminating the Future of Bitcoin](https://www.cointime.com/news/driving-mass-adoption-of-crypto-81155)
- [Preseting: Bitswap](https://medium.com/@porticoexchange/presenting-bitswap-a3b59d8082a1)
- [RGB20 and RGB21 on Bitcoin mainnet with BitMask](https://dibaglobal.medium.com/rgb20-and-rgb21-on-bitcoin-mainnet-with-bitmask-35c520bd4e6d)
- [Bitcoin RGB Protocol Ten Thousand Words Research Report: Can Lightning Network and smart contracts lead a new round of technological changes? Panoramic dismantling of its development history, technical principles, ecological status and five major risks and challenges(Relatory in Chinese)](https://research.web3caff.com/zh/archives/11414?ref=0)
- [Tranascript about Prime presentation at PoW Summit](https://x.com/kanzure/status/1706679211140805107?s=46&t=gvP5ENKSm34hlhVAka2BsA)
- [RGB protocol by UTXO Management](https://www.utxo.management/content/files/2023/10/UTXO_Management_RGB_Report.pdf)
- [REPORT: UTXO Management X BM Pro Present RGB Research Report](https://bmpro.substack.com/p/report-utxo-management-x-bm-pro-present)
- [RGB: An In-Depth Analysis of the RGB Bitcoin Layer 2 Approach](https://www.utxo.management/rgb-an-in-depth-analysis/)
- [Taking stock of BTC ecological protocols, which protocols can win the last prize?](https://followin.io/en/feed/6456797)
- [Understanding The "Bitcoin L2 Trilemma"](https://bitcoinmagazine.com/technical/understanding-the-bitcoin-l2-trilemma)
- [A Brief Overview on RGB — Can RGB Replicate The Ordinals Hype](https://www.bitget.com/news/detail/12560603830569)
- [Off-Chain Transactions: The Evolution of Bitcoin Asset Protocols](https://mirror.xyz/0x5CCF44ACd0D19a97ad5aF0da492AC0388469DfE9/h7XChxETK-cBfGdc0sTq_cCuWeo13-sp1j-g0ZYoYdc)
- [Cosminmart(Bitlight Labs) interview](https://www.panewslab.com/zh/articledetails/f50h5ynw.html)
- [RGB learning resources collection](https://mirror.xyz/dapngdun.eth/9F5ef9YCwbVSvopEeRxIKsARCsQvOsQYOvS7GAYokqI)
- [About RGB: OP Crypto Weekly X (Twitter) thread and it got longer](https://opcryptovc.medium.com/about-rgb-protocol-op-crypto-weekly-x-twitter-thread-and-it-got-longer-7031fe39439b)
- [Paolo Ardoino, CEO of Tether: “In the future, data centers will be used as weapons”](https://atlas21.com/it/ardoino-i-data-center-saranno-usati-come-armi)
- [Paolo Ardoino sees RGB as 'best opportunity' to issue stablecoins on Bitcoin](https://www.theblock.co/post/258350/bitfinex-rgb-bitcoin-stablecoins)
- [Evolution and challenge of BTC expansion from asset issuance](https://medium.com/@ACCapital1/evolution-and-challenge-of-btc-expansion-from-asset-issuance-d8caba8aeb07)
- [BitMask & RGB w/ Hunter Beast](https://cryptoquick.com/files/BitMask-RGB-v2.pdf)
- [Bitcoin Upper Layers Explained: Types, Origins, & Future](https://blog.rootstock.io/noticia/bitcoin-layers/)
- [The next hot spot in the BTC ecosystem? Noteworthy projects on the RGB protocol](https://www.blocktempo.com/take-stock-of-noteworthy-projects-on-the-rgb-protocol/)
- [Understanding the RGB Protocol: Bridging Bitcoin and Smart Contract](https://beosin.com/resources/understanding-the-rgb-protocol-bridging-bitcoin-and-smart-contract?lang=en-US)
- [Introduction of RGB](https://medium.com/@jesse06/introduction-of-rgb-92c235b2b2dc)
- [What Is the RGB Protocol? A Beginner's Guide](https://www.samara-ag.com/market-insights/rgb-protocol)
- [This Protocol Can Make Bitcoin More Scalable and Private](https://bitpinas.com/pr/rgb-protocol-bitcoin-private/)
- [Bitcoin's RGB Protocol: Issuing Assets and Tokens on the Lightning Network](https://www.daijiworld.com/news/newsDisplay?newsID=1142106)
- [The RGB protocol in the BTC ecosystem is about to explode. Let’s take a look at the projects worth paying attention to in the RGB ecosystem.](https://www.odaily.news/en/post/5191287)
- [Apart from $Ordi, how can we invest in BTC ecosystem?](https://medium.com/@infinitas.contact/apart-from-ordi-how-can-we-invest-in-btc-ecosystem-8370931a50bd)
- [The New Narrative of Inscription — Under the Support of Different Ecosystems](https://tokeninsight.com/en/research/market-analysis/the-new-narrative-of-inscription-under-the-support-of-different-ecosystems)
- [Why is Bitcoin RGB protocol the ultimate form of smart contracts?](https://medium.com/@infinitas.contact/why-is-bitcoin-rgb-protocol-the-ultimate-form-of-smart-contracts-0d2f8c57a36c)
- [Decoding the Complex Landscape of Bitcoin Layer 2: Navigating Challenges and Building Narratives](https://wublock.substack.com/p/decoding-the-complex-landscape-of)
- [CGV Research | From Colored Coins, Mastercoin/Omni to Ordinals/BRC20, a Comprehensive Analysis of Technological Evolution in the Bitcoin Ecosystem](https://wublock.substack.com/p/cgv-research-from-colored-coins-mastercoinomni)
- [From Asset Issuance to BTC Scalability: Evolution and Challenges](https://www.gate.io/learn/articles/from-asset-issuance-to-btc-scalability/1030)
- [Bitcoin Ecosystem — The Engine for the Next Bull Market](https://www.bitget.com/blog/articles/bitcoin-ecosystem-the-engine-for-the-next-bull-market)
- [RGB Protocol, Poised for Takeoff](https://www.gate.io/learn/articles/rgb-protocol-poised-for-takeoff/1090)
- [BiHelix: An essential compilation of RGB ecological projects](https://medium.com/@bihelix.contact/bihelix-an-essential-compilation-of-rgb-ecological-projects-25e0fe049469)
- [Quais novas tecnologias devem surgir nos próximos anos no Bitcoin?](https://portaldobitcoin.uol.com.br/quais-novas-tecnologias-devem-surgir-nos-proximos-anos-no-bitcoin/)
- [2024 Crypto Market Outlook by Coinsbase Institutiona](https://coinbase.bynder.com/m/c8c6fdc663f44b5/original/2024-Crypto-Market-Outlook-V3.pdf)
- [RGB Bolsters Bitcoin and Lightning Network’s Scalability and Privacy Capabilities](https://mpost.io/rgb-bolsters-bitcoin-and-lightning-networks-scalability-and-privacy-capabilities/)
- [Renaissance of Bitcoin Scaling IV — RGB](https://lbanklabs.medium.com/renaissance-of-bitcoin-scaling-iv-rgb-0ce0a3c8a656)
- [RGB Protocol: A Revolutionary Smart Contract System in the Bitcoin Ecosystem](https://medium.com/@sicily0913/rgb-protocol-a-revolutionary-smart-contract-system-in-the-bitcoin-ecosystem-5a9777ee124c)
- [10,000 Words Research Report: Bitcoin Ecological RGB Protocol and Development Progress](https://www.laitimes.com/en/article/6bdfb_6rpq5.html)
- [All You Need to Know About the RGB Protocol](https://www.gate.io/learn/articles/all-you-need-to-know-about-the-rbg-protocol/1196)
- [Exploring the Landing Paths for Bitcoin Layer 2 Ecosystem ](https://wublock.substack.com/p/exploring-the-landing-paths-for-bitcoin)
- [A hundred flowers are blooming in Bitcoin Layer 2, a look at the progress of 6 major mainstream protocols](https://blockcast.it/2024/01/17/the-state-of-top-bitcoin-layer2-projects/)
- [The Rising Synergy Between Liquid Network and RGB](https://www.btctimes.com/news/the-rising-synergy-between-liquid-network-and-rgb)
- [Detailed introduction to RGB, BitVM, and Nostr](https://www.techflowpost.com/article/detail_16046.html)
- [Bitlight Labs Seed Round Successfully Concluded](https://medium.com/@bitlightlabs/bitlight-labs-seed-round-successfully-concluded-4086e0064c8c)
- [RGB++ Protocol Light Paper](https://talk.nervos.org/t/rgb-protocol-light-paper/7733/3)
- [RGB++: Contributing to Orthodox Bitcoin L2](https://www.coinlive.com/news/rgb-contributing-to-orthodox-bitcoin-l2)
  ## Videos

- [BH2022: Smart Contracts, Bitcoin in El Salvador, Economic Empowerment and Civil Resistance ](https://www.youtube.com/watch?v=43sqrqfrD9Y)
- [RGB protocol: Asset issuance on Bitcoin and Lightning Network](https://www.youtube.com/watch?v=WBnMiHQCt6g)
- [RGB Update: Smart Contracts For Bitcoin & The Lightning Network](https://www.youtube.com/watch?v=y2Ak970WpkA)
- [SEGUNDA CAMADA do Bitcoin: Liquid Network, RSK, RGB, ARK e Lightning, GUIA dos protocolos L2 no BTC](https://www.youtube.com/watch?v=lqnsh8BWvS8)
- [RGB Protocol - Federico Tenga](https://www.youtube.com/watch?v=6fYB5vILB30)
- [Bitfinex Talks: RGB Protocol and tokenization on top of Bitcoin with Federico Tenga](https://www.youtube.com/watch?v=3tO0I-db4l4)
- [RGB Protocol: Bitcoin Lightning Smart Contracts | BitDevsLA](https://www.youtube.com/watch?v=Mkidb0wjua0)
- [What is the potential of RGB? - Olga Ukolova](https://www.youtube.com/watch?v=6vXu5xYy7I8)
- [Prime](https://www.youtube.com/live/V3vvybsc1A4?feature=shared&t=23631)
- [Ṕrime presentation at PoW Summit](https://www.youtube.com/watch?v=uq01tDKvxOg) - starting from 7:25:21
- [E125: RGB Deep-Dive & Scaling Bitcoin with Hunter Beast - Director of Engineering at DIBA](https://www.youtube.com/watch?v=iZJQ2J-uNtE)
- [Ordinals and Layer 2 - Bitcoin Amsterdam 2023](https://youtu.be/YM_b6q7l0H4?t=12829)
- [Protocols on the top of Bitcoin - Debate](https://www.youtube.com/watch?v=7L-RKqgRr7Y)
- [Radiant, Prime and RGB - Bitcoin Amsterdam 2023](https://www.youtube.com/watch?v=E1yvIOXz8Tg)
- [RGB Protocol Explained - Hunter Beast | Denver BitDevs 11/2/2023](https://www.youtube.com/watch?v=oeoBSYB0H7U)
- [Modernizing RGB with Taproot at 2022-04-02](https://www.youtube.com/watch?v=7sBAtv88mSE&ab_channel=LNPBPStandardsAssociation)
- [Asset Issuance On Bitcoin: Discovering The RGB Protocol - Federico Tenga (Part.1)](https://www.youtube.com/watch?v=23_IKrIonQk)
- [Asset Issuance On Bitcoin: Discovering The RGB Protocol - Federico Tega (Part.2)](https://www.youtube.com/watch?v=t3U8XsRndvc)
- [和PEPE-RGB创始人 一起聊聊赚RGB生态，可能彩蛋哦｜In talk with Pepe-RGB, one of the first project for RGB ecosystem](https://www.youtube.com/watch?v=m3U0h7qWj5k)
- [中文区第一次！和DIBA/Bitmask团队Gideon一起聊聊RGB生态 ｜ In talk of RGB/Bitcoin with Gideon from DIBA/Bitmask team ](https://www.youtube.com/watch?v=lNjeKGJKAHQ)
- [The first RGB trading platfrom | RGB生态的第一个交易平台？我们有什么可以期待的](https://youtu.be/2L3_RWLhVTM?si=vu8CWXf_wGvYdJ1l)
- [A Talk with Alex the founder of Cororo | The first BTC phone with RGB node ｜第一个BTC手机？挖矿/depin/RGB节点？](https://www.youtube.com/watch?v=5MXx7iu9Iy4&t=2149s)
- [RGB HMP with Diba & Bitmask team](https://www.youtube.com/watch?v=WZN36y8UWGc)
- [How will the RGB Protocol Benefit the Bitcoin Ecosystem?](https://www.youtube.com/watch?v=ntHJ_S1PKCg)
- [Meet Kilian from Boltz.exchange | 和Boltz创始人聊聊闪电网络，Liquid和RGB ](https://www.youtube.com/watch?v=h0Dm-RtKAL4)
- [和Taproot Asset协议的提拉米苏钱包的创始人聊一聊，空投怎么发，Adam代币持有人有什么福利？｜未来和RGB融合的可能性](https://www.youtube.com/watch?v=xRPt-Yh6cd0)

## Podcast

- [SLP439 Federico Tenga – What is RGB for Bitcoin? Iris wallet](https://stephanlivera.com/episode/439/)
 
- [Maxim Orlovsky on Building RGB, Standards for BTC & LN, and Smart Contracts on Bitcoin | E108](https://www.youtube.com/watch?v=mLrKainZgAw)

- [SLP501 RGB Walkthrough with Maxim Orlovsky](https://stephanlivera.com/episode/501/)

- [RGB & Art with Diba team](https://twitter.com/i/spaces/1eaJbgkZZzaxX?s=20)

- [Anatomy of RGB21](https://x.com/trydiba/status/1720527686706032694?s=20)

- [Exploring the Future Potential of RGB Ecosystem with Bitlight Labs, Bitmask & Diba, Spank Exchange, Pepper and DaPangGun](https://x.com/ACCapital1/status/1729815369798344808?s=20)

- [e17 The Bitcoin Contracting Layer - RGB with Maxim](https://anchor.fm/dtrhole/episodes/e17-The-Bitcoin-Contracting-Layer---RGB-with-Maxim-Orlovsky-eqdfh6)

- [Prime & Abraxas - TWitter Spaces](https://x.com/DesiBitcoinShow/status/1747153575594410378)

## Education

- [RGB Journey](https://github.com/BitcoinOS-Labs/rgb-journey)
- [LN/BP Education](https://geyser.fund/project/lnpbpeducation)
- [Mastering Bitcoin, 3rd Edition](https://www.oreilly.com/library/view/mastering-bitcoin-3rd/9781098150082/) - with RGB protocol
  
## Guides

- [Scriptless Atomic Swaps](https://github.com/crisdut/lnpbp-regtest/blob/master/usecases/2_scriptless_atomic_swaps.md)
- [RGB Sandbox](https://github.com/RGB-Tools/rgb-sandbox)
- [RGB21 Assets workflow](https://gist.github.com/rkedez/fef785f4c12a2be1253659a7ef28b3b8)
- [RGB Install](https://rgb.tech/install/)
- [RGB in Rust](https://rgb.tech/program/rust/)
- [Zero-code contracts](https://rgb.tech/power-user/#issue)
- [Programming with Contractum](https://rgb.tech/program/contractum/)


## Libraries and CLIs

- [RGB-lib](https://github.com/RGB-Tools/rgb-lib)
- [RGB Lib Python bindings](https://github.com/RGB-Tools/rgb-lib-python)
- [RGB Core Library](https://github.com/RGB-WG/rgb-core)
- [RGB STD](https://github.com/RGB-WG/rgb-std)
- [RGB Schemata](https://github.com/RGB-WG/rgb-schemata)
- [RGB CLI](https://github.com/RGB-WG/rgb)
- [LNP Core](https://github.com/LNP-WG/lnp-core)
- [Lightning Encoding](https://github.com/LNP-WG/lightning_encoding)
- [LN Types](https://github.com/LNP-WG/ln-types)
- [BP Core](https://github.com/BP-WG/bp-core)
- [BP STD](https://github.com/BP-WG/bp-std)
- [BP Wallet](https://github.com/BP-WG/bp-wallet)
- [Storm Core](https://github.com/Storm-WG/storm-core)
- [Storm Stored](https://github.com/Storm-WG/storm-stored)
- [Descriptor Wallet](https://github.com/BP-WG/descriptor-wallet)
- [Clien Side Validation](https://github.com/LNP-BP/client_side_validation)
- [Rust LNPBP](https://github.com/LNP-BP/rust-lnpbp)
- [Invoices](https://github.com/LNP-BP/invoices)
- [RGB Lib Swift bindings](https://github.com/RGB-Tools/rgb-lib-swift)
- [RGB Lib Kotlin bindings](https://github.com/RGB-Tools/rgb-lib-kotlin)
- [BPro Library](https://github.com/pandora-prime/bpro)
- [RGB TS](https://github.com/chernyal/rgb)
- [RGB Lib Sample](https://github.com/diamondhands-rgb/rgb-lib-sample)

## Token and NFTs Example

- [USDT example by OneForaAlone](https://github.com/oneforalone/rgb20-usdt)
- [USDT Demo by Bitlight Labs and co-authored by OneForaAlone](https://github.com/bitlightlabs/rgb20-usdt)
- [UTXO token by UTXO Labs and co-authored by OneForaAlone ](https://github.com/UTXOLabs/UTXO-RGB20)
- [Pepe RGB](https://pepe-rgb.wtf/)
- [RGB21 Assets workflow](https://gist.github.com/rkedez/fef785f4c12a2be1253659a7ef28b3b8)
- [Single Use Seals](https://t.me/SingleUseSeal)
- [Doge RGB](https://www.rgbdoge.xyz)
- [Assets: BTN & USDN by Pandora Prime](https://github.com/pandora-prime/assets)
- [Assets DEX: Amazon, Apple, Real State by Bitswap](https://github.com/BitSwap-BiFi/assets-dex)
- [PandaPo](https://pandapo.xyz/)
- [BitMan](https://bitman.city/)
- [BaseDao](http://thebasedao.xyz/)
- MRGB

## Wallets

- [MyCitadel](https://mycitadel.io/) 
- [BitMask](https://bitmask.app/) 
- [Iris Wallet](https://github.com/RGB-Tools/iris-wallet-android) 
- [Shiro](https://github.com/diamondhands-dev/shiro-backend)
- [Wallby](https://wallby.app/)
- [Bitcoin Tribe](https://bitcointribe.app/)
- [Tiramisu Wallet](https://mainnet.tiramisuwallet.com/walletapp/)
- [Keeper Wallet](https://bitcoinkeeper.app/)
- [Aqua Wallet](https://aquawallet.io/)
- Bitlight Wallet
- UTXO Wallet
- Invebit Wallet
- [XRGB Wallet](https://app.xrgb.xyz/login) (mobile, extension and web)
  
## Exchanges

- [Bitswap](https://github.com/BitSwap-BiFi) - DEX AMM on RGB Protocol and Lightning Network
- [RGBFI](https://twitter.com/RGBFIOfficial) - DEX AMM (copy/paste from Bitswap)
- Colorshift - Swap RGB Assets under Swiss Law
- [Bitifinex](https://www.bitfinex.com/) - Major and Old Exchange in the Bitcoin industry
- [Hodl Hodl](https://hodlhodl.com/) - P2P Lending and Exhcange
- [Bitlight Labs](https://bitlightlabs.com/) - Marketplace for tokens and NFTs
- [Diba](https://diba.io/) - Marketplace for UDAs
- [AMM DEX Demo by Melvin Carvalho](https://play-grounds.github.io/nosdav/swapstr.html) - Demo AMM for swap RGB assets
- [UTXO Exchange](https://beta.utxoexchange.xyz/) - Exchange with Marketplace for RGB20 and RGB21 tokens
- [Ordi Finance](https://doc.ordifinance.xyz/) - Bridge beteween RGB, LN, ETH and DEX AMM
- [BitRGB](https://bitrgb.network/) - Achieving Infinite Scalability for web3 Asset Issuance and Trading
- [Tiramisu Wallet](https://mainnet.tiramisuwallet.com/walletapp/) - Wallet and Exhange integrated
- [Sax Bridge](http://sax.exchange/) - Exchange and Bridge between RGB20<>EVM
- [Yellow](https://yellow.money/) - Cross-chain AMM DEX
- [Bitrans](https://www.bitrans.io/) - DEX with spot and derivatives
- [PalleteRGB](https://palettergb.com) - Marketplace for RGB20 and RGB21 assets with trading
  
## Explorer

- [RGBex](https://rgbex.io/)
  
## Registries

- [RGB schemata registry](https://github.com/RGB-WG/schemata-registry)
- [Storm](https://github.com/Storm-WG)
- [Carbonado](https://github.com/diba-io/carbonado)
- [Mindstr](https://mindstr.org/?map=https%3A%2F%2Fnosdav.net%2Fmelvin%2Fmm%2Frgb%2Findex.json)
-  Fatline Protocol
-  [BitMask Asset Registry](https://beta.bitmask.app/#/registry)

## Nodes

- [RGB Lightning Node](https://github.com/RGB-Tools/rgb-lightning-node)
- [BP Node](https://github.com/BP-WG/bp-node)
- [LNP Node](https://github.com/LNP-WG/lnp-node)
- [Storm Node](https://github.com/Storm-WG/storm-node)


## Asset Management and Tokenization

- [BitRGB](https://bitrgb.network/)
- [Hercle](https://www.hercle.financial/)
- [Invebit](https://www.invebit.com/)

## DAOs

- [BaseDao](http://thebasedao.xyz/)

## Games

- [Infinite Fleet](https://www.infinitefleet.com/)

## Services

- [RGB Minting Service](https://github.com/LukasBahrenberg/rgb-minting-service)
- [RGB NFT Minting Service CLI](https://github.com/V0nMis3s/rgb-nft-minting-service)
- [RGB Lightning Sample](https://github.com/RGB-Tools/rgb-lightning-sample)
- [Bitcoin Pro](https://github.com/pandora-prime/bitcoin-pro)
- [RGB Proxy Server](https://github.com/grunch/rgb-proxy-server)
- [RGB Lightning Node](https://github.com/RGB-Tools/rgb-lightning-node)
- [RGB Lightning Node API](https://rgb-tools.github.io/rgb-lightning-node/)
- SLR (Security Lightning RGB)
- Fatline Protocol
- [Bitcoin Waila](https://github.com/MutinyWallet/bitcoin-waila)
- [NFT on RGB](https://github.com/palutz/nft_on_rgb)
- [Faucet RGB](https://github.com/RGB-Tools/faucet-rgb)
- [RGB CLI Assistant by OpenAI](https://chat.openai.com/g/g-Vo6HpNQSK-rgb-cli-assistant)
- [RGB++ protocol](https://talk.nervos.org/t/rgb-protocol-light-paper/7733/3)
  
## NFTs

- [DIBA](https://diba.io/)
- [RGB Minting Service](https://github.com/LukasBahrenberg/rgb-minting-service)
- [RGB NFT Minting Service CLI](https://github.com/V0nMis3s/rgb-nft-minting-service)
- [NFT on RGB](https://github.com/palutz/nft_on_rgb)
- [Scarce City](https://scarce.city/)
- [UTXO Exchange](https://beta.utxoexchange.xyz/)


## Companies working of form independent on RGB Protocol

- [RGB Tools](https://github.com/RGB-Tools)

## Comapanies support RGB Protocol 

- [Bitifinex](https://www.bitfinex.com/)
- [HodlHodl](https://hodlhodl.com/)
- [DIBA](https://diba.io/)
- [Pandora Prime](https://pandoraprime.ch/)
- [Fulgur Ventures](https://fulgur.ventures/)
- [Hojo Foundation](https://twitter.com/hojofoundation)
- [Bitlight Labs](https://bitlightlabs.com/)
- [Bitswap](https://github.com/BitSwap-BiFi)
- [Bihelix](https://www.bihelix.net/)
- [BitcoinOS Labs](https://github.com/BitcoinOS-Labs)
- [Bithyve](https://github.com/bithyve)
- [Invebit](https://www.invebit.com/)
- [CivKit](https://github.com/civkit)
- [Bacademy](https://bcademy.it/en/)
- [Mutiny Wallet](https://github.com/MutinyWallet/bitcoin-waila)
- [Iris Wallet](https://github.com/RGB-Tools/iris-wallet-android)
- [Tiramisu Wallet](https://mainnet.tiramisuwallet.com/walletapp/)
- [RGB Tools](https://github.com/RGB-Tools)
- [Hercle](https://www.hercle.financial/)
- [Diamond Hands](https://www.diamondhands.community/)
- [Scarce City](https://scarce.city/)
- [UTXO Exchange](https://beta.utxoexchange.xyz/)
- [Waterdrip Capital](https://waterdrip.io/)
- [Satoshi Lab](https://twitter.com/SatoshiLab_)
- [Web3Labs.club](https://twitter.com/Web3LabsClub)
- [LightningNetwork+](https://lightningnetwork.plus/)
- [Ordi Finance](https://doc.ordifinance.xyz/)
- [BitRGB](https://bitrgb.network/)
- [Yellow](https://yellow.money/)
- Cororo
- [Lorenzo](https://www.lorenzo-protocol.xyz/home)
- [BitMan](https://bitman.city/)
- [Uniport](http://uniport.network/)
- [RGBFI](https://twitter.com/RGBFIOfficial)
- [Sax Bridge](http://sax.exchange/)
- [Keeper Wallet](https://bitcoinkeeper.app/)
- [Bitrans](https://www.bitrans.io/)
- [Infinite Fleet](https://www.infinitefleet.com/)
- [Pepe RGB](https://pepe-rgb.wtf/) (project)
- [Single Use Seals](https://t.me/SingleUseSeal) (project)
- [Peper Friends](https://t.me/pepperfriends)  (project)
- [BaseDao](http://thebasedao.xyz/)
- [Jan3](https://jan3.com)
- [Infinite Fleet](https://www.infinitefleet.com/)
- [MagicRGBMoney](https://www.magicrgbmoney.com/)
- [XRGB](http://xrgb.xyz/)
- [PalleteRGB](https://palettergb.com)
- [Nervos Network](https://www.nervos.org/)      
- [Doge RGB](https://www.rgbdoge.xyz) (project)
- [PandaPo](https://pandapo.xyz/) (project)
- MRGB (project)
- [DaPangDunCrypto](https://twitter.com/DaPangDunCrypto) (chinese influencers)

## Others things

- [Bitcoin Protocol](https://github.com/BP-WG)
- [Pandora Network](https://github.com/pandora-network)
- [Pandora Core](https://github.com/pandoracore/)
- [Prometheus: trustless & scalable machine learning](https://github.com/Prometheus-WG)
- [reNostr](https://github.com/renostr)
- [Cyphernet](https://github.com/cyphernet-dao)
- [Bifrost](https://www.rgbfaq.com/glossary/bifrost)
- [Prime](https://github.com/LNP-BP/layer1)
- [Flossverse](https://github.com/flossverse)
- [Abraxis](https://github.com/cryptoquick/abraxis/)
- Abraxas
- Handron
- Kaleidoscope
- [The 9th Proof of Folding - A new proposal for Prime](https://github.com/adambor/The9thProofOfFolding)

## Extra lists

- [Awesome RGB by Lounès Ksouri](https://github.com/louneskmt/awesome-rgb) 
- [Awesome RGB by BitcoinOS Labs](https://github.com/BitcoinOS-Labs/awesome-rgb)
- [RGB Resources by Federico Tenga](https://github.com/fedsten/rgb-resources)

## Disclaimer

Authors of this list is not responsible for eventual issues with third party projects be trading, speculation or any other thing. 

Please do your own research

## Contributors

<a align="center" href="https://github.com/22388o/awesome-rgb-protocol/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=22388o/awesome-rgb-protocol" />
</a>
