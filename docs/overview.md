---
title: "Overview"
---

# General Overview

Secret Network is a blockchain protocol that enables decentralized applications to perform encrypted computations. The Rust code that enables applications to use private data is referred to as a “Secret Contract” on Secret Network. Secret Contracts are similar to smart contracts, such as those used with Ethereum. The key difference is that Secret Contracts can take encrypted inputs and produce encrypted outputs, without exposing any data while it is in-use. In addition, a contract state (its internal, persisted database), remains encrypted throughout executions.

Data on blockchains is public by default. This is a problem for applications which make use of sensitive information, such as user data, personally identifiable information (PII), votes, or moves in a game like rock-paper-scissors or poker. The Secret Network aims to solve this problem by enabling data-in-use privacy through private computation for decentralized applications.

For example, a developer could create a voting application where individual votes are never revealed, but the overall results are provably correct. Additionally, a credit scoring application could generate a score based on verified data submitted by users, without ever seeing that sensitive data (or storing it on-chain). Many applications require data privacy, which is especially difficult to achieve in blockchain-based applications.

The Secret Network is decentralized, so governance decisions are made collectively through votes conducted by the community. The network is run by delegators and validators who propose blocks according to a delegated proof-of-stake model. Node operators earn SCRT rewards for proposing new blocks. Users pay SCRT to the network as fees in order to have their transactions included.

The Secret Network was built with the Cosmos SDK using Tendermint for consensus. Enigma is a company introducing a privacy-preserving applications and ecrypted computation services. As part of this work, Enigma is a core contributor to the Secret Network.

To achieve data privacy, the Secret Network relies on a combination of key management and encryption protocols, along with Trusted Execution Environment (TEE) technology.

![contracts](./images/diagrams/contracts.png)


# Commonly Asked Questions

### What's so special about Secret Network?
Secret Network combines the best features of decentralized, open-source networks and blockchains with the benefits of data privacy and improved usability. These improvements are critical for achieving mass adoption.

We want to enjoy the benefits of [smart contracts](https://en.wikipedia.org/wiki/Smart_contract) and decentralized applications (or dApps): they are robust, unstoppable, censor-resistant and transparent. But blockchains, and by extension smart contracts, have one glaring problem that is often overlooked — all data stored on them is public. In that sense, blockchains are worse than anything that came before them when it comes to privacy. Instead of trusting your data with a single organization (e.g., as is the case with Facebook, Google, your bank, etc), you now have to trust *everyone.* Secret contracts and Secret Apps combine these benefits of dApps but add the ability to keep data private, helping remove one of the biggest barriers to mass adoption of the decentralized web. 

### What are secret contracts and Secret Apps?
"Secret contracts" are _privacy-preserving_ smart contracts built on Secret Network. Smart contracts (in this context) are essentially self-executing pieces of code that are managed on a blockchain. Secret contracts improve on regular smart contracts in that they not only solve for _correctness_, but also for _data privacy_. Secret contracts are written in the [Rust programming language](https://www.rust-lang.org). Secret Apps utilize the capabilities of secret contracts to enable unique use cases that empower users and increase opportunities for growth and impact.

>Learn more on the [Protocol](/protocol.html) page.

### Why privacy?
Members of our community, including secret node operators and Secret App developers, believe that **privacy is a fundamental human right and a public good.** Privacy needs to be protected and supported by the technologies we use in daily life. However,  an overly centralized internet and large data monopolies have put our privacy, our security, and our society at risk. That's why we are dedicated to building solutions with privacy at their core, empowering users to take and keep control of their valuable information. Privacy makes the applications we rely on more usable and more secure - and when privacy is not protected, neither are we.

### Why blockchain?
By using blockchain, a decentralized network of computers can reach consensus on the state of the network while remaining open and permissionless. Secret Network is built on [Cosmos SDK / Tendermint](https://tendermint.com/sdk), a popular blockchain framework, allowing for a wide variety of organizations and individuals to participate in our community and network. The only way to build a sustainable foundation for privacy-first applications is by creating an open, diverse, and transparent culture, united by the purpose of data dignity for all!

### What is programmable privacy?
Secret Network is focused on achieving _[programmable privacy](https://blog.scrt.network/programmable-privacy/)_. Most privacy solutions in the blockchain space today concentrate only on _transactional privacy_, specifically obscuring data on senders or receivers of transactions. Programmable privacy is a much more expansive vision, as a transaction is just one (trivial) type of computation. Secret Network allows applications to use encrypted inputs, encrypted outputs, and encrypted state, meaning we can enable groundbreaking new use cases for smart contracts and decentralized applications.

### What does Secret Network help solve?
Everything! Which applications would you use every day if they could not protect you or your data? When you use blockchains today for any purpose, you are forced to compromise on privacy. Any decentralized applications built on Secret Network benefit from its privacy protections. Our community is primarily focused on use cases that help us achieve our stated mission: to advance privacy as a human right and a public good; to empower individuals through development and use of decentralized technologies; and to protect freedom and create more valuable systems by eliminating data monopolies.

*Sample use cases include:* privacy-preserving credit scoring and lending; private on-chain auctions for cryptoart and other digital collectibles; decentralized access control; secret voting for collective decision-making; privacy-preserving machine learning; and many more applications in the fields of decentralized finance, gaming, healthcare, and dozens of other industries.

### What is SCRT?
SCRT (pronounced "Secret") is the native coin of the Secret Network. This means SCRT is used to pay fees and transfer value on the network. Secret nodes must stake SCRT in order to operate on the network, and in return they receive fees and network rewards in SCRT. When nodes go offline, they can be "slashed" and lose a portion of their SCRT stake. Holders of SCRT who are not operating nodes may "bond" their stake to a specific node in order to become a _delegator_. Delegators have an opportunity to earn a share of fees and network rewards by supporting a particular set of validators.

Another utility for SCRT is governance of the network. Secret nodes can create and vote on governance proposals using SCRT, allowing for decentralized control of the network.

>Learn more on the [Network](/network.html) page

### What are Trusted Execution Environments, and why do we use them?
[Trusted Execution Environments](https://en.wikipedia.org/wiki/Trusted_execution_environment) (TEEs) are special enclaves inside a computer that function like a "black box", allowing computations to occur _confidentially_ inside of them. They are utilized in a broad range of everyday hardware, including the fingerprint readers in smartphones. Secret nodes in the network use these secure enclaves to protect the data used by secret contracts.

While our community is constantly exploring other innovative privacy solutions (such as multi-party computing, homomorphic encryption, private set intersection, etc.), they are simply not practical to use in production for applications today. There are always tradeoffs between scalability, performance, and security, and today secure enclaves provide the best option for protecting data privacy in a decentralized network. We continue to explore and research other solutions!

### What is Cosmos, and why are you using their technologies?
[Cosmos](https://cosmos.network/) represents a standard approach to developing scalable and interoperable blockchain applications. We believe the Cosmos SDK, Tendermint and Inter-Blockchain Communication Protocol (IBC) are groundbreaking since they are looking ahead to a future of many interconnected, app-specific blockchains. We're excited to see how Secret Network can bring more privacy solutions to the Cosmos ecosystem. [Learn more about this on our blog.](https://blog.scrt.network/secret-hub/)

### Is Secret Network a "Layer One" or "Layer Two" solution?
Secret Network has its own consensus and provides privacy for smart contracts deployed on the network, without Secret Network needing to interoperate with any other blockchain. We have often referred to this as "blockchain independence", but based on this description, others would call Secret Network a "Layer One" blockchain. However, part of our vision has always been bringing privacy to *every* blockchain. This means our community is continuing to explore key "Layer Two" functionality for Secret Network, such as by utilizing [IBC](https://cosmos.network/ibc) / Cosmos interoperability, building an Ethereum bridge, or other means.

*Interested in helping expand this guide? You can [contribute to this page!](https://github.com/enigma/SecretNetwork)*

## Secret Contracts and Use Cases
Decentralized technologies need privacy at their core in order to be secure and usable. Secret contracts (smart contracts on Secret Network) utilize encrypted inputs, encrypted outputs and encrypted state. This greatly improves usability of existing blockchain applications and expands the scope of products that can be built on public blockchains.

Below we highlight some existing use cases for which Secret Network can provide clear performance, security, and usability advantages:

### Access Control / Digital Content Management
Used for monetization of digital content in decentralized web, such applications would store a decryption key (secret) to the content in the encrypted secret contract state, and when users make the required payment (triggering event), the secret contract will share a decryption key (secret) that is unique to each user. This use-case is not possible to build in the traditional blockchain networks as all data in state is publicly visible.

### Secret Auctions and Secret Voting
These related use cases involve replacing the inefficient, two-step “commit-reveal” schemes with a better approach, which relies on secret contract functionality. Both secret auctions and secret voting would allow the users to submit their encrypted bids/votes and the secret contract can compute on encrypted inputs to determine the winner(s), without requiring the users to reveal bids or votes. 

### Decentralized Finance
Imagine an open, global economy with more accessible financial services, e.g. savings, lending, trading, insurance, and more! On Secret Network, DeFi customers maintain privacy while interacting with a permissionless economic system that creates new opportunities for wealth.
