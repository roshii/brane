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

This document explores problems faced by crypto-investors. It argues in favor of a portfolio management tool, Brane, and describes required functionalities for such tool. 

## Table of Contents ##

1. [Introduction](#introduction)
2. [Problem Statement](#problem-statement)
    1. [Investing in the crypto market](#investing-in-the-crypto-market)
	    1. [Asset Selection](#asset-selection)
	    2. [Rate, Optimize and Trade](#rate-optimize-and-trade)
	    3. [Distribute Third Party Risk](#distribute-third-party-risk)
	2. [A Growing Complexity](#a-growing-complexity)
    3. [Trading Ease of Use for Risk](#trading-ease-of-use-for-risk)
3. [Solution](#solution)
    1. [Single Point of Entry](#single-point-of-entry)
	    1. [External Data Service](#external-data-service)
	    2. [Local Data Service](#local-data-service)
	2. [Financial Statements Module](#financial-statements-module)
	3. [Analyses Modules](#analyses-module)
	    1. [Market Analyses](#market-analyses)
	    2. [Portfolio Analyses](#portfolio-analyses)
	4. [Algorithmic Trading](#algorithmic-trading)
	5. [Distributed Data Intelligence](#distributed-data-intelligence)
	6. [Dedicated Hardware](#dedicated-hardware)
4. [Conclusion](#conclusion)
5. [Additional Resources](#additional-resources)

## 1. Introduction ##

Bitcoin did successfully manage to remove trust in central authority that was so far required for any currency to be valued and used. Its ecosystem has developed over the years with the birth of hundreds different cryptocurrencies and a financial system being a pale copy of the fiat financial system with exchanges and funds all being handled by a third party which users have to blindly trust.  
While exchanges do greatly help to enhance market liquidity and cannot be overlooked by investors, funds or ETF do shade away market complexity and operations, acting as a simple facade for investors.  
The below describes the complexity of investing in cryptocurrencies and solution that investors could use to easily manage their investment without scarifying ease of use for third party risk.

## 2. Problem Statement ##

### 2.1 Investing in the crypto market ###

#### 2.1.1 Asset Selection ####

The crypto market offers a lot of investment options with more than sixteen hundreds crypto assets<sup>[[1]](#coincount)</sup> and any wannabee investor will have to do his home work before entering the market. In most cases, Bitcoin will be the first, default crypto-currency selected to build a portfolio - Bitcoin is just *the* original crypto-currency, with the most capitalization, etc.  

Regardless of the above, building a proper portfolio will require a quantitative analysis of available options so that assets can be selected and added to a portfolio to minimize risk and maximize return; it is assumed that "investors are risk averse, meaning that given two portfolios that offer the same expected return, investors will prefer the less risky one. Thus, an investor will take on increased risk only if compensated by higher expected returns. Conversely, an investor who wants higher expected returns must accept more risk."<sup>[[2]](#mpt)</sup>  

Crypto-assets do have a wide variety of use cases associated with different markets, so selecting the later and classifying crypto-asset are the first steps that should be taken to facilitate diversification.  
According ton P. Kravchenko<sup>[[3]](#periodictable)</sup>, classification depends on five processes which may have at least three states (centralized, decentralized, not possible), and which can be managed by one or separate roles:  


  * Governance  
  * Custody  
  * Issuance and distribution
  * Transaction processing  
  * Audit  

Different combinations of the ways these processes are managed lead to hundred twenty five possible different types of digital assets and markets from which investors can pick to build a portfolio, including but not limited to crypto currencies, digital currencies, commodity-backed tokens, equity tokens, utility tokens, digital collectibles, etc.  
In parallel of type classification, assets should be analyzed and rated individually by aggregating some key data such as:<sup>[[4]](#weiss)</sup>  

  * Risk Index  
  * Reward Index  
  * Technology Index  
  * Adoption Index  

While to first two indexes can be extracted and calculated from market data, the last ones follow a rather manual process and will also be subjective to investor values and believes.  
Inventors will then have to optimize risk and return for each type portfolio, extract a type index to, at last, optimize the whole portfolio.  

<a name="coincount">[1]</a> [CoinMarketCap](#https://coinmarketcap.com/).  
<a name="mpt">[2]</a> [Modern portfolio theory - Wikipedia](#https://en.wikipedia.org/wiki/Modern_portfolio_theory#Risk_and_expected_return)  
<a name="periodictable">[3]</a> [The Periodic Table of Blockchain - Pavel Kravchenko](#https://www.coindesk.com/periodic-table-blockchain-classify-tokens/)  
<a name="weiss">[4]</a> [The Weiss Cryptocurrency Ratings Explained - Weiss Ratings, LLC](#https://weisscryptocurrencyratings.com/ratings/the-weiss-cryptocurrency-ratings-explained-15)  

#### 2.1.2 Rate, Optimize and Trade ####

Having their ideal portfolio distribution at hand, investors will then have to enter or exit markets and time their entry or exit to balance their actual portfolio distribution against benchmark and get the most reward out of the trade, most likely using technical analysis of each market.  

Overall, investors will follow a repetitive process consisting of:  

  * Asset rating  
  * Portfolio optimization  
  * Trade timing  

#### 2.1.3 Distribute Third Party Risk ####

Last and not least, investors could very well select and use a single exchange and have all their asset stored and traded there, that would be convenient but would also be very bad if that exchange goes Mt Gox<sup>[[1]](#mtgox)</sup>... Thus, investors are better off spreading their risk over multiple parties and wallets and give away convenience; as the saying goes: don't put all your eggs in the same basket.  

<a name="mtgox">[1]</a> [Mt. Gox - Wikipedia](#https://en.wikipedia.org/wiki/Mt._Gox)  

### 2.2 A Growing Complexity ###

Regardless of how investors build their portfolio, following and managing the later is a manual process involving multiple parameters. Even though services or software are available to ease some parts of the process such as rating, optimization and timing, none do cover the whole repetitive process of rating, optimizing and timing at once.  
Investors are thus required to handle data manually at some point in time of the process. Considering investors should keep track of multiple parameters of multiple crypto asset held at multiple third parties, complexity and reporting is growing exponentially with each new element added to a portfolio, which can quickly become hard to manage manually.

### 2.3 Trading Ease of Use for Risk ###

New crypto ETF<sup>[[1]](#funds)</sup> keep coming to the market with more the hundred and fifty active as off April 2018 and while they do cover the need for a service shading away the complexity of managing a crypto portfolio, investors do have to trust a single third party going against what cryptocurrencies have made possible: getting rid of the trusted third party.  
Investors clearly need a tool to get rid of this middle man by providing all functionality needed for an investor to manage crypto portfolio through a single, unified software than can run from home.  
It must allow investors to easily manage portfolio made of assets held at various exchanges and wallets, de facto reducing third party risk, but must also provide various service made possible by being at the core of portfolio operations such as financial reporting, market and performance analyses, automated trading, data intelligence.  

<a name="funds">[1]</a> 150+ funds according to [Bloomberg](#https://www.bloomberg.com/news/articles/2018-04-02/crypto-hedge-fund-bubble-begins-to-deflate-as-returns-tumble)  

### 3 Solution ###

The first and logical step to get rid of third party risk is to spread assets over multiple parties while managing all operation through a facade that standardize operations. This will be the main function of the proposed solution, Brane.  
Being at the core of all portfolio operations Brane will be able to provide a range of functionalities naturally building on each other.  

For the sake of transparency and audit-ability Brane will be release under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or any later version, allowing anyone to audit, contribute, fork or copy its code.  

It will be designed using the Julia language, mainly for its dynamic nature and high productivity and performance for both financial analytics and infrastructure.<sup>[[1]](#julia)</sup>

<a name="julia">[1]</a> [Julia - A new language for technical computing](#http://www.automatedtrader.net/articles/technology-strategy/157921/julia-_-a-new-language-for-technical-computing)  

### 3.1 Single Point of Entry ###

#### 3.1.1 External Data Service ####

Leveraging exchanges and wallets' API functionalities, Brane will allow investors to connect to multiple parties and retreive both market and investor's trade data over multiple assets. It will provide both a live connection and an unified interface for querying past data from multiple sources.  
The above naturally implies securely storing investor credential for private API calls.  

#### 3.1.2 Local Data Service ####

All data acquired through the external data service will be stored in persisve local databases split in two distinct categories: public and private, covering market and portfolio data respectively.

### 3.2 Financial Statements Module ###

The financial statements module will provide information about the financial position, financial performance, and cash flows of a portfolio, following International Accounting Standards<sup>[[1]](#ias)</sup>. To meet that objective, financial statements will include:  

  * a statement of financial position (balance sheet) at the end of the period  
  * a statement of profit or loss  
  * a statement of cash flows for the period  

<a name="ias">[1]</a> [IAS](#https://www.iasplus.com/en/standards/ias/ias1)  

### 3.3 Analyses Modules ###

#### 3.3.1 Market Analyses ####

The market analyses module will provide investors with markets' technical indicators. Brane will provide a library of indicators and allow investors to create and use their very own indicators.  
To avoid re-computing information, indicators' value will be stored by local data service in a dedicated persitive database for later access or analyses.

#### 3.3.2 Portfolio Analyses ####

The portfolio analyses module will provide investors with the ability to select, rate and calculate weight of assets that will make up a portfolio, depending on its selected characteristics. It will consist of several sub-modules listed here after.  

  * Portfolio characteristics definition including asset type, horizon, risk tolerance  
  * Assets rating, on the basis of both data feeded from the market analyses module and data entered manually by investors  
  * Determine ideal portfolio allocation following the (post) modern portfolio theory, Black-Litterman model, or any other relevant optimization model. 

### 3.4 Algorithmic Trading ###

Algorithmic trading will rely on Brane's analyses modules to provide investors with a wide range of indicators. These indicators will in turn be used to trigger buy or sell orders according to investors' input.  
Brane will allow investors to back test their strategy on historcal market data, enable it in a simulation mode a.k.a. paper trade and restrict trading to portfolio portions only.

### 3.5 Distributed Data Intelligence ###

Considering Brane will be used by multiple investors each using their very trading own strategy, Brane will build upon this by allowing investors to trade their strategies with other investors by comparing respective performances and signaling investors of possible strategy deal.  

#### 3.5.1 Market Data ####

Data beyond used indicator stored on distributed database

#### 3.5.2 Strategy Data ####

### 3.6 Dedicated Hardware ###

## 4 Conclusion ##

### 4.1 Summary ###

### 4.2 Future ###

## 5 Additional Resources ##

See specifications file in docs folder.

<!--  LocalWords:  MERCHANTABILITY periodictable weiss
 -->
