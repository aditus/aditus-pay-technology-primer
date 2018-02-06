# Aditus Technology Primer

This will be a series of posts aimed at addressing how a cryptocurrency payment gateway ecosystem ticks. While traditional digital payments have become much of a habit in day-to-day consumption, the challenges present with leveraging cryptocurrencies and blockchain technologies are unique. We'll take a layman approach and break down complex blockchain concepts to make this as simple to understand as possible.

---

#### Catalogue

The series will be separated based on different perspectives to better highlight individual use cases:
1. Under the hood of a cryptocurrency payment gateway 
2. Adoption & Use cases in the real world for Merchants & Consumers
3. Future: Evolution of blockchain technologies and cryptocurrency markets

---

## Under the hood of a cryptocurrency payment gateway 

### Introduction
At Aditus, we believe that cryptocurrency and blockchain technologies represents a shift in how the financial service industry will be disrupted. Like how the internet creates Amazon that disrupts brick and mortar stores like Walmart, cryptocurrencies and blockchain provides an unqiue opportunity to rethink how the payment industry can operate. Thus we are excited to be in this journey to jointly creating this future.

The current state of cryptocurrency is relatively unregulated and that introduces interesting challenges for both businesses and consumers. Cryptocurrency, while introducing amazing potential, can not currently be easily spent and that defeats the purpose of having it as a currency / store of value. 

Therefore we'll be citing different scenarios to demonstrate real world use cases while highlighting the challenges that it represents for all parties involved.

### Challenges
1. Transaction Speed & Confirmation
2. Price Volatility
3. Transaction Cost
4. Market Liquidity & Convertability Pricing
5. Security
6. Counterparty Risk
7. Operational Transparency, Auditability & Anonymity
8. Blockchain Specific Issues

---

### 1. Transaction Speed & Confirmation
#### _Scenario_

> Sam is looking to purchase coffee at a coffee shop. 
>
> However he did not realised that the blockchain network is currently congested, this will result in slower transaction confirmation and thus take longer before the merchant can receive and process his coffee purchase. 
>
> This creates a hassle during payment for both Sam and the merchant since such circumstances can happen unexpectedly.


#### _Problem_
As with blockchain transactions, payments are only confirmed upon having it "bounded" into a block. Transaction speed is determined through the concept of a fee market *[memory pool] and payments are confirmed based on transaction priority according to how much fees are being paid.

Then there is also the fundamental limitation of how fast a transaction can be completed based on blockchain confirmation. This limit differs based on the underlying blockchain *[ Average block time: Bitcoin - 10 minutes, Litecoin - 2.5 minutes, Ethereum - 15 seconds ]* with varying "double-spending" trade-offs. 

Thus it can seem unrealistic to ever imagine using cryptocurrency as a means of payment.

#### _Solution_
We need to look at this scenario from three angles: high valued, median valued & low valued transactions

**High valued transactions**

> If you are buying an international property with bitcoin, transaction speed will not be a concern since other alternative means of payment would likely take even longer due to banking approvals required for huge transfers.

**Median valued transactions**

> If you are buying a television set with bitcoin, transaction speed is barely a concern as well since delivery of the product does not happen immediately. Thus there is no real urgency requiring immediate confirmation of payment

**Low valued transactions**

> If you are buying coffee with bitcoin, transaction speed matters a lot since it's unlikely you will want to wait for 15 minutes before getting your coffee. This however can be migitated by accepting 0 confirmation transactions as long as the transactions appear on the blockchain's memory pool. 

There might be arguments that 0 confirmation transactions are unsafe for the merchant, however similar issues exist with other mediums of payment as well *[ Cash - Forgery notes; Credit Card - Chargebacks ]*. While this is not an ideal scenario, 2nd layer solutions will be available in the near future that will fix this: Lightning network and Sidechains.

Transaction speed as demonstrated is not that different afterall from other methods of payment. 

---

### 2. Price Volatility
#### _Scenario_

> Sam is looking to purchase coffee at a coffee shop. 
>
> However he realised that the price of his cryptocurrency is fluctuating wildly due to some news regarding cryptocurrency regulations. This presents a dilemma for both Sam and the merchant since it feels uncomfortable paying / receiving for a purchase, only to find out it is worth more / less at the end of the day.


#### _Problem_
Due to the infancy and speculative nature of cryptocurrencies, prices can fluctuate wildly making it hard for merchants to accept cryptocurrencies outright without taking price risk. This also creates a caveat for consumers that may be anticipating a price rise thus limiting adoption of cryptocurrency being used.

#### _Solution_
This problem is not entirely limited to cryptocurrency since business usually operate across international borders which results in dealing with multiple soverign currencies. The outstanding issue is with the relatively extreme volatility in the cryptocurrency market.

Price volatility is inherent and unavoidable as the cryptocurrency market matures. This will eventually be resolved as more cryptocurrency based financial instruments and derivatives comes on to the market; specificially increasing market depth and liquidity.

