---
layout: page
title: Consensus
---

I'll go into a bit of detail about consensus mechanisms since they are such key
properties of blockchains. You need to understand a few things about this
subject to judge whether a coin may be a good investment or not.

Consensus refers to the process by which all the nodes on a network come to
agreement about the current state of the database. In a centralised database
residing on a single machine, the state can be updated immediately when someone
requests a transaction. But in a distributed database, someone will put in a
request for a transaction to one of the nodes, and that node must broadcast the
new state to all the other nodes so that all nodes maintain the same state.
If all nodes trust each other, this isn't too hard. But in the crypto world,
this isn't the case. The fundamental problem (that Bitcoin was first to solve)
was how to ensure all the nodes come to consensus about the database state
without any node having to trust any other.

Proof of Work (PoW)
-------------------

PoW is a type of consensus protocol. Bitcoin, Ethereum, and various other
cryptos use it. The idea is that all the nodes try to add the next block to the
chain, but to do so, they must solve a mathematical problem. This problem is
set up to be a kind of trial and error: the nodes try many different numbers
until they find one that works. When a node succeeds, it tells the other nodes.
The other nodes check the solution, then include the proposed block at the end
of the chain, then move on to the next block.

For Bitcoin, the maths problem is designed to take the network about 10 minutes
to solve, so Bitcoin gets a new block in its chain every 10 minutes or so.
Since it takes so long, it is unlikely that 2 or more nodes will solve the
problem within the time it takes to broadcast a solution around the network.
If that does happen, the chain forks into multiple pieces; each chain proceeds
as above; then everyone switches to the longest chain once one of the forks
gets ahead.

Some properties of PoW:
* Secure provided that nobody manages to acquire 51% of the coins.
* Proven over many years in Bitcoin, Ethereum, etc.
* Uses a lot of energy: all those computers working at full capacity to solve
  that maths problem use a lot of energy. There's some estimate (probably
  inaccurate) that Bitcoin's network currently consumes energy at a similar
  rate to the whole of Denmark.
* Can be slow. 10 minute block times for Bitcoin, and you need to add a few
  blocks (say 6) for a transaction to be confirmed.
* Hard to scale as number of users increases, eg energy consumption increases.

Proof of Stake (Pos)
--------------------

PoS removes the need for the high energy consumption of PoW. It replaces the
requirement for a node to solve a maths problem with the requirement for a node
to stake money. Nodes propose blocks to be added to the chain and one is chosen
at random. If a node is seen to be attempting malicious behaviour, it risks
losing its stake.

PoS is still at the research stage.
* Ethereum is working on a version, called Caspar, which seems to be a couple
  of years away from deployment.
* Cardano has a peer-reviewed version with some proven desirable properties
  which is scheduled for deployment early 2019.

Delegated Proof of Stake (dPos)
-------------------------------

A PoS consensus algorithm is hard to develop without sacrificing any of the
desirable properties of blockchains. dPoS is a compromise that sacrifices
decentralisation for good scaling properties (ie supporting many users while
maintaining speed and not getting congested). The basic idea is that a small
number of nodes (eg 20 in the case of EOS) are the only ones that maintain the
database and have to arrive at a consensus. The other nodes typically get to
vote the 20 in or out - so the network is kept secure because misbehaving nodes
can be voted out.

That's the idea. In practice, I'm highly suspicious of these coins. People will
always collude and try to cheat when money is involved, and these dPoS networks
are too easy for rich and/or coordinated groups to control. Which is not to say
they won't be successful... perhaps society will decide that this trade-off is
acceptable, and we'll give the power to a small group of people for the benefit
of a fast network. I don't like it, though: putting too much power into the
hands of a few often ends badly.

Proof of Authority (PoA)
------------------------

I don't know much about how PoA works. I do know that it is intended for
private blockchains where all the nodes are trusted, such as within a single
company. In that scenario it works well, but shouldn't be used for a public
blockchain where nodes may be adversarial.
