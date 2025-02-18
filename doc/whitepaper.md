# Kismet Whitepaper

David Vennik <david@cybriq.systems>

June 2022

**Abstract.** Leadership and consensus are two distinct concepts in distributed systems. Proof of Work picks a leader, same as Proof of Stake, but in the Bitcoin design, it dictates the timing of blocks, and the emission of tokens all in one. While this has advantages of simplicity it makes the distributed system it creates somewhat inadequate for transaction processing. Proof of Stake is nothing more than distributed systems replication of plutocracy. Kismet brings the idea of Proof of Work for leadership while using a proven, fast Classical Consensus for the actual block scheduling and timing of transaction processing.



## Introduction

Currently in the field of public blockchain based financial ledgers there is the Proof of Work chains with random timing and probabalistic finality, and on the other hand, the Proof of Stake classical consensus chains with rapid or instant finality. There is a wide gulf between these two systems as regards to satisfying the requirements for a financial ledger for processing payments. 

"Proof of Work" chains have the problem that you can't be sure about transactions staying final until several hours later, but protect against monopolisation, which has happened many times to "Proof of Stake" blockchains.

Underpinning both models is the idea of distributing risk amongst a group of entities who get short term leadership of the system. This is a little similar to the idea of term limits in Democracy.

Proof of Stake chains sacrifice the breadth of this hedge against corruption for fast processing. Proof of Work sacrifices regular processing times for a broader hedge against corruption.

1. ## Proof of Work for Leadership with Classical Consensus

What Kismet proposes is creating a chain purely for recording the winners of a Proof of Work lottery for various leadership roles, and accumulating these ahead of time to produce a future queue of validators for a classical consensus based on Tendermint's variant of the Practical Byzantine Fault Tolerance protocol.

Winning a validator slot enables the winner to join the pBFT chain validator queue, by applying to the current validator set for membership, who then agree to place the winner's right to membership into schedule for new blocks.

Standard pBFT chains use a new block generated seeding for random selection, combined with a weighting algorithm to reward bigger stakes with more leadership rewards.

The pBFT chains that use Proof of Stake to select leadership for rounds of the consensus have a problem that through mischief an outsized quantity of tokens can be acquired, and so they have to add further complexity with a rule called "slashing" that entails peers being able to unlock and divert stake to a governance treasury or burning the stake in order to disincentivise such mischief.

Proof of Work doesn't have this weakness because acquiring mining power cannot be cheated. Thus there is no need for this complication.

The problem gets even more acute in the context of Decentralised Finance, where one need not merely rob someone to gain a leadership position, but to defraud a credit market, or in other words, rob many someones. 

Leadership in distributed systems quite simply becomes more and more vulnerable to gaming the less randomly it is given out.

2.   ## Long Term Veto Power Balanced by Forking Power

The second big vulnerability of blockchain financial ledgers is another rather popular feature in many new projects, commonly called "governance". This power is likewise distributed to those with the biggest stakes, and enables arbitrary changes in the protocol to be "mandated". 

Kismet has a mineable token for creating proposals, as well as mining for voting slots to vote on proposals once these proposals have been spent. However, such proposals can involve decisions that can corrupt the security of the protocol.

The first rule of democracy is that if you change the voting rules you can manipulate the appearance of legitimacy.

In order to defend against this, there is a role granted to one individual, who can delegate this task of sentinel for governance, and the only power this role has is to stop governance proposals from being passed.

It is a founding statement of the Kismet project that there is two legitimate uses for this veto, one is changing the token emission rate, and the second is changing the rule about the existence of this permanent, succession based role holding the veto power. It would not be legitimate to somewhat expand the number of individuals with such veto power but dividing their power would be illegitimate.

The most invested miners can then enforce this refusal by forking the chain by manually designating a particular proposal being vetoed by an illegitimate holder of the veto power as being invalid, and causing the Proof of Work chain to fork this disputed veto off the chain.

By these two mechanisms combined, it should be possible to permanently ensure that no decision made for the governance of Kismet can change these vitally important foundational rules, nor permit the abuse of this veto power by the majority of miners whose real world, non cheatable investments in mining capacity collectively function in the same way as the veto power itself. 

The Veto holder is the political leader, and the Miners are the business leaders. They can nullify each other's attempts to nullify, and force a similar thing to the dissolution of a parliament, annulling a proposal, or annulling the nullification of a proposal, allowing it to be voted on. The Veto Holder will be forced to pass on his power to a successor if the majority of miners keep forking his vetos off the chain, or he/she can use it wisely.

Thus, the Veto key provides for two features, creating a child key, which can be revoked, and creating a successor key, which cancels the parent key.

It simply is not in the interests of the miners to change this structure of leadership. The stubborn conservatism of the bitcoin mining community has proven to be very effective in stopping the breaking of the security of bitcoin, and we exploit that strength in Kismet.

3.   ## Sensor Network Causality Consensus

A third feature, optional for financial ledgers, but extremely useful for auditible, collaborative, session based realtime interactive systems, such as game worlds and shared creation environments, is the use of the many to many architecture of classical consensus, combined with probabalistic consensus to rapidly decide a sequence of events within a realtime (100ms) time horizon.

With the relative simplicity of chains that only register leadership allocation to network participants, the idea of creating new ledgers, and stepping outside the box of simple financial ledgers into any kind of collaborative log of events on a network with rapid resolution of sequence, this realtime causality consensus can form part of other ledgers that can be spawned in parallel and operate under any arbitrary consensus that users agree on.

The use of parallel, proof of work chains that only grant leadership means that this protocol can be effectively unbounded in its interconnection and potential userbase as well as enabling fixed and fluid parallelisation of data processing for application specific purposes. The session based realtime protocol is just the first proposed subchain. 

In addition to this, it is probable that the consensus can be used in combination with the realtime competition for leadership role tokens, combined with proximity and latency limitation to distribute risk of monopoly of these fast protocols as well.

Such extended protocols need not necessarily be focused on realtime speeds either, but focus instead on the geographic proximity or affinity of users and the temporary nature of the data, which may not need to be stored in mass duplicate for the purposes of the application.

Limiting membership via a hybrid of proof of work and staking can then enable humans to vet membership in a protocol and provide locality limited governance systems.

This element is a little more nebulous and speculative than the first two, but the primary two elements form a foundation that enables such creative collaboration.

## Conclusion

Like all good games, the best rules are the most concise. As such, this is the entire Whitepaper. 

The goal for the first implementation is section 1 and 2. The third section is for future elaboration and intended to be tied back to the first two as their regulatory foundations.

The control of network systems is the ultimate power in human society. The goal of Kismet is to distribute that risk to the most responsible and careful individuals possible. While it looks like just another distributed systems protocol, it is actually the foundation of a system of government as well. 