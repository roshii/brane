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

Table of Contents
=================
* 1 [Introduction](#1-introduction)
* 2 [Problem Statement](#2-problem-statement)
    * 2.1 [Investing in the crypto market](#21-investing-in-the-crypto-market)
    * 2.2 [Pain Points](#22-pain-points)
    * 2.3 [Needs](#23-needs)
    * 2.4 [Benefits](#24-benefits)
* 3 [Solution](#3-solution)
    * 3.1 [Single Point of Entry](#31-single-point-of-entry)
	* 3.2 [Reporting Made Easy](#32-reporting-made-easy)
	* 3.3 [Analyses Module](#33-analyses-module)
	* 3.4 [Algorithmic Trading](#34-algorithmic-trading)
	* 3.5 [Decentralized Data Intelligence](#35-decentralized-data-intelligence)
	* 3.6 [Dedicated Hardware](#36-dedicated-hardware)
* 4 [Conclusion](#4-conclusion)
* 5 [Additional Resources](#5-additional-resources)

## 1 Introduction ##

Bitcoin did successfully manage to remove trust in central authority that was so far required for any currency to be valued and used. Its ecosystem has developed over the years with the birth of hundreds different cryptocurrencies and a financial system being a pale copy of the fiat financial system with exchanges and funds all being handled by a third party which users have to blindly trust.  
While exchanges do greatly help to enhance market liquidity and cannot be overlooked by investors, funds or ETF do shade away market complexity and operations, acting as a simple facade for investors.  
The below describes the complexity of investing in cryptocurrencies and solution that investors could use to easily manage their investment without scarifying ease of use for third party risk.

## 2 Problem Statement ##

### 2.1 Investing in the crypto market ###

#### 2.1.1 Asset Selection ####

The crypto market offers a lot of investment options with more than sixteen hundreds crypto assets<sup>[[1]](#coincount)</sup> and any wannabee investor will have to do his home work before entering the market. In most cases, Bitcoin will be the first, default crypto-currency selected to build a portfolio - Bitcoin is just *the* original crypto-currency, with the most capitalization, etc.  

Regardless of the above, building a proper portfolio will require a quantitative analysis of available options so that assets can be selected and added to a portfolio to minimize risk and maximize return; it is assumed that "investors are risk averse, meaning that given two portfolios that offer the same expected return, investors will prefer the less risky one. Thus, an investor will take on increased risk only if compensated by higher expected returns. Conversely, an investor who wants higher expected returns must accept more risk."<sup>[[2]](#mpt)</sup>  

Crypto-assets do have a wide variety of use cases associated with different markets, so selecting the later and classifying crypto-asset are the first steps that should be taken to facilitate diversification.  
According ton P. Kravchenko<sup>[[3]](#periodictable)</sup>, classification depends on five processes which may have at least three states (centralized, decentralized, not possible), and which can be managed by one or separate roles:

- Governance  
- Custody  
- Issuance and distribution  
- Transaction processing  
- Audit  

Different combinations of the ways these processes are managed lead to hundred twenty five possible different types of digital assets and markets from which investors can pick to build a portfolio, including but not limited to crypto currencies, digital currencies, commodity-backed tokens, equity tokens, utility tokens, digital collectibles, etc.  
In parallel of type classification, assets should be analyzed and rated individually by aggregating some key data such as:<sup>[[4]](#weiss)</sup>

- Risk Index  
- Reward Index  
- Technology Index  
- Adoption Index  

While to first two indexes can be extracted and calculated from market data, the last ones follow a rather manual process and will also be subjective to investor values and believes.  
Inventors will then have to optimize risk and return for each type portfolio, extract a type index to, at last, optimize the whole portfolio.  

<a name="coincount">[1]</a> [CoinMarketCap](#https://coinmarketcap.com/).  
<a name="mpt">[2]</a> [Modern portfolio theory - Wikipedia](#https://en.wikipedia.org/wiki/Modern_portfolio_theory#Risk_and_expected_return)  
<a name="periodictable">[3]</a> [The Periodic Table of Blockchain - Pavel Kravchenko](#https://www.coindesk.com/periodic-table-blockchain-classify-tokens/)  
<a name="weiss">[4]</a> [The Weiss Cryptocurrency Ratings Explained - Weiss Ratings, LLC](#https://weisscryptocurrencyratings.com/ratings/the-weiss-cryptocurrency-ratings-explained-15)  

#### 2.1.2 Rate, Optimize and Trade ####

Having their ideal portfolio distribution at hand, investors will then have to enter or exit markets and time their entry or exit to balance their actual portfolio distribution against benchmark and get the most reward out of the trade, most likely using technical analysis of each market.  

Overall, investors will follow a repetitive process consisting of:  
- Asset rating  
- Portfolio optimization  
- Trade timing  

#### 2.1.3 Distribute Third Party Risk ####

Last and not least, investors could very well select and use a single exchange and have all their asset stored and traded there, that would be convenient but would also be very bad if that exchange goes Mt Gox<sup>[[1]](#mtgox)</sup>... Thus, investors are better off spreading their risk over multiple parties and wallets and give away convenience; as the saying goes: don't put all your eggs in the same basket.  

<a name="mtgox">[1]</a> [Mt. Gox - Wikipedia](#https://en.wikipedia.org/wiki/Mt._Gox)  

### 2.2 A growing complexity ###

Regardless of how investors build their portfolio, following and managing the later is a manual process involving multiple parameters. Even though services or software are available to ease some parts of the process such as rating, optimization and timing, none do cover the whole repetitive process of rating, optimizing and timing at once.  
Investors are thus required to handle data manually at some point in time of the process. Considering investors should keep track of multiple parameters of multiple crypto asset held at multiple third parties, complexity and reporting is growing exponentially with each new element added to a portfolio, which can quickly become hard to manage manually.

### 2.3 Trading Ease of Use for Risk ###

New crypto ETF<sup>[[1]](#funds)</sup> keep coming to the market with more the hundred and fifty active as off April 2018 and while they do cover the need for a service shading away the complexity of managing a crypto portfolio, investors do have to trust a single third party going against what cryptocurrencies have made possible: getting rid of the trusted third party.  
Investors clearly need a tool to get rid of this middle man by providing all functionality needed for an investor to manage crypto portfolio through a single, unified software than can run from home.  
It must allow investors to easily manage portfolio made of assets held at various exchanges and wallets, de facto reducing third party risk, but must also provide various service made possible by being at the core of portfolio operations such as financial reporting, market and performance analyses, automated trading, data intelligence.  

<a name="funds">[1]</a> 150+ funds according to [Bloomberg](#https://www.bloomberg.com/news/articles/2018-04-02/crypto-hedge-fund-bubble-begins-to-deflate-as-returns-tumble)  

## 3 Solution ##

The first and logical step to get rid of third party risk is to spread assets over multiple parties while managing all operation through a facade that standardize operations. This will be the main function of the proposed solution, Brane.  
Being at the core of all portfolio operations Brane will be able to provide a range of functionalities naturally building on each other.  

For the sake of transparency and audit-ability Brane will be release under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or any later version, allowing anyone to audit, contribute, fork or copy its code.  

It should be designed using a Julia language, mainly for its high productivity and performance for both financial analytics and infrastructure.<sup>[[1]](#julia)</sup>

<a name="julia">[1]</a> [Julia - A new language for technical computing](#http://www.automatedtrader.net/articles/technology-strategy/157921/julia-_-a-new-language-for-technical-computing)  

### 3.1 Single Point of Entry ###

#### 3.1.1 Live Data Service ####

Leveraging exchanges and wallets' API functionalities, Brane will allow investors to connect to multiple parties and retreive both market and investor's trade data over multiple assets, that implies securely storing investor credential for private API calls.

#### 3.1.2 Historical Data Service ####

Historical or past data must and will be splitted in two distinct categories: public and private.  
Public data or everything related to market will ideally be stored

### 3.2 Reporting Module ###

Data coming from exchanges and wallets must be stored in a local database with consistent data format allowing investors to generate statement and performance report.

### 3.3 Analyses Module ###

Building on its local database and live connection to exchanges, Brane must allow investors to analyze markets with the least possible delay and provide indicators on their respective actual. On top of the later, Brane must allow investors to calculate and advise ideal portfolio composition, taking in account investors' preferences.

#### 3.3.1 Market Analyses ####
#### 3.3.2 Portfolio Analyses ####

### 3.4 Algorithmic Trading ###

Algorithmic trading is the natural next step for Brane which can rely on its own market indicators and actual portfolio deviation to ideal one. This implies that Brane must allow investors to back test their strategy, enable it in a simulation mode a.k.a. paper trade and restrict trading to portfolio portions only.

### 3.5 Decentralized Data Intelligence ###

Considering Brane is used by multiple investors each using their very trading own strategy, Brane can build upon this by allowing investors to trade their strategies with other investors by comparing respective performances and signaling investors of possible strategy deal.  

#### 3.5.1 Market Data ####
#### 3.5.2 Strategy Data ####

### 3.6 Dedicated Hardware ###



## 4 Conclusion ##

### 4.1 Summary ###

### 4.2 Future ###

## 5 Additional Resources ##

See specifications file in docs folder.

<!--  LocalWords:  Brane MERCHANTABILITY periodictable weiss
 -->
