    © Copyright 2018, Simon Castano

    This file is part of Brane.
	
    Brane is free software: you can redistribute it and/or modify
    it under the terms of the GNU General Public License as published by
    the Free Software Foundation, either version 3 of the License, or
    any later version.

    Brane is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU General Public License for more details.

    You should have received a copy of the GNU General Public License
    along with this program. If not, see <https://www.gnu.org/licenses/>.
 

# The Case for a Crypto-Portfolio Management Tool #

## Abstract ##

This document explores problems faced by crypto-investors for managing their investment.  
It argues in favor of a portfolio management tool, Brane, describes its required functionalities and set a road map for future extensions. 

## Table of Contents ##

1. [Introduction](#introduction)
2. [Problem Statement](#problem-statement)
    1. [Investing in the crypto market](#investing-in-the-crypto-market)
	    1. [Asset Selection](#asset-selection)
	    2. [Optimize and Trade](#optimize-and-trade)
	    3. [Distribute Third Party Risk](#distribute-third-party-risk)
	2. [A Growing Complexity](#a-growing-complexity)
    3. [Trading Ease of Use for Risk](#trading-ease-of-use-for-risk)
3. [Solution](#solution)
    1. [Single Point of Entry](#single-point-of-entry)
	    1. [Unified Trading Language](#unified-trading-language)
		2. [External Data Service](#external-data-service)
	    3. [Local Data Service](#local-data-service)
	2. [Financial Statements Module](#financial-statements-module)
	3. [Analyses Modules](#analyses-module)
	    1. [Market Analyses](#market-analyses)
	    2. [Portfolio Analyses](#portfolio-analyses)
	4. [Algorithmic Trading](#algorithmic-trading)
4. [Conclusion](#conclusion)
5. [Future](#future)
	1. [Distributed Data](#distributed-data-intelligence)
	    1. [Market Data](#market-data)
		1. [Strategy Data](#strategy-data)
	2. [Distributed Computing](#distributed-computing)
	3. [Dedicated Hardware](#dedicated-hardware)
6. [Additional Resources](#additional-resources)

## 1. Introduction ##

Bitcoin did successfully manage to remove trust in central authority that was so far required for any currency to be valued and used. Its ecosystem has developed over the years with the birth of hundreds different cryptocurrencies and a financial system being a pale copy of the fiat financial system with exchanges and funds all being handled by a third party which users have to blindly trust.  
While exchanges do greatly help to enhance market liquidity and cannot be overlooked by investors, funds or ETF simply shade away market complexity and operations, acting as a simple facade for investors.  
The below describes the complexity of investing in cryptocurrencies and solution that investors could use to easily manage their investments without scarifying ease of use for third party risk.

## 2. Problem Statement ##

### 2.1 Investing in the crypto market ###

The crypto market offers a lot of investment options with more than sixteen hundreds crypto assets<sup>[[1]](#coincount)</sup> and any wannabee investor will have to do his home work before entering the market. In most cases, Bitcoin will be the first, default crypto-currency selected to build a portfolio - Bitcoin is just *the* original crypto-currency, with the most capitalization, etc.  

Regardless of the above, building a proper portfolio will require a quantitative analysis of available options so that assets can be selected and added to a portfolio if appropriate. It is assumed that "investors are risk averse, meaning that given two portfolios that offer the same expected return, investors will prefer the less risky one. Thus, an investor will take on increased risk only if compensated by higher expected returns. Conversely, an investor who wants higher expected returns must accept more risk."<sup>[[2]](#mpt)</sup>  

#### 2.1.1 Asset Selection ####

To begin with, investors have to understand what they are investing in and may start with classifying crypto-assets. Exibiting a wide range of use cases associated with different markets, similar assets will tend to behave similarly in given market conditions and their classification will help investor to diversify.  

For example and according to P. Kravchenko<sup>[[3]](#periodictable)</sup>, classification could be done on five processes which may have at least three states (centralized, decentralized, not possible), and which can be managed by one or separate roles:  

  * Governance  
  * Custody  
  * Issuance and distribution
  * Transaction processing  
  * Audit  

Different combinations of the ways these processes are managed lead to hundred twenty five possible different types of digital assets and markets from which investors can pick to build a portfolio, including but not limited to crypto currencies, digital currencies, commodity-backed tokens, equity tokens, utility tokens, digital collectibles, etc.  

In parallel of classification, assets should be analyzed and rated individually by aggregating some key data such as the below.<sup>[[4]](#weiss)</sup> Classification combined with rating methodology will allow investors to compare assets quantitatively, on a common basis.

  * Risk Index  
  * Reward Index  
  * Technology Index  
  * Adoption Index  

Note that while to first two indexes can be extracted and calculated from market data, the last ones follow a rather manual process and will also be subjective to investor values and believes.  

<a name="coincount">[1]</a> [CoinMarketCap](#https://coinmarketcap.com/).  
<a name="mpt">[2]</a> [Modern portfolio theory - Wikipedia](#https://en.wikipedia.org/wiki/Modern_portfolio_theory#Risk_and_expected_return)  
<a name="periodictable">[3]</a> [The Periodic Table of Blockchain - Pavel Kravchenko](#https://www.coindesk.com/periodic-table-blockchain-classify-tokens/)  
<a name="weiss">[4]</a> [The Weiss Cryptocurrency Ratings Explained - Weiss Ratings, LLC](#https://weisscryptocurrencyratings.com/ratings/the-weiss-cryptocurrency-ratings-explained-15)  

#### 2.1.2 Optimize and Trade ####

Investors are then able to optimize risk and return for their portfolio using rating and classification data collected previously. With their ideal portfolio distribution at hand, investors can enter and/or exit markets to balance their actual portfolio distribution against benchmark and time their trades to get the most reward out of it.  

Overall, investors will follow a repetitive process consisting of:  

  * Asset rating  
  * Portfolio optimization  
  * Trade timing  

#### 2.1.3 Distribute Third Party Risk ####

Last and not least, investors could very well select and use a single exchange and have all their asset stored and traded there, that would be convenient but would also be very bad if that exchange goes Mt Gox<sup>[[1]](#mtgox)</sup>... Thus, investors are better off spreading their risk over multiple parties and wallets and give away some convenience; as the saying goes: don't put all your eggs in the same basket.  

<a name="mtgox">[1]</a> [Mt. Gox - Wikipedia](#https://en.wikipedia.org/wiki/Mt._Gox)  

### 2.2 A Growing Complexity ###

Regardless of how investors build their portfolio, following and managing the later is a manual process involving multiple parameters. Even though services or software are available to ease some parts of the process such as rating, optimization and timing, none do cover the whole repetitive process of rating, optimizing and timing at once.  
Investors are thus required to handle data manually at some point in time of the process. Considering investors should keep track of multiple parameters of multiple crypto asset held at multiple third parties, complexity and reporting is growing exponentially with each new element added to a portfolio, which can quickly become hard to manage manually.

### 2.3 Trading Ease of Use for Risk ###

New crypto ETF<sup>[[1]](#funds)</sup> keep coming to the market with more the hundred and fifty active as off April 2018 and while they do cover the need for a service, shading away the complexity of managing a crypto portfolio, investors do have to trust a single third party going against what cryptocurrencies have made possible: getting rid of the trusted third party.  
Investors clearly need a tool to get rid of this middle man by providing all functionality needed for an investor to manage crypto portfolio through a single, unified software than can run from home.  
It must allow investors to easily manage portfolio made of assets held at various exchanges and wallets, de facto reducing third party risk, but must also provide various service made possible by being at the core of portfolio operations such as financial reporting, market and performance analyses, automated trading, data intelligence. It will ideally connect to decentralized exchanges to trully decentralize investments.  

<a name="funds">[1]</a> 150+ funds according to [Bloomberg](#https://www.bloomberg.com/news/articles/2018-04-02/crypto-hedge-fund-bubble-begins-to-deflate-as-returns-tumble)  

### 3 Solution ###

The first and logical step to get rid of third party risk is to spread assets over multiple parties while managing all operation through a facade that standardize operations. This will consequently reduce investors' risk without giving away ease of use. And this will be the main function of the proposed solution, Brane.  
Being at the core of all portfolio operations Brane will be able to provide a range of added functionalities naturally building on each other.  

For the sake of transparency and audit-ability Brane will be release under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or any later version, allowing anyone to audit, contribute, fork or copy its code.  

It will be designed using the Julia language, mainly for its dynamic nature and high productivity and performance for both financial analytics and infrastructure.<sup>[[1]](#julia)</sup>

<a name="julia">[1]</a> [Julia - A new language for technical computing](#http://www.automatedtrader.net/articles/technology-strategy/157921/julia-_-a-new-language-for-technical-computing)  

### 3.1 Single Point of Entry ###

#### 3.1.1 Unified Trading Language ####

Interactions with services will be standardized to allow investors to use external services without having to worry about the various API specifics. It will just simplify the management of multiple parties by unifying query constructs.

#### 3.1.2 External Data Service ####

Leveraging the unified trading language, Brane will allow investors to connect to multiple parties to retrieve both market and investor's trade data over multiple assets. It will provide both live connection and construct for querying past data from multiple sources.  
The above naturally implies securely storing investor credential for private API calls.  

#### 3.1.3 Local Data Service ####

All data acquired through the external data service will be stored in persistive local databases split in categories: e.g. market data, portfolio data, asset rating, etc.

### 3.2 Financial Statements Module ###

The financial statements module will provide information about the financial position, financial performance, and cash flows of a portfolio, following International Accounting Standards<sup>[[1]](#ias)</sup>. To meet that objective, financial statements will include:  

  * a statement of financial position (balance sheet) at the end of the period  
  * a statement of profit or loss  
  * a statement of cash flows for the period  

In other words, this module will simply query and concatenate local data in a predefined (or user-defined) model.  

<a name="ias">[1]</a> [IAS](#https://www.iasplus.com/en/standards/ias/ias1)  

### 3.3 Analyses Modules ###

#### 3.3.1 Market Analyses ####

The market analyses module will provide investors with markets' technical indicators. Brane will provide a library of indicators and allow investors to create and use their very own indicators.  
To avoid re-computing information, indicators' value will be stored by local data service in a specific category for later access or analyses.

#### 3.3.2 Portfolio Analyses ####

The portfolio analyses module will provide investors with the ability to select, rate and calculate weight of assets that will make up a portfolio, depending on its selected characteristics. It will consist of several sub-modules including:  

  * Portfolio characteristics definition including asset type, horizon, risk tolerance  
  * Assets rating, on the basis of both data feed from the market analyses module and data entered manually by investors  
  * Portfolio optimization following the (post) modern portfolio theory, Black-Litterman model, or any relevant optimization model. 

### 3.4 Algorithmic Trading ###

Algorithmic trading will rely on Brane's analyses modules to provide investors with a wide range of indicators. These indicators will in turn be used to trigger buy or sell orders according to investors' input.  
Brane will allow investors to back test their strategy on historical market data, enable it in a simulation mode a.k.a. paper trade and restrict trading to portfolio portions only.

## 4 Conclusion ##

With the above mentioned modules interacting with each others, i.e. data service, reporting, analyses and algorithmic trading, Brane will offer all managed ETF's advantages to private investors, simply owning an internet connection and a computer. On top of the later, investors will be able to include or exclude any third party or asset they deem non trustable, following their very own analyses or belief.  

## 5 Future ##

Brane is first intended to be used by tech-savvy investors that have basic knowledge in scripting and operating servers. In the longer term though, Brane will develop GUI to facilitate user interactions.  
Other modules will be investigated, aiming at distributing trading data, intelligence and computing, further described here after. These later modules combined with a friendly GUI would allow any investor to use Brane, purchasing strategy, computing and/or data from investor to investor.  

### 5.1 Distributed Data ###

Brane will allow users to reduce or backup local storage by distributing non critical data<sup>[[1]](#critical)</sup> over multiple nodes. It will also create a decentralized data market where investorsin which each and every node is free to participate.

<a name="critical">[1]</a> data not required for calculating indicators 
 
#### 5.1.1 Market Data ####

This will be an automated system in which market data beyond date ranges used to calculate indicators, will be stored in a distributed database.  
Ideally, data distribution would be similar to torrents and before being added publicly, data will have to be signed for correctness by multiple users. While market data will easily be verifiable, indicators will require multiple computation to ensure correctness. On the other hand, this data would need to be calculated and verified only once, allowing later investor to simply retrieve it.  

#### 5.1.2 Strategy Data ####

This module will allow investors to trade their strategies with other investors by comparing respective performances and signaling investors of possible strategy deal.  
Strategy data will have to be signed by investor before publication to a strategy market. Such signature will be taking in account market data from the distributed market data to allow anyone to verify for strategy performance without revealing strategy. A strategy buyer would receive strategy private key against a fee for decryption of the later.  
Strategy market will be an automated system, matching best strategy for investors depending on their risk profiles, preferences and views on crypto market.

### 5.2 Distributed Computing ###

Calculating indicators and optimizing portfolio might end up being resource intensive and we could imagine some investors willing to deep test their strategy using res sources from other nodes to speed up optimization. This will require some sort of proof of work system in which result would be provided to requester only. And instead of being competitive, result would be delivered by a collaborative distributed computation network.  
This could allow investors to develop and test trading strategy using deep learning algorithm while allowing others to rent their spare computing capabilities. Other setup, could give birth to collaborative funds in which investors having same profile and objective would mutualize resources with each others.

### 5.3 Dedicated Hardware ###

A dedicated hardware running Brane along with 100% free software will be developed in the longer term to facilitate deployment. This will allow investor to simply plug it, go through configuration and have their personal crypto fund running within the hour.

### 5.3 A Note About Decentralized Exchange ###

Last and not least, Brane is originally thought to be used with decentralized exchange which will hopefully be develop and slowly replace classic exchange. As soon as this becomes a reality, Brane will make the most sense by allowing investor to remain in total control of their funds, providing a range of functionalities, expendables by means of modules. 

## 6 Additional Resources ##

Please refer to [GitHub project page](#https://github.com/roshii/brane/)
