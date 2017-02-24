# Trade Guild Overview

##### The Safe, minimal trust way for non-professionals to invest in digital currencies.

The Trade Guild ([tradeguild.io](https://tradeguild.io) coming soon) is a secure, distributed digital currency investment fund featuring automated management, self-insurance, and tamper-proof accounting records published on a blockchain.

Users will be able to manage their digital currency investments from an online portfolio, and instruct automated trade bots in investment strategy.

At accounting time, each account will have timestamped, mark to market records of each trade on a [GitGuild](http://gitguild.com) blockchain. This creates a perfect, impossible to fake or modify accounting record.

### Automated Trading

The Trade Guild's main feature set is automated trading of digital currency tokens. A number of exchanges, tokens and strategies are supported to fit our diverse user base. Strategies we will launch with are as follows.

| Name | Risk profile* | Description |
|------|------|-------------|
| Cost averaging | Simple | Accumulate or close a position gradually by making regular trades. |
| Market making | Moderate | Place bid and ask limit orders both priced aggressively. The goal is for both to fill, netting the difference between them. 
| Business Hedging | Moderate | Hedge your business activities by telling the bot what market exposure your business has created. I.e. you received 1 BTC in payment, so the bot will sell 1 BTC. |
| Arbitrage | Moderate | Buy an asset low on one orderbook while selling it high on another. Ideally this happens at the same time. |
| Multi-step Arbitrage | High | Like arbitrage, but involving 3 or more orderbooks instead of 2. |
| Trend follower | High | Using pseudo-[Bayesian inference](https://en.wikipedia.org/wiki/Bayesian_inference), assume breakout trends will continue, and trade along the trend. I.e. buy when the price is rising, sell when it is falling. |
| Configurable Levels | High | Set price levels on a daily basis, which correspond to buying and selling plans. |

\* Risk profile does not promise any returns, and is not financial advice. It is an indicator of net exposure for applying that strategy, i.e. size and number of trades open on a given day.

##### Exchanges

The Trade Guild will support trading the following digital currency exchanges.

+ [Bitfinex](https://www.bitfinex.com/?refcode=01xKtJ5kvg) The highest volume USD exchange. Offers up to 3x margin on a number of tokens.
+ [Kraken](https://kraken.com) The highest volume EUR exchange. Offers up to 3x margin on a number of tokens.
+ [Poloniex](https://poloniex.com) The highest volume altcoin exchange. Offers up to 5x margin on a number of tokens.
+ [Bitmex](https://www.bitmex.com/register/I20ONy) mercantile exchange. Offers up to 100x margin on derivatives, i.e. futures or swaps.

##### Tokens

The Trade Guild will support trading the following digital currency tokens.


| Token | Type | Exchange(s) |
|-------|------|-------------|
| Bitcoin | Proof of Work | Bitfinex, Kraken, Poloniex, Bitmex |
| Dash | Proof of Work | Poloniex, Bitmex |
| Litecoin | Proof of Work | Bitfinex, Kraken, Poloniex, Bitmex |
| Ethereum | Proof of Work going to Proof of Stake | Bitfinex, Kraken, Poloniex, Bitmex |
| Ethereum Classic | Proof of Work | Bitfinex, Kraken, Poloniex, Bitmex |
| ZCash | Proof of Work | Bitfinex, Kraken, Poloniex, Bitmex |
| Monero | Proof of Work | Bitfinex, Kraken, Poloniex, Bitmex |
| Augur | Proof of Stake | Bitfinex, Kraken, Poloniex, Bitmex |

### Fees

##### Trading Accounts

All trading accounts have up front and quarterly fees. All plans include server setup, as well as our on-boarding tutorial about creating API keys. In all cases but the Beginner plan, setup also includes a 1 hour consultation with one of our digital currency experts to help the user choose which tokens and strategies to enable.

| Plan         | Setup | Hosting* | Profit Sharing* | Min Cap | Max Cap | Private** |
|--------------|-------|----------|-----------------|---------|---------|-----------|
| Beginner     | $100  | $25      | 2.5%            | $0      | $5,000  | No        |
| Intermediate | $250  | $25      | 1.5%            | $2,500  | $25,000 | No        |
| Private      | $500  | $100     | 1%              | $5,000  | No Max  | Yes       |
| Custom***    | $1,000 | $100    | 1%              | $25,000 | No Max  | Yes       |

\* Hosting and Profit Sharing are charged quarterly. Profit sharing is calculated as total portfolio value on a mark to market basis against the US Dollar.

** The Trade Guild offers two types of plans: public (pseudonymous) and private. For details on privacy for pseudonymous plans, see "Security" section below.

*** Custom plans carry an additional, up front bot development cost described below.

##### Vault

In addition to active trading accounts which carry counter-party risk on third party exchanges, the Trade Guild offers a long term Vault service. Because of the labor intensive processes and expensive cold storage setup, Vault wallets carry more fees than self-hosted wallets. See "Security" section below for details.

| Fee Type    | Amount |Description |
|-------------|--------|------------|
| Profit Sharing | 0.5% | Vault funds are included in the profit sharing fee based on mark to market value at the close of each fiscal quarter. |
| withdrawal  | 0.1%   | To compensate the Vault admins for the manual effort of signing, a 0.05% fee will be set aside for each. |

##### Custom

In addition to standard plans and trade bots, users may request additional consultation and/or development services. These are all performed by our highly skilled digital currency experts.

| Fee Type | Amount | Description |
|-------------|--------|------------|
| Open source bot dev. | $10,000 | Our expert developers will work with you to distil and automate your desired trading algorithm, to be released under an MIT license. |
| Proprietary bot dev. | $25,000 | Our expert developers will work with you to distil and automate your desired trading algorithm, and you keep the intellectual property. |
| Consultation  | $100/h   | Consult with one of our digital currency experts via video conference. |

##### Referral

To compensate our marketing partners, as well as user to user referrals, 10% of any setup and quarterly fees will go to the referrer. This includes setup, hosting, and profit sharing, but not custom development, consultations, or Vault withdrawal fees.

##### Self-Insurance

An internal insurance fund will be set up to cover any loss of funds or disputes. This fund will be denominated in bitcoin, and stored in a published multi-signature address. The insurance fund will receive 10% of any setup and quarterly fees. This includes setup, hosting, and profit sharing, but not custom development, consultations, or Vault withdrawal fees.

### Security

Trade Guild will never have access to user funds, but instead will provide tools to assist the user in self-management of the funds.

##### Automatically Traded Funds

Funds managed by the automated trade bots will be on deposit with third party exchanges under the customer's name and control. The customer only needs to set up a no-withdrawal API key for the bots to work, and is responsible for all movement of funds between exchanges, as well as for any counter-party risk with said exchanges.

##### Vault

The Trade Guild will offer a multi-signature vault service for long term fund storage. Neither the user, nor the Trade Guild will be able to move funds without the other, ensuring security of the funds, as well as enforcement of terms. This will be done through a 3 of 4 signature scheme.

| Key Number | Access Type | Holder |
|------------|-------------|--------|  
| 1          | Password based key derivation (PBKDF) | User |
| 2          | Cold storage (paper backup) | User |
| 3          | Cold storage | Trade Guild admin 1 |
| 4          | Cold storage | Trade Guild admin 2 |  

Normal withdrawals will require the user to sign with key #1, which can be done from with their username and password. Then two Trade Guild admins will each manually sign the withdrawal during their daily signing session at 10 PM (22:00) UTC. This laborious process ensures numerous manual and offline checks, protecting funds from traditional hacking methods.
  
To steal funds from the Vault, and attacker would need to compromise both of the user's keys, and one of the administrator's cold storage wallets. Similarly, if something unforeseen happens to one of the admins, users can still access their funds, until the admin recovery/replacement plan can be implemented using cold storage key backups.  

##### Privacy

For all "public" plans, all trades are published under a pseudonym. This is both easier and cheaper to host, as well as proof of performance. The pseudonyms will be SHA256 hashes of usernames. This ensures that no one in the public will be able to derive the username from the pseudonym (SHA256 hashes are one directional), while allowing users to audit their trading activity from the public blockchain.  

### Technical Details

The Trade Guild will operating automated trading services using it's open source [Trade Manager](https://github.com/TradeGuild/trade-manager) software. This fifth generation trade bot has a proven track record of years and tens of millions of dollars worth of trades. It works with all of the major exchanges, and features pluggable strategies.

All accounting records will be published to git repositories, and signed with a [PGP](https://en.wikipedia.org/wiki/Pretty_Good_Privacy) key. This process creates a tamper-proof blockchain, managed by the [GitGuild](https://github.com/gitguild/gitguild) software.  

The Trade Guild website will be a low-access portfolio management system. Users will be able to view their balances, invoices, and accounting records. Once the Vault is ready, it will be integrated into the website, providing basic wallet functionality.  

### Launch Plan

__March 15 2017 - Soft Launch__

Since the Trade Manager and GitGuild software are ready for use, launch can happen very quickly. Some customization will need to be done to each to accommodate the Trade Guild model, but this will take less than a week. Factor an additional week to create the website and prepare wallets and other accounts.

__April 1 2017 - Public Launch__

After two weeks of testing and feedback-driven improvements, we will do a full public launch. This will include a press release and marketing campaign in partnership with [Crypto Hustle](https://cryptohustle.com) and [200 Social](http://200social.com)  

__TBD - Vault Launch__

At a to be determined date, the Vault will be added to tradeguild.io. This is significantly different from the other services to be provided by the Trade Guild, and will require significant time investment.