However by using a cryptocurrency payment gateway, businesses should be able to receive the exact payment amount indicated without having to worry about price volatility. Here's an hypothetical scenario:

> - Merchant is selling his book for $50. 
> - Consumer is looking to purchase the book. 
> - Merchant brings out his cryptocurrency payment gateway that indicates the book would cost 0.001 BTC. 
> - Consumer pays the 0.001 BTC. 
> - Merchant receives his $50 while the payment gateway handles the operational logistics of settling the trade.

As for the cryptocurrency payment gateway, during extreme volatile periods of price movement there will always be the need to price volatility into the margins accordingly. Some price risk will always be present but it always does in any business.

---

### 3. Transaction Cost
#### _Scenario_

> Sam is looking to purchase coffee at a coffee shop. 
>
> However he realised that the blockchain network is congested and he probably have to wait 10-15 minutes for his transaction to be confirmed on the blockchain.
> 
> Since the merchant is only willing to confirm his purchase after his transaction is confirmed, he unwillingly pays a higher transaction fee for his coffee purchase to be confirmed faster.


#### _Problem_
It feels unnatural for consumers to pay transaction fees when doing transactions. Making it worst, is the unreliability of the fees required to get the transactions confirmed as fast as possible.

#### _Solution_
Again we have to re-look at this scenario from three angles: high valued, median valued & low valued transactions.

**High valued transactions**

> If you are buying an international property with bitcoin, transaction cost will be of low concerns since it will definitely be cheaper than any banking fees incurred through any means

**Median valued transactions**

> If you are buying a television set with bitcoin, transaction cost has slight concern since it increases the purchasing price of the goods. However compared to the charges that would be incurred by traditional digital payment gateway of 2-3%, businesses can price goods & services lower for cryptocurrency payment and still result in the same or less range of profit margins.

**Low valued transactions**

> If you are buying coffee with bitcoin, transaction cost matters a lot since it's unlikely anyone will pay $3 for a $5 cup of coffee. While there's no immediately addressable solution, transactions could happen on less congested blockchains for a cheaper fee. In the near future as Lightning network and Sidechains gather momentum, this will be resolved significantly easily.

Alternatively cryptocurrency payment gateway can implement a "debit card" system as follows:

> - Consumer deposits 0.001 BTC to cryptocurrency payment gateway. 
> - Consumer sees a book he wants to buy for $50 which cost 0.001 BTC. 
> - He proceeds to pay with his balance on the payment gateway to the merchant. 
> - The merchant's account is credited with $50 through conversion of the consumer's 0.001 BTC.

This solution may seems centralised but at the end of the day, it is no different from what already exist in traditional digital payment gateway.

---

### 4. Market Liquidity & Convertability Pricing
#### _Scenario_

> Sam is looking to purchase coffee at a coffee shop. 
>
> The merchant is keen to accept cryptocurrency for it but is worried about how to eventually convert it back to cash. 
> With business overheads to cover, he will need to avoid taking too much price risk. 
> While accepting cryptocurrencies may help increase business revenue, it creates hassle for the business if their volume of cryptocurrency payments increases.


#### _Problem_
Every transaction that happens on a cryptocurrency payment gateway is indirectly a conversion of cryptocurrency to sovereign currency on public exchanges. In the general sense, it is difficult for businesses to manage the conversion process due to the lack of economy of scale and leading the price inefficiency during conversion.

Another issue is that cryptocurrency markets are still maturing, different cryptocurrencies have different abilities to absorb huge volume of market sell orders if high valued transactions happen. While not fundamentally a deal-breaker, price convertability is crucial to estimate price on a real-time basis. 

#### _Solution_
By enabling tiers of transaction based on settlement amount, cryptocurrency payment gateway can effective migitate the issue of insufficient market liquidity. Examples of such proposal:

> **Bitcoin** <br />
> 24 hour exchange volume: $10 Billion <br />
> Allowed single transaction amount: $5 Million <br />
> Exchange volume to transaction amount ratio: 0.0005%

---

### 5. Security
#### _Scenario_

> Sam is looking to purchase coffee at a coffee shop. 
>
> The merchant is glad to accept cryptocurrency for his purchase. However as more cryptocurrency payments are made, it becomes a hassle keeping track and securing the cryptocurrencies he accepted. 
>
> Reading about major hacks that happens infrequently, he is now worried if his cryptocurrency stash is sufficiently secured.

#### _Problem_
While most businesses are accustomed to the security concepts of traditional payment gateway, understanding how cryptocurrencies are secured seems unapproachable especially to non-technical savvy users. This is especially concerning since major hacks happen almost yearly to varying extent without any recourse to reclaiming stolen funds.

#### _Solution_
The operational logistics of accepting cryptocurrencies is ideally dependant on a setup of Hot & Cold Wallet system. This allows flexibility of operational automation while limiting security risk present due to software coding errors.

