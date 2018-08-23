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
 

# Brane #

## Abstract ##

Brane is a cryptoassets portfolio management tool.

Table of Contents
=================
* 1 [Introduction](#1-introduction)
* 2 [Problem Statement](#2-problem-statement)
    * 2.1 [Today's Market](#21-today's-market)
    * 2.2 [Pain Points](#22-pain-points)
    * 2.3 [Needs](#23-needs)
    * 2.4 [Benefits](#24-benefits)
* 3 [Solution](#3-solution)
    * 3.1 [In Short](#31-in-short)
	* 3.2 [In Details](#32-in-details)
	    * 3.2.1 [Single Point of Entry](#321-single-point-of-entry)
		* 3.2.2 [Reporting Made Easy](#322-reporting-made-easy)
		* 3.2.3 [Analyses Module](#323-analyses-module)
		* 3.2.4 [Algorithmic Trading](#323-algorithic-trading)
		* 3.2.5 [Decentralized Data Intelligence](#324-decentralized-data-intelligence)
		* 3.2.6 [Dedicated Hardware](#326-dedicated-hardware)
* 4 [Conclusion](#4-conclusion)
* 5 [Additional Resources](#5-additional-resources)

## 1 Introduction ##

Bitcoin did successfully manage to remove trust in central authority that was so far requiered for any currency to be valued and used.  
While ecosystem has developped over the years with the birth of hundreds differents cryptocurrencies<sup>[1](#footnote1)</sup>, the whole financial system around it remains a pale copy of the fiat financial system with exchanges, funds<sup>[2](#footnote2)</sup>, futures and others, all being handled by a third party which users have to blindy trust.  

<a name="footnote1">1</a>: 1600+ cryptocurrencies according to [CoinMarketCap](#https://coinmarketcap.com/).  
<a name="footnote2">2</a>: 150+ funds according to [Bloomberg](#https://www.bloomberg.com/news/articles/2018-04-02/crypto-hedge-fund-bubble-begins-to-deflate-as-returns-tumble)  

## 2 Problem Statement ##

### 2.1 Investing in the crypto market ###

The cryto market offers a lot of investment options with more than sixteen hundreds cryptoassets and any wanabee investor will have to do his home work before entering the market. In most cases, Bitcoin will be the first, default cryptocurrency selected to build a portfolio - Bitcoin is just *the* original cryptocurrency, with the most capitalization, etc.  

Regardless of the above, building a proper porfolio will require a quantitative analysis of available options so that assests can be selected and added to a portfolio to minimze risk and maximize return; it is assumed that "investors are risk averse, meaning that given two portfolios that offer the same expected return, investors will prefer the less risky one. Thus, an investor will take on increased risk only if compensated by higher expected returns. Conversely, an investor who wants higher expected returns must accept more risk."<sup>[*](#mpt)</sup>  


Cryptoassets do have a wide variety of use cases associated with different markets, so selecting the later and classifying cryptoasset are the first steps that should be taken to facilitate diversification.  
According ton P. Kravchenko<sup>[*](#periodictable)</sup>, classification depends on five processes which may have at least three states (centralized, decentralized, not possible), and which can be managed by one or separate roles:

- Governance  
- Custody  
- Issuance and distribution  
- Transaction processing  
- Audit  

Different combinations of the ways these processes are managed lead to hundred twenty five possible different types of digital assets and markets from which investors can pick to build a portfolio, including but not limited to crypto currencies, digital currencies, commodity-backed tokens, equity tokens, utility tokens, digital collectibles, etc.  
In parallel of type classification, assets should be analyzed and rated individually by aggregating some key data such as:<sup>[*](#weiss)</sup>

- Risk Index  
- Reward Index  
- Technology Index  
- Adoption Index  

While to first two indexes can be extracted and calculated from market data, the last ones follow a rather manual process and will also be subjective to invertor values and believes.  
Invertors will then have to optimize risk and return for each type portfolio, extract a type index to, at last, optimize the whole portfolio.  

Having their ideal portfolio distribution at hand, investors will then have to enter or exit markets and time their entry or exit to balance their actual portofolio distribution against benchmark and get the most reward out of the trade, most likely using technical analysis of each market.  

Overall, invertors will follow a repetitive process consisting of:
- Asset rating
- Portfolio optimization
- Trade timing

Last and not least, investors could very well select and use a single exchange and have all their asset stored and traded there, that would be convinient but would also be very bad if that exchange goes Mt Gox<sup>[*](#mtgox)</sup>... Thus, investors are better off spreading their risk over multiple parties and wallets and give away convinience; as the saying goes: don't put all your eggs in the same basket.  

<a name="mpt">*</a> [Modern portfolio theory - Wikipedia](#https://en.wikipedia.org/wiki/Modern_portfolio_theory#Risk_and_expected_return)

<a name="periodictable">*</a> [The Periodic Table of Blockchain - Pavel Kravchenko](#https://www.coindesk.com/periodic-table-blockchain-classify-tokens/)

<a name="weiss">*</a> [The Weiss Cryptocurrency Ratings Explained - Weiss Ratings, LLC](#https://weisscryptocurrencyratings.com/ratings/the-weiss-cryptocurrency-ratings-explained-15)

<a name="mtgox">*</a> [Mt. Gox - Wikipedia](#https://en.wikipedia.org/wiki/Mt._Gox)


### 2.2 A growing complexity ###

Regardless of how investors build their portfolio, following and managing the later is a manual process involving multiple parameters. Even though services or sofware are available for part of the process such as rating, optimization and timing, none do cover the whole repetitive process of rating, optimmizing and timing at once.  
Investors are thus required to handle data manually at some point in time of the process. Considering investors should keep track of multiple parameters of multiple crypto asset held at multiple third parties, complexity and reporting is growing exponentilly with each new element in the portfolio, which can quickly become hard to manage manually.

### 2.3 What do crypto investors need? ###

New crypto ETF keep coming to the market with more the hundred and fifty active as off April 2018 and while they do cover the need for a service shading away the complexity of managing a crypto portfolio, investors do have to trust a single third party going against what cryptocurrencies have made possible: getting rid of the trusted third party.  
Investors clearly need a tool to get rid of this middle man by providing all functionallity needed for an investor to manage crypto portfolio through a single, unified software than can run from home.

### 2.4 Benefits ###

Not only Brane will allow investors to manage portfolio made of assests held at various exchanges and wallets, de facto reducing third party risk, but will also provide various service made possible by beeing at the core of portfolio operations such as financial reporting, market and performance analyses and automated trading.


## 3 Solution ##

First and foremost Brane will be release under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or any later version, allowing anyone to audit, contribute, fork or copy its code.  

It will be designed using a fast number processing language: Julia.  


### 3.1 Single Point of Entry ###

Brane main benefit is its single point of entry to a multi-party, multi-assest portfolio that can simply be made possible by leveraging exchanges and wallets' API functionnality.

### 3.2 Reporting Module ###

Data coming from exchanges and wallets must be stored in a local database with consistent data format allowing investors to generate statement and performance report.

### 3.3 Analyses Module ###

Building on its local database and live connection to exchanges, Brane must allow investors to analyse markets with the least possible delay and provide indicators on their respective actuals. On top of the later, Brane must allow investors to calculate and advise ideal portfolio composition, taking in account investors' preferences.

#### 3.3.1 Market Analyses ####
#### 3.3.2 Portfolio Analyses ####

### 3.4 Algorithmic Trading ###

Algorithic trading is the natural next step for Brane which can rely onits own market indicators and actual portfolio deviation to ideal one. This implies that Brane must allow investors to back test their startegy, enable it in a simulation mode a.k.a. paper trade and restrict trading to portfolio portions only.

### 3.5 Decentralized Data Intelligence ###

Considering Brane is used by multiple investors each using their very trading own strategy, Brane can build upon this by allowing investors to trade their startegies with other investors by comparing respective performances and signaling investors of possible strategy deal.  

#### 3.5.1 Market Data ####
#### 3.5.2 Startegy Data ####

### 3.6 Dedicated Hardware ###



## 4 Conclusion ##

### 4.1 Summary ###

### 4.2 Future ###

## 5 Additional Resources ##

See specifications file in docs folder.
