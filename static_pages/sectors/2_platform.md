---
layout: page
title: Platform
---

What do I mean by *platform*? Let's compare Ethereum and Bitcoin.
* In Bitcoin, an account stores coins, and a transaction describes the
  transfer of coins between accounts. Transactions are stored forever, and
  nobody can tamper with the stored data.
* In Ethereum, an account stores coins (as in Bitcoin), but it may also contain
  a chunk of arbitrary computer code, called a *smart contract*. A transaction
  may transfer coins between accounts (again, like Bitcoin), but it may also
  invoke the functionality of a smart contract (ie run the code).
This makes Ethereum more general than Bitcoin; Ethereum is a decentralised
computer. Smart contracts and the coins they manipulate are stored on the
blockchain, so they inherit the benefits of decentralisation: they are tamper
proof, and there is an immutable record of all past transactions.

The ability to run arbitrary code extends the utility of the blockchain well
beyond currency. Consider a standard contract, such as the kind of thing you
sign when you buy a house, take out insurance, and so on. The contract is
typically is a list of clauses that specify precisely what is to happen if
various situations occur. For example, if you fail to pay your mortgage on
time, the contract may say that the bank gets to charge a fee; if your car is
stolen, your insurance contract will specify your entitlement to compensation;
and so on. A list of "if this happens, then do that" ... looks a lot like a
simple computer program - and indeed, many contracts can be written in computer
code. But the *smart* part of a smart contract is that the contract can now be
enforced entirely automatically. Your mortgage contract or car insurance
contract relies on the legal system for enforcement. Thanks to blockchain tech,
smart contracts do not require this. Once the contract is agreed and placed on
the blockchain, it is immutable and will carry out the conditions of the
contract automatically. (There is an issue with outside data and *oracles*
here, but let's not worry about that right now.)

But *smart contract* is a bit of a misnomer. It is an arbitrary chunk of
computer code, so it is more than just a replacement for paper contracts.
It can run anything that a regular computer can run (although in practice, the
programs have to be quite short with present technology.) Thus, a blockchain
platform is a base layer on which a variety of applications can be built. An
example application is token generation: Ethereum has a smart contract that
allows you to create your own token. Most of the tokens in the cryptocurrency
market today are implemented by an Ethereum smart contract. A new class of
applications called *dapps* - decentralised apps - are generalisations of web
or phone apps: they are dynamic web pages (like many regular apps) but which
interact with a blockchain to manipulate tokens.

Platform Coins As An Investment
===============================

Platforms seem like a promising investment, especially for the beginner: if you
can't predict which blockchain applications will become popular, why not invest
in a platform? Then, as long as *something* built on that platform becomes
popular, the value of the platform coin should increase, right?

Perhaps, but we must be careful.
* We must consider the tokenomics of each platform coin individually.
  The incentives to buy and hold these coins vary a lot between them.
  The price of the coin will only increase if demand for it increases, so we
  must be sure that the success of the platform means that its coin
  experiences greater demand.
* Blockchains are usually open-source projects (and you shouldn't invest in
  any that isn't), which means there code can be copied. If, say, Ethereum
  became hugely successful, use of the network would rise, and so price of the
  coin would rise (because the coin is required to use the network), but fees
  would also rise. Why would somebody not copy the code and start an
  "Ethereum 2" - or even Ethereum 3, 4, 5, etc? The new network would have few
  user initially, so small fees. People would therefore use this in preference
  to the original Ethereum, wouldn't they? Couldn't we end up with a great many
  low-level platform networks? Perhaps, but I don't think so.
  1. It is not too difficult to fork a blockchain, but it's a bit harder than a
     non-blockchain open-source project. One needs to re-distribute the new
     coins somehow, and the applications built on top of the chain will need to
     be forked or replaced too.
  2. There is probably a developer network effect. Developers for the original
     chain would likely stay there because their friends are there, or out of
     loyalty.
  3. Most importantly, the security of a network is directly related to its
     value. If someone is able to acquire a majority of the coins, they
     effectively control the network. So if a high-value application is
     running on a blockchain, it cannot move to a low-value platform because it
     would then become profitable for an attacker to buy out the platform and
     take over the application. It seems to me that it will likely be necessary
     for parties with a stake in the success of a platform to hold significant
     coins in that platform that its security is maintained.
  In summary, I think we will see a future with a small number of high-value,
  successful, platforms.

But which platforms are the most promising?

* [Ethereum](./1_eth)
* [Cardano](./2_ada)
