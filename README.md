# ether-stock-market
## Abstract

This project aims to build a proof of concept of distributing and holding
stock exchange values across different owners through the help of Ethereum smart contracts.

## Concept

To simplify explanations and discussions, we will only speak about company shares that are
bought and sold through a stock exchange classic principle but the concept aims to enlarge
to any buyable product.

A central organisation (**_Cent_**) buys shares of **_XYZ_** on a stock exchange and wants to be
able to distribute the ownership of these units to others. It can be a full share but also a part
of it (fractional-share).

People can then buy those fractional-shares in a decentralized way.

We want here to demonstrate that this is feasible using Ethereum decentralized virtual machine.

## What is available to us?

* Smart contracts
* Token creation, distribution and exchange
* Proof of ownership provided by the underlying blockchain of Ethereum
* Wallets to old tokens

## Limitations & Problems to take into account

Ethereum is based on Ether which as a market cap of around 20B$ (3/6/2017).
Usage of the peer network and the "computer" requires that each transaction is backed up by a fee
that will transfer Ethers from one account to multiple miners to thank them for having settled and
verified the transaction. At the moment Ethereum works on the base of a PoW (Proof of Work) but
this might change in the near future to a Proof of Stake. See a comparison
[here](https://blockgeeks.com/guides/proof-of-work-vs-proof-of-stake/)

Meaning that each transaction happening on the networks induces a fee that someone needs to pay
for.

Stock markets are subject to volatility either is the Ethereum network. This problem needs to be
addressed in order for the Buyer or the Seller to pay the right price for fractional-share trading.

Holding fractional shares represents a risk because it might create illiquidity. Indeed,
when trading on the stock market there might already be some liquidity issues because there
is not enough orders in the order book to enable a trader to successfully execute an order.
This problem might get even greater with fractional shares and an early market creation.
The critical mass needs to be met on this secondary market to enable efficient trading of assets.

When trading on regulated market bid-offer spread provides liquidity. This aspect might or not
need to be taken into account. Even though, at large scale, creation of fractional-shares
might be a solution to avoid bid-offer spread and provide higher liquidity.

The fact of creating a secondary market-place might create an additional volatility on the available
securities.

## Legal Concerns & Disclaimer

Legal side needs certainly to be inspected carefully. From a basic understanding, if this system is
used in a way that it creates a separate value it might fall under strict regulation, if it's used
to create trust and a decentralised ownership it might be easier. Therefore value might need to be
tight to the value on the stock market, demand created, needs to be followed by Cent.

Therefore, I do not recommend, neither do I take responsibility for the use of this project. Make your
researches and make sure you can do it.

## Insuring ownership

As seen, the goal is to create (via Ethereum) fractional-shares of stock quoted shares of a company.
The idea is that **_Cent_** serves as a deal-maker for the secondary market. Therefore, we need to
be sure that **_Cent_** will respect the secondary market by binding shares ownership to the
blockchain and that it cannot be undone unless units want to be sold.

### First idea

In order to respect that engagement, the idea would be to create a legal regular contract that
would be stored in the blockchain that everyone can access in case there would be an issue.
Those shares would need to be non lent neither borrowed and hence be hold on a bullet-proof
custody account. In order to create trust, it might be worth that a non profit organization
ruled by Blockchain voting is in place. This non-profit would have responsibility to create
legal binding contracts and take all reasonable steps in order to insure that **_Cent_** is 
respecting the contracts they signed off. An insurance contract on default might be worth to be
put in place. This insurance contract would create pressure on **_Cent_** to not make default
as they would have necessary power to recover any damage as a straight profit in turn of
paying the asset price and mandating another **_Cent_** to re-bind on the existing contract.

In order to create a **_Cent_**. A company must apply to the non profit by signing off necessary
standard contracts. Once done, the company would be submitted to a vote by the non-profit for approval.

The way this binding system is made should also enable individuals to value their rights if they
feel the non-profit is failing on them.

#### Problems

**_Cent_**'s are hard to create and imply a market-barrier. Chained default is possible but
is still hard to create. The non-profit needs to police the **_Cent_**'s which would involve
money lost because the non-profit would need money to work and this money would need to come from
market players.

### Second idea

An alternative way would be that anyone could be a **_Cent_** but that each **_Cent_** puts a
collateral as a warranty to the ownership, incentivising **_Cent_**'s to not fail on their engagements.
This collateral would need to be higher than the value of the asset otherwise, when the value
of the asset rises, there would be no incentive anymore of keeping the asset. A threshold should be
in place that would auto-engage higher collateral when asset value increases. If **_Cent_** cannot
put a higher collateral, a third market would have to be put in place to exchange those contracts
when someone is about default it.

To incentivize **_Cent_**'s to be created, they would need to receive a premium and make money
by just doing this job otherwise there is no point of becoming a **_Cent_**.

#### Problems

Once a **_Cent_** has made more money than what the underlying asset costs it could default it just
by reducing the profit made without anyone noticing it and create a bad chain reaction at
some point.
 
**_Cent_**'s could also pretend they own the asset and just engage a collateral without ever
having the underlying asset which would mean that blockchain owners do not own the asset but
just a right on the collateral thus offer and demand on this secondary market would not have
any impact on asset price and flaw the whole purpose of the project.

## Handling corporate actions

Corporate actions need to be reflected on the secondary market as well.
* Cash dividends
* Stock dividends
* Splits
* Symbol change

These events being public, it is rather easy to reflect them on owners but some problems might
rise as well.

Indeed, stock dividends and splits might produce more/less shares associated with cash. The reason
for that is that company usually prefer avoiding ending up with fractional shares. Hence,
users might surprisingly receive cash as well even though it was not a dividend. How to prove
the right of the user on getting a part of this cash as the only one ending up with the information
is **_Cent_**?

Corporate actions do happen always when the markets are closed, therefore the price of the asset
is *not* moving at that point, even though it has moved, there is always a fixed price when the
corporate action happens. Therefore this price can be known and flaws can be excluded.

A solution needs to be found to force the contracts to respect that. Meaning a source needs to
give the information and the source data needs to be bulletproof otherwise the contract will
not be correct and actions would be taken without right because of the nature of the program
not being able to revert when an error happened. Errors can not happen. Hence, it would be
the responsibility of the non-profit to grant corporate actions data introduction into the contracts.
Again this could be done through a vote and event automated per contract by using multiple sources
and maybe even some humans when sources aren't agreeing on something. It would be fair to take
also into account the opinion of **_Cent_** but the casting vote would need to end up being
in the hands of the non-profit to avoid conflict of interest. Meaning if every party agrees
(Data sources and **_Cent_**) the non-profit does not need to be taken into account.
When unanimity is not met, then the non-profit has to cast vote the data introduction.

So when an event happens (no matter which). Multiple data sources need to try introducing
the event in the blockchain to cause a reaction. **_Cent_** needs to provide the same information.
If consensus is not met, multiple voters of the non-profit would need to give their version of
the story, if 2/3 agrees, **_Cent_** needs to execute as the non-profit casted the vote.

Up to **_Cent_** to go after them if they think there really is something wrong, this can be done
off blockchain without impacting traders.

## Simple approach, requiring trust

**_Cent_** is a company that just wants to delegate ownership and to enable people to own
fractional-shares with the help of the blockchain. Having this approach in place, enables
users to need less trust in **_Cent_**, helps reducing the risk of being hacked, loosing track of
ownership and reducing costs faced in IT infrastructure.

By having those safe harbours in place, **_Cent_** can offer a better service and excel at costs.

### How to?

* Placing legal contracts of ownership in the blockchain (public records)
* Use of a custody account to ensure shares are not borrowed or lent
* Group trade users to have better deals
* Respecting market will
* Enable inter user share exchange to remove stock-markets and broker fees

### But really, how to?
#### User perspective
##### Buying

**_A_** wants to buy XYZ shares.

##### Selling

#### Cent perspective

## Workflow example buying 0.1 XYZ
XYZ:BR, is a Buy right on XYZ

![Workflow example buying 0.1 XYZ](/uml/buy.png)