<p align="center">
  <a href="https://www.youtube.com/watch?v=N5b4_5hvOog"><img
    src="https://raw.githubusercontent.com/corollari/awesome-neo-docs/master/fast_learning.png"
    height="150px"
   ></a>
</p>

<h1 align="center">Awesome NEO Docs</h1>

<p align="center">
  A curated and categorised list of awesome documentation for <b><a href="https://neo.org/">NEO</a></b>.
</p>

## How to use this list
Read first the docs marked with **[Basic]**, then the **[Intermediate]** ones and finally the **[Advanced]** ones.

## [Basic] I've developed a dApp in Ethereum before, how do I develop one for NEO?
Equivalences:
- MetaMask = NEOLine, Teemo or O3
  - NEOLine: [Chrome extension](https://chrome.google.com/webstore/detail/neoline/cphhlgmgameodnhkjdmkpanlelnlohao) | [Docs](https://neoline.cn/dapi/)
  - Teemo: [Chrome extension](https://chrome.google.com/webstore/detail/teemo-wallet/faddjfhplkcfackpcjnmmeapchnkobjk) | [Docs](https://dapi.nel.group/en/)
  - O3: [Desktop wallet](https://o3.network) | [Docs](https://docs.o3.network/docs/dapiIntro/)
- Web3 = [neon-js](https://github.com/CityOfZion/neon-js) | [Docs](https://cityofzion.io/neon-js/) | [JSFiddle Examples](https://github.com/CityOfZion/neon-js/blob/master/examples/browser/README.md)
- Mist = [nOS](https://nos.io)
- Geth = [neo-cli](https://github.com/neo-project/neo-cli) or [neo-python](https://github.com/CityOfZion/neo-python)
- Ganache = [neo-local](https://github.com/CityOfZion/neo-local)
- ENS = [NNS](https://neons.name/index_En.html)
- Solidity = [C#](https://github.com/neo-project/neo-compiler) or [Python](https://github.com/cityOfZion/neo-boa)
  - There are more languages that can be used to code smart contracts, such as Java or Go, but the compilers and the tooling around them are not as mature as the ones available for C# and Python so use at your own risk.
  - Remix IDE = [Neocompiler](https://neocompiler.io/#!/ecolab/compilers)
  - Differences:
    - NEO smart contracts can't send NEO or GAS by themselves, they can only send NEP-5 tokens. NEO smart contracts can receive and store NEO or GAS, but to transfer these a transaction must be crafted and sent by a node in the NEO network.
    - It's not possible to get the NEO or GAS balance of an account (including the smart contract) in an easy way.
    - NEO smart contracts can return data of arbitrary length, so returning dynamic arrays is possible.
- ERC20 = [NEP-5](https://github.com/neo-project/proposals/blob/master/nep-5.mediawiki)
- ERC721 = [NEP-11](https://github.com/neo-project/proposals/pull/41)
- ERC165 = [NEP-10](https://github.com/neo-project/proposals/blob/master/nep-10.mediawiki)
- Ether = GAS (GAS fulfills all the functions of ether, the other token, NEO, is only used for voting the validators)
- EVM = NeoVM

## [Basic] How do smart contracts work?
- [Introduction to smart contracts](https://docs.neo.org/docs/en-us/sc/gettingstarted/introduction.html)

## [Basic] How does consensus formation work in NEO?
1. Read [this medium article](https://medium.com/neo-smart-economy/neos-dbft-2-0-single-block-finality-with-improved-availability-6a4aca7bd1c4)
2. Read [this explanation of how validator voting works](https://docs.neo.org/developerguide/en/articles/consensus/vote_validator.html)
3. Extra:
  * [To understand the old version of dBFT better](https://docs.neo.org/developerguide/en/articles/consensus/consensus_algorithm.html)
  * At the end of the day NGD owns a huge amount of NEO so they are the once deciding who will be the validators. [Understand how NGD picks the validators](https://neo-ngd.github.io/reference/How-To-Become-NEO-Consensus-Node.html)
  * To understand the new version of dBFT better, skim through [this paper](https://raw.githubusercontent.com/NeoResearch/yellowpaper/master/releases/08_dBFT.pdf) (you don't have to read it all as it's quite verbose)
  * To understand the attack that lead to the creation of dBFT 2.0, read [this issue comment](https://github.com/neo-project/neo/pull/320#issuecomment-422308894)

## [Basic] NEO 3.0
- [Roadmap and new features in 3.0](https://medium.com/neo-smart-economy/roadmap-of-neo-3-0-development-e2ae64edf226)

## [Advanced] How does NeoVM work?
- MUST read: [NeoVM tutorial](https://neoresearch.io/nvm-learn/)
- NeoVM overview and future upgrades in [article form](https://medium.com/neo-smart-economy/a-deep-dive-into-neovm-neocontract-e470c2c3afb0) and [video form](https://www.youtube.com/watch?v=fLppte-guYE)
- [Explanation of stack isolation and why it is needed](https://medium.com/neo-smart-economy/upgrade-of-neovm-36ee232835d9)
- [NeoVM architecture explanation and Opcode reference](https://docs.neo.org/developerguide/en/articles/neo_vm.html)
- [Syscall reference](https://docs.neo.org/developerguide/en/articles/smart_contract.html)

## [Advanced] How does the P2P protocol work?
- [Overview, examples and quick reference](https://docs.neo.org/developerguide/en/articles/network_protocol.html)
- [Detailed reference](https://docs.neo.org/docs/en-us/tooldev/network-protocol.html)
- [Explanation and reference of messages used for consensus formation](https://docs.neo.org/developerguide/en/articles/consensus/consensus_protocol.html)

## [Extra] Meta information
- [Explanation of the requisites needed to become a core developer](https://neo-ngd.github.io/reference/Becoming_Core_Dev/How-to-Become-A-NEO-Core-Developer.html)
- [NEO Enhancement Proposals (NEPs)](https://github.com/neo-project/proposals). Not really useful, I'd recommend only reading NEP-5. I'd delay reading the other NEPs till you find a reference to them and want to know more about a specific one.

## [Extra] Research
- NeoFS - Distributed file system (like IPFS) that uses zero knowledge proofs
- NeoQS - An adaptation of the NEO protocol that uses quantum resistant algorithms
- dBFT 2.0 - An adaptation of pBFT for smart contract blockchains

## Documentation list
> Comprehensive list of all the documentation sources that are worthwhile
- [Docs](https://docs.neo.org/docs/en-us/index.html)
- [Developer guide](https://docs.neo.org/developerguide/en/articles/introduction.html)
- [Community articles](https://docs.neo.org/articles/en-us/index.html)
- [NEO Tutorial](https://github.com/neo-ngd/NEO-Tutorial)
- [NGD reference](https://neo-ngd.github.io/reference/)
- [API reference](https://docs.neo.org/developerguide/en/api/index.html)
- [Yellowpaper](https://github.com/NeoResearch/yellowpaper) / [Specification](https://github.com/neo-project/specification) (they are the same)
- [NEPs (RFCs for NEO)](https://github.com/neo-project/proposals)