The proposed setup:
> **Hot Wallet** <br />
> **Intent:** Used to operationally transfer funds for various means <br />
> **Access:** Programmatically using software code

> **Cold Wallet** <br />
> **Intent:** Used to store funds securely <br />
> **Access:** Multisignature address leveraging hardware wallet

Cryptocurrency payments are decentralised in nature and there is no need for proprietary code to begin accepting it. Thus payments should reference directly to the blockchain to limit potential security errors. Software code interfacing wallets should be used only to manage operational flow instead of managing funds.

---

### 6. Counterparty Risk
#### _Scenario_

> Sam is looking to purchase coffee at a coffee shop. 
>
> The merchant is glad to accept cryptocurrency for his purchase. However to avoid the hassle of handling cryptocurrency and blockchain related matters, the merchant engages a cryptocurrency payment gateway to abstract away this complexity. 
>
> He wonders if it is safe to trust someone else since cryptocurrencies is all about decentralisation and trusting someone else seems to be counterproductive

#### _Problem_
While cryptocurrencies and blockchain technology supposingly provides a decentralised means of peer-to-peer transfer, to integrate into business operations is not always so straightforward and thus resulting in some form of reliance on third payment: cryptocurrency payment gateway.

Even cryptocurrency payment gateway will eventually rely on exchanges and other counterparties to provide access to markets. This presents counterparty risks cascading from one party to the other.

#### _Solution_
In every business, counterparty risk is unavoidable since it is the act of interaction that allows business transactions to happen.

That being said, we try to keep true to the vision of what blockchain technology aims to achieve by decentralising as much as possible to reduce risk. Which is why we will be working closely with our partners, Kyber Network & Digix, to fulfill this vision by leverging their proprietary technology.

> **Kyber Network:** 
> Using Kyber Network's decentralised exchange network, we will be able to safely provide conversion services through cryptographically secured methods without being exposed to counterparty risk.

> **Digix:**
> Using Digix's DGX tokens that represent physical gold bullions allows us to hedge price movements to the relatively stable gold prices.

With this combined partnership, it allows us to provide additional assurance to businesses.

---

### 7. Operational Transparency, Auditability & Anonymity
#### _Scenario_

> Sam is looking to purchase coffee at a coffee shop. 
>
> The merchant is glad to accept cryptocurrency for his purchase. However the merchant is worried having his business financials being available publicly. Ideally, he also wants to take advantage of the technology that blockchain provides but it all seems too complicated to handle.

#### _Problem_
With cryptocurrency payments, one area of concern is always privacy. 

Businesses do not want their transactions records to be known to competitors and yet wish to enjoy the benefits blockchain technology brings with operational efficiency and transparency. Auditability & anonymity sounds like different side of the same coin and it seem paradoxically to claim that this is achievable.

#### _Solution_

**Anonymity Concerns**
Hierarchical Deterministic (HD) wallets enables the ability to differentiate transactions to provide auditability while keeping anonymity for all parties involved. HD wallets are essentially accounts that creates a new address after every use. 

**Auditability Concerns**
By leveraging blockchain system, it enables the ability to do record keeping *[ Taxes, Audits, Operational purposes ]* since all transactions are immutable and publicly available. 


---

### 8. Blockchain Specific Issues
#### _Scenario_

> Sam is looking to purchase coffee at a coffee shop. 
>
> The merchant is glad to accept cryptocurrency for his purchase. However there are various blockchain events that happens on different blockchains every once in a while.
>
> The merchant have no time to research into how to deal with each specific event that happen. He wishes it was simpler so he can just focus on his business while accepting cryptocurrencies.

#### _Problem_
While not immediate familiar to most, there lies minute nuances across different blockchain system that impact various aspects of how operations are handled.

> **Bitcoin & Litecoin** <br />
> BTC & LTC works on the concept of UXTO (unspent transactions output) which calculates transaction fee based on the size of transactions. Thus one can think of the equivalence between accepting a thousand dollar note vs 1 thousand pennies, it results in certain inefficiencies that ends up with higher fees 

> **Ethereum ERC-20 Tokens** <br />
> Ethereum tokens requires Ether as gas to broadcast transactions on the blockchain. Therefore under certain price conditions, it might cost more Ether to send out your tokens than what is worthed.

> **Forks** <br />
> Blockchains are based on a system of consensus. There may be circumstances that result in soft or hard forks occasionally. Such events are result in chain splits and periodical down time for the cryptocurrency's network.

#### _Solution_
There is no one-size fits all solution to the above problem and this is why a cryptocurrency payment gateway is eventually essential to widespread adoption. The evolution to various blockchain technologies will only accelerate as the market matures and as a merchant it will require too much effort to keep up.

---

The above mentioned issues is exactly why Aditus Pay is unique in providing cryptocurrencies payment as a service that abstracts away the complexities involved with accepting cryptocurrency. 

Contact Aditus today to explore how we can better facilitate your businesses into accepting cryptocurrencies.
