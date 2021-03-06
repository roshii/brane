# The Case for a Crypto-Portfolio Management Tool

    Copyright (C)  Simon J. Castano.
    Permission is granted to copy, distribute and/or modify this document
    under the terms of the GNU Free Documentation License, Version 1.3
    or any later version published by the Free Software Foundation;
    with no Invariant Sections, no Front-Cover Texts, and no Back-Cover Texts.
    A copy of the license is included in the section entitled "GNU
    Free Documentation License". 

## Abstract

This document explores problems faced by crypto-investors for managing their investments.  
It argues in favor of a portfolio management tool, Brane, describes its required functionalities and set a road map for future extensions. 

## Table of Contents

1. [Introduction](#introduction)
2. [Problem Statement](#problem-statement)
    1. [Investing in the Crypto Market](#investing-in-the-crypto-market)
        1. [Asset Selection](#asset-selection)
        2. [Optimize and Trade](#optimize-and-trade)
        3. [Trading Ease of Use for Risk](#trading-ease-of-use-for-risk)
    2. [A Growing Complexity](#a-growing-complexity)
    3. [Trading Ease of Use for Risk](#trading-ease-of-use-for-risk)
3. [Proposed Solution](#proposed-solution)
    1. [One for All](#one-for-all)
    2. [Financial Statements Module](#financial-statements-module)
    3. [Analyses Modules](#analyses-modules)
    4. [Algorithmic Trading](#algorithmic-trading)
4. [Future](#future)
    1. [Distributed Data](#distributed-data)
    2. [Distributed Computing](#distributed-computing)
    3. [Dedicated Hardware](#dedicated-hardware)
5. [Conclusion](#conclusion)
6. [Additional Resources](#additional-resources)
    1. [A Note About Decentralized Exchange](#a-note-about-decentralized-exchange)
	2. [GNU Free Documentation License](#gnu-free-documentation-license)

## Introduction <a name="introduction"></a>

Bitcoin did successfully manage to remove trust in central authority that was so far required for any currency to be valued and used. Its ecosystem has developed over the years with the birth of hundreds different cryptocurrencies and a financial system being a pale copy of the fiat financial system with exchanges and funds all being handled by a third party which users have to blindly trust.  
While exchanges do greatly help to enhance market liquidity and cannot be overlooked by investors, funds or ETF simply shade away market complexity and operations, acting as a simple facade for investors.  
The below describes the complexity of investing in cryptocurrencies and solution that investors could use to easily manage their investments without scarifying ease of use for third party risk.

## Problem Statement <a name="problem-statement"></a>

### Investing in the Crypto Market <a name="investing-in-the-crypto-market"></a>

The crypto market offers a lot of investment options with more than sixteen hundreds crypto assets<sup>[[1]](#coincount)</sup> and any wannabee investor will have to do his home work before entering the market. In most cases, Bitcoin will be the first, default crypto-currency selected to build a portfolio - Bitcoin is just *the* original crypto-currency, with the most capitalization, etc.  

Regardless of the above, building a proper portfolio will require a quantitative analysis of available options so that assets can be selected and added to a portfolio if appropriate. It is assumed that "investors are risk averse, meaning that given two portfolios that offer the same expected return, investors will prefer the less risky one. Thus, an investor will take on increased risk only if compensated by higher expected returns. Conversely, an investor who wants higher expected returns must accept more risk."<sup>[[2]](#mpt)</sup>  

#### Asset Selection <a name="asset-selection"></a>

To begin with, investors have to understand what they are investing in and may start with classifying crypto-assets. Exhibiting a wide range of use cases associated with different markets, similar assets will tend to behave similarly in given market conditions and their classification will help investor to diversify.  

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

<a name="coincount">[1]</a> [CoinMarketCap](https://coinmarketcap.com/)  
<a name="mpt">[2]</a> [Modern portfolio theory - Wikipedia](https://en.wikipedia.org/wiki/Modern_portfolio_theory#Risk_and_expected_return)  
<a name="periodictable">[3]</a> [The Periodic Table of Blockchain - Pavel Kravchenko](https://www.coindesk.com/periodic-table-blockchain-classify-tokens)  
<a name="weiss">[4]</a> [The Weiss Cryptocurrency Ratings Explained - Weiss Ratings, LLC](https://weisscryptocurrencyratings.com/ratings/the-weiss-cryptocurrency-ratings-explained-15)  

#### Optimize and Trade <a name="optimize-and-trade"></a>

Investors are then able to optimize risk and return for their portfolio using rating and classification data collected previously. With their ideal portfolio distribution at hand, investors can enter and/or exit markets to balance their actual portfolio distribution against benchmark and time their trades to get the most reward out of it.  

Overall, investors will keep on repeating the following processes, to adapt to market and maximize return:  

  * Rating assets  
  * Optimizing portfolio  
  * Timing trades  

#### Distribute Third Party Risk <a name="distribute-third-party-risk"></a>

Last and not least, investors could very well select and use a single exchange and have all their asset stored and traded there, that would be convenient but would also be very bad if that exchange goes Mt Gox<sup>[[1]](#mtgox)</sup>... Thus, investors are better off spreading their risk over multiple parties and wallets and give away some convenience; as the saying goes: don't put all your eggs in the same basket.  

<a name="mtgox">[1]</a> [Mt. Gox - Wikipedia](https://en.wikipedia.org/wiki/Mt._Gox)  

### A Growing Complexity <a name="a-growing-complexity"></a>

Regardless of how investors build their portfolio, following and managing the later is a manual process involving multiple parameters. Even though services or software are available to ease some parts of the process such as rating, optimization and timing, none do cover the whole repetitive process of rating, optimizing and timing at once.  
Investors are thus required to handle data manually at some point in time of the process. Considering investors should keep track of multiple parameters of multiple crypto asset held at multiple third parties, complexity and reporting is growing exponentially with each new element added to a portfolio, which can quickly become hard to manage manually.

### Trading Ease of Use for Risk <a name="trading-ease-of-use-for-risk"></a>

New crypto ETF<sup>[[1]](#funds)</sup> keep coming to the market with more the hundred and fifty active as off April 2018 and while they do cover the need for a service, shading away the complexity of managing a crypto portfolio, investors do have to trust a single third party going against what cryptocurrencies have made possible: getting rid of the trusted third party.  

<a name="funds">[1]</a> 150+ funds according to [Bloomberg](https://www.bloomberg.com/news/articles/2018-04-02/crypto-hedge-fund-bubble-begins-to-deflate-as-returns-tumble)  

### Proposed Solution <a name="proposed-solution"></a>

Investors clearly need a tool to get rid of this middle man by providing all functionalities needed to manage crypto-portfolios through a single, unified software than can run from home.  
It must allow investors to easily manage portfolio made of assets held at various exchanges and wallets, de facto reducing third party risk, but must also provide various service made possible by being at the core of portfolio operations such as financial reporting, market and performance analyses, automated trading, data intelligence. It will ideally connect to decentralized exchanges to truly decentralize investments.  

The first and logical step to get rid of third party risk is to spread assets over multiple parties while managing all operation through a facade that standardize operations. This will consequently reduce investors' risk without giving away ease of use. And this will be the main function of the proposed solution: Brane.  
Being at the core of all portfolio operations Brane will be able to provide a range of added functionalities naturally building on each other.  

For the sake of transparency and audit-ability Brane will be release under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or any later version, allowing anyone to audit, contribute, fork or copy its code.  

It will be designed using the Julia language, mainly for its dynamic nature and high productivity and performance for both financial analytics and infrastructure.<sup>[[1]](#julia)</sup>

<a name="julia">[1]</a> [Julia - A new language for technical computing](#http://www.automatedtrader.net/articles/technology-strategy/157921/julia-_-a-new-language-for-technical-computing)  

### One for All <a name="one-for-all"></a>

#### Unified API Language <a name="unfified-api-language"></a>

Interactions with services will be standardized to allow investors to use external services without having to worry about the various API specifics. It will just simplify the management of multiple parties by unifying query constructs.

#### External Data Service <a name="external-data-service"></a>

Leveraging the unified trading API language, Brane will allow investors to connect to multiple parties to retrieve both market and investor's trade data over multiple assets. It will provide both live connection and construct for querying past data from multiple sources.  
The above naturally implies securely storing investor's credential for private API calls.  

#### Local Data Service <a name="local-data-service"></a>

All data acquired through the external data service will be stored in persistive local databases split in categories: e.g. market data, portfolio data, asset rating, etc.

### Financial Statements Module <a name="financial-statements-module"></a>

The financial statements module will provide information about the financial position, financial performance, and cash flows of a portfolio, following International Accounting Standards<sup>[[1]](#ias)</sup>. To meet that objective, financial statements will include:  

  * a statement of financial position (balance sheet) at the end of the period  
  * a statement of profit or loss  
  * a statement of cash flows for the period  

In other words, this module will simply query and concatenate local data in a predefined (or user-defined) formats.  

<a name="ias">[1]</a> [IAS](https://www.iasplus.com/en/standards/ias/ias1)  

### Analyses Modules <a name="analyses-modules"></a>

#### Market Analyses <a name="market-analyses"></a>

The market analyses module will provide investors with markets' technical indicators. Brane will provide a library of indicators and allow investors to create and use their very own indicators.  
To avoid re-computing information, indicators' value will be stored by the local data service in a specific category for later access or analyses.

#### Portfolio Analyses <a name="portfolio-analyses"></a>

The portfolio analyses module will provide investors with the ability to select, rate and calculate weight of assets that will make up a portfolio, depending on its selected characteristics. It will consist of several sub-modules including:  

  * Portfolio characteristics definition including asset type, horizon, risk tolerance  
  * Assets rating, on the basis of both data feed from the market analyses module and data entered manually by investors  
  * Portfolio optimization following the (post) modern portfolio theory, Black-Litterman model, or any relevant optimization model. 

### Algorithmic Trading <a name="algorithmic-trading"></a>

Algorithmic trading will rely on Brane's analyses modules to provide investors with a wide range of indicators. These indicators will in turn be used to trigger buy or sell orders according to conditions defined by investor.  
It will also allow investors to back test strategy, run it in simulation mode a.k.a. paper trade and restrict trading to portfolio portions only.

## Future <a name="future"></a>

Brane is first intended to be used by tech-savvy investors that have basic knowledge in scripting and operating servers. In the longer term though, Brane will develop GUI to facilitate user interactions.  
Other modules will be investigated, aiming at distributing trading data, intelligence and computing, further described here after. These later modules combined with a friendly GUI would allow any investor to use Brane, purchasing strategy, computing and/or data from investor to investor.  

### Distributed Data <a name="distributed-data"></a>

Brane will allow users to reduce or backup local data by distributing whats non critical<sup>[[1]](#critical)</sup> over multiple nodes. It will also create a decentralized data market in which each and every node is free to participate.

<a name="critical">[1]</a> i.e. data not required for calculating indicators.  
 
#### Market Data <a name="market-data"></a>

This will be an automated system in which market data beyond date ranges used to calculate indicators, will be stored in a distributed database.  
Ideally, data distribution would be similar to torrents and before being added publicly, data will have to be signed for correctness by multiple users. While market data will easily be verifiable, indicators will require multiple computation to ensure correctness. On the other hand, this data would need to be calculated and verified only once, allowing later investor to simply retrieve it.  

#### Strategy Data <a name="strategy-data"></a>

This module will allow investors to trade their strategies with other investors by comparing respective performances and signaling investors of possible strategy deal.  
Strategy data will have to be signed by investor before publication to a strategy market. Such signature will be taking in account market data from the distributed market data to allow anyone to verify for strategy performance without revealing strategy. A strategy buyer would receive strategy private key against a fee for decryption of the later.  
Strategy market will be an automated system, matching best strategy for investors depending on their risk profiles, preferences and views on crypto market.

### Distributed Computing <a name="distributed-computing"></a>

Calculating indicators and optimizing portfolio might end up being resource intensive and we could imagine some investors willing to use resources from other nodes to speed up computation, optimization. This will require some sort of proof of work system in which result would be provided to requester only. And instead of being competitive, result would be delivered by a collaborative distributed computation network.  
This could allow investors to develop and test trading strategy using deep learning algorithm while allowing others to rent their spare computing capabilities. Other setup, combined with the distributed strategy market could give birth to collaborative funds in which investors having similar profile and objectives would mutualize resources.

### Dedicated Hardware <a name="dedicated-hardware"></a>

A dedicated hardware running Brane along with 100% free software will be developed in the longer term to facilitate deployment. This will allow investor to simply plug it, go through configuration and have their personal crypto fund running within the hour.

## Conclusion <a name="conclusion"></a>

With its core modules interacting with each others, i.e. data service, reporting, analyses and algorithmic trading, Brane will offer all the tools necessary to private investors to manage their crypto fund with a simple internet connection and computer. On top of the later, investors will be able to include or exclude any third party or asset they deem non trustworthy, following their very own analyses or belief.  
It the longer term Brane, will not only connect investors and create a decentralized market for data and computing resources but will also allow anyone with limited knowledge in crypto investment to participate in this market and delegate management to Brane which will retrieve and run best proven strategies matching investor's profile.  

## Additional Resources <a name="additional-resources"></a>

Please refer to [Brane Project Web Site](https://www.brane.cc)  

### A Note About Decentralized Exchange <a name="a-note-about-decentralized-exchange"></a>

Brane is originally thought to be used with decentralized exchange which will hopefully be develop and slowly replace classic exchange. As soon as this becomes a reality, Brane will make the most sense by allowing investor to remain in total control of their funds, providing a range of functionalities, expendables by means of modules. 


### GNU Free Documentation License <a name="gnu-free-documentation-license"></a>

Version 1.3, 3 November 2008

Copyright (C) 2000, 2001, 2002, 2007, 2008 Free Software Foundation,
Inc. <https://fsf.org/>

Everyone is permitted to copy and distribute verbatim copies of this
license document, but changing it is not allowed.

#### 0. PREAMBLE

The purpose of this License is to make a manual, textbook, or other
functional and useful document "free" in the sense of freedom: to
assure everyone the effective freedom to copy and redistribute it,
with or without modifying it, either commercially or noncommercially.
Secondarily, this License preserves for the author and publisher a way
to get credit for their work, while not being considered responsible
for modifications made by others.

This License is a kind of "copyleft", which means that derivative
works of the document must themselves be free in the same sense. It
complements the GNU General Public License, which is a copyleft
license designed for free software.

We have designed this License in order to use it for manuals for free
software, because free software needs free documentation: a free
program should come with manuals providing the same freedoms that the
software does. But this License is not limited to software manuals; it
can be used for any textual work, regardless of subject matter or
whether it is published as a printed book. We recommend this License
principally for works whose purpose is instruction or reference.

#### 1. APPLICABILITY AND DEFINITIONS

This License applies to any manual or other work, in any medium, that
contains a notice placed by the copyright holder saying it can be
distributed under the terms of this License. Such a notice grants a
world-wide, royalty-free license, unlimited in duration, to use that
work under the conditions stated herein. The "Document", below, refers
to any such manual or work. Any member of the public is a licensee,
and is addressed as "you". You accept the license if you copy, modify
or distribute the work in a way requiring permission under copyright
law.

A "Modified Version" of the Document means any work containing the
Document or a portion of it, either copied verbatim, or with
modifications and/or translated into another language.

A "Secondary Section" is a named appendix or a front-matter section of
the Document that deals exclusively with the relationship of the
publishers or authors of the Document to the Document's overall
subject (or to related matters) and contains nothing that could fall
directly within that overall subject. (Thus, if the Document is in
part a textbook of mathematics, a Secondary Section may not explain
any mathematics.) The relationship could be a matter of historical
connection with the subject or with related matters, or of legal,
commercial, philosophical, ethical or political position regarding
them.

The "Invariant Sections" are certain Secondary Sections whose titles
are designated, as being those of Invariant Sections, in the notice
that says that the Document is released under this License. If a
section does not fit the above definition of Secondary then it is not
allowed to be designated as Invariant. The Document may contain zero
Invariant Sections. If the Document does not identify any Invariant
Sections then there are none.

The "Cover Texts" are certain short passages of text that are listed,
as Front-Cover Texts or Back-Cover Texts, in the notice that says that
the Document is released under this License. A Front-Cover Text may be
at most 5 words, and a Back-Cover Text may be at most 25 words.

A "Transparent" copy of the Document means a machine-readable copy,
represented in a format whose specification is available to the
general public, that is suitable for revising the document
straightforwardly with generic text editors or (for images composed of
pixels) generic paint programs or (for drawings) some widely available
drawing editor, and that is suitable for input to text formatters or
for automatic translation to a variety of formats suitable for input
to text formatters. A copy made in an otherwise Transparent file
format whose markup, or absence of markup, has been arranged to thwart
or discourage subsequent modification by readers is not Transparent.
An image format is not Transparent if used for any substantial amount
of text. A copy that is not "Transparent" is called "Opaque".

Examples of suitable formats for Transparent copies include plain
ASCII without markup, Texinfo input format, LaTeX input format, SGML
or XML using a publicly available DTD, and standard-conforming simple
HTML, PostScript or PDF designed for human modification. Examples of
transparent image formats include PNG, XCF and JPG. Opaque formats
include proprietary formats that can be read and edited only by
proprietary word processors, SGML or XML for which the DTD and/or
processing tools are not generally available, and the
machine-generated HTML, PostScript or PDF produced by some word
processors for output purposes only.

The "Title Page" means, for a printed book, the title page itself,
plus such following pages as are needed to hold, legibly, the material
this License requires to appear in the title page. For works in
formats which do not have any title page as such, "Title Page" means
the text near the most prominent appearance of the work's title,
preceding the beginning of the body of the text.

The "publisher" means any person or entity that distributes copies of
the Document to the public.

A section "Entitled XYZ" means a named subunit of the Document whose
title either is precisely XYZ or contains XYZ in parentheses following
text that translates XYZ in another language. (Here XYZ stands for a
specific section name mentioned below, such as "Acknowledgements",
"Dedications", "Endorsements", or "History".) To "Preserve the Title"
of such a section when you modify the Document means that it remains a
section "Entitled XYZ" according to this definition.

The Document may include Warranty Disclaimers next to the notice which
states that this License applies to the Document. These Warranty
Disclaimers are considered to be included by reference in this
License, but only as regards disclaiming warranties: any other
implication that these Warranty Disclaimers may have is void and has
no effect on the meaning of this License.

#### 2. VERBATIM COPYING

You may copy and distribute the Document in any medium, either
commercially or noncommercially, provided that this License, the
copyright notices, and the license notice saying this License applies
to the Document are reproduced in all copies, and that you add no
other conditions whatsoever to those of this License. You may not use
technical measures to obstruct or control the reading or further
copying of the copies you make or distribute. However, you may accept
compensation in exchange for copies. If you distribute a large enough
number of copies you must also follow the conditions in section 3.

You may also lend copies, under the same conditions stated above, and
you may publicly display copies.

#### 3. COPYING IN QUANTITY

If you publish printed copies (or copies in media that commonly have
printed covers) of the Document, numbering more than 100, and the
Document's license notice requires Cover Texts, you must enclose the
copies in covers that carry, clearly and legibly, all these Cover
Texts: Front-Cover Texts on the front cover, and Back-Cover Texts on
the back cover. Both covers must also clearly and legibly identify you
as the publisher of these copies. The front cover must present the
full title with all words of the title equally prominent and visible.
You may add other material on the covers in addition. Copying with
changes limited to the covers, as long as they preserve the title of
the Document and satisfy these conditions, can be treated as verbatim
copying in other respects.

If the required texts for either cover are too voluminous to fit
legibly, you should put the first ones listed (as many as fit
reasonably) on the actual cover, and continue the rest onto adjacent
pages.

If you publish or distribute Opaque copies of the Document numbering
more than 100, you must either include a machine-readable Transparent
copy along with each Opaque copy, or state in or with each Opaque copy
a computer-network location from which the general network-using
public has access to download using public-standard network protocols
a complete Transparent copy of the Document, free of added material.
If you use the latter option, you must take reasonably prudent steps,
when you begin distribution of Opaque copies in quantity, to ensure
that this Transparent copy will remain thus accessible at the stated
location until at least one year after the last time you distribute an
Opaque copy (directly or through your agents or retailers) of that
edition to the public.

It is requested, but not required, that you contact the authors of the
Document well before redistributing any large number of copies, to
give them a chance to provide you with an updated version of the
Document.

#### 4. MODIFICATIONS

You may copy and distribute a Modified Version of the Document under
the conditions of sections 2 and 3 above, provided that you release
the Modified Version under precisely this License, with the Modified
Version filling the role of the Document, thus licensing distribution
and modification of the Modified Version to whoever possesses a copy
of it. In addition, you must do these things in the Modified Version:

-   A. Use in the Title Page (and on the covers, if any) a title
    distinct from that of the Document, and from those of previous
    versions (which should, if there were any, be listed in the
    History section of the Document). You may use the same title as a
    previous version if the original publisher of that version
    gives permission.
-   B. List on the Title Page, as authors, one or more persons or
    entities responsible for authorship of the modifications in the
    Modified Version, together with at least five of the principal
    authors of the Document (all of its principal authors, if it has
    fewer than five), unless they release you from this requirement.
-   C. State on the Title page the name of the publisher of the
    Modified Version, as the publisher.
-   D. Preserve all the copyright notices of the Document.
-   E. Add an appropriate copyright notice for your modifications
    adjacent to the other copyright notices.
-   F. Include, immediately after the copyright notices, a license
    notice giving the public permission to use the Modified Version
    under the terms of this License, in the form shown in the
    Addendum below.
-   G. Preserve in that license notice the full lists of Invariant
    Sections and required Cover Texts given in the Document's
    license notice.
-   H. Include an unaltered copy of this License.
-   I. Preserve the section Entitled "History", Preserve its Title,
    and add to it an item stating at least the title, year, new
    authors, and publisher of the Modified Version as given on the
    Title Page. If there is no section Entitled "History" in the
    Document, create one stating the title, year, authors, and
    publisher of the Document as given on its Title Page, then add an
    item describing the Modified Version as stated in the
    previous sentence.
-   J. Preserve the network location, if any, given in the Document
    for public access to a Transparent copy of the Document, and
    likewise the network locations given in the Document for previous
    versions it was based on. These may be placed in the "History"
    section. You may omit a network location for a work that was
    published at least four years before the Document itself, or if
    the original publisher of the version it refers to
    gives permission.
-   K. For any section Entitled "Acknowledgements" or "Dedications",
    Preserve the Title of the section, and preserve in the section all
    the substance and tone of each of the contributor acknowledgements
    and/or dedications given therein.
-   L. Preserve all the Invariant Sections of the Document, unaltered
    in their text and in their titles. Section numbers or the
    equivalent are not considered part of the section titles.
-   M. Delete any section Entitled "Endorsements". Such a section may
    not be included in the Modified Version.
-   N. Do not retitle any existing section to be Entitled
    "Endorsements" or to conflict in title with any Invariant Section.
-   O. Preserve any Warranty Disclaimers.

If the Modified Version includes new front-matter sections or
appendices that qualify as Secondary Sections and contain no material
copied from the Document, you may at your option designate some or all
of these sections as invariant. To do this, add their titles to the
list of Invariant Sections in the Modified Version's license notice.
These titles must be distinct from any other section titles.

You may add a section Entitled "Endorsements", provided it contains
nothing but endorsements of your Modified Version by various
parties—for example, statements of peer review or that the text has
been approved by an organization as the authoritative definition of a
standard.

You may add a passage of up to five words as a Front-Cover Text, and a
passage of up to 25 words as a Back-Cover Text, to the end of the list
of Cover Texts in the Modified Version. Only one passage of
Front-Cover Text and one of Back-Cover Text may be added by (or
through arrangements made by) any one entity. If the Document already
includes a cover text for the same cover, previously added by you or
by arrangement made by the same entity you are acting on behalf of,
you may not add another; but you may replace the old one, on explicit
permission from the previous publisher that added the old one.

The author(s) and publisher(s) of the Document do not by this License
give permission to use their names for publicity for or to assert or
imply endorsement of any Modified Version.

#### 5. COMBINING DOCUMENTS

You may combine the Document with other documents released under this
License, under the terms defined in section 4 above for modified
versions, provided that you include in the combination all of the
Invariant Sections of all of the original documents, unmodified, and
list them all as Invariant Sections of your combined work in its
license notice, and that you preserve all their Warranty Disclaimers.

The combined work need only contain one copy of this License, and
multiple identical Invariant Sections may be replaced with a single
copy. If there are multiple Invariant Sections with the same name but
different contents, make the title of each such section unique by
adding at the end of it, in parentheses, the name of the original
author or publisher of that section if known, or else a unique number.
Make the same adjustment to the section titles in the list of
Invariant Sections in the license notice of the combined work.

In the combination, you must combine any sections Entitled "History"
in the various original documents, forming one section Entitled
"History"; likewise combine any sections Entitled "Acknowledgements",
and any sections Entitled "Dedications". You must delete all sections
Entitled "Endorsements".

#### 6. COLLECTIONS OF DOCUMENTS

You may make a collection consisting of the Document and other
documents released under this License, and replace the individual
copies of this License in the various documents with a single copy
that is included in the collection, provided that you follow the rules
of this License for verbatim copying of each of the documents in all
other respects.

You may extract a single document from such a collection, and
distribute it individually under this License, provided you insert a
copy of this License into the extracted document, and follow this
License in all other respects regarding verbatim copying of that
document.

#### 7. AGGREGATION WITH INDEPENDENT WORKS

A compilation of the Document or its derivatives with other separate
and independent documents or works, in or on a volume of a storage or
distribution medium, is called an "aggregate" if the copyright
resulting from the compilation is not used to limit the legal rights
of the compilation's users beyond what the individual works permit.
When the Document is included in an aggregate, this License does not
apply to the other works in the aggregate which are not themselves
derivative works of the Document.

If the Cover Text requirement of section 3 is applicable to these
copies of the Document, then if the Document is less than one half of
the entire aggregate, the Document's Cover Texts may be placed on
covers that bracket the Document within the aggregate, or the
electronic equivalent of covers if the Document is in electronic form.
Otherwise they must appear on printed covers that bracket the whole
aggregate.

#### 8. TRANSLATION

Translation is considered a kind of modification, so you may
distribute translations of the Document under the terms of section 4.
Replacing Invariant Sections with translations requires special
permission from their copyright holders, but you may include
translations of some or all Invariant Sections in addition to the
original versions of these Invariant Sections. You may include a
translation of this License, and all the license notices in the
Document, and any Warranty Disclaimers, provided that you also include
the original English version of this License and the original versions
of those notices and disclaimers. In case of a disagreement between
the translation and the original version of this License or a notice
or disclaimer, the original version will prevail.

If a section in the Document is Entitled "Acknowledgements",
"Dedications", or "History", the requirement (section 4) to Preserve
its Title (section 1) will typically require changing the actual
title.

#### 9. TERMINATION

You may not copy, modify, sublicense, or distribute the Document
except as expressly provided under this License. Any attempt otherwise
to copy, modify, sublicense, or distribute it is void, and will
automatically terminate your rights under this License.

However, if you cease all violation of this License, then your license
from a particular copyright holder is reinstated (a) provisionally,
unless and until the copyright holder explicitly and finally
terminates your license, and (b) permanently, if the copyright holder
fails to notify you of the violation by some reasonable means prior to
60 days after the cessation.

Moreover, your license from a particular copyright holder is
reinstated permanently if the copyright holder notifies you of the
violation by some reasonable means, this is the first time you have
received notice of violation of this License (for any work) from that
copyright holder, and you cure the violation prior to 30 days after
your receipt of the notice.

Termination of your rights under this section does not terminate the
licenses of parties who have received copies or rights from you under
this License. If your rights have been terminated and not permanently
reinstated, receipt of a copy of some or all of the same material does
not give you any rights to use it.

#### 10. FUTURE REVISIONS OF THIS LICENSE

The Free Software Foundation may publish new, revised versions of the
GNU Free Documentation License from time to time. Such new versions
will be similar in spirit to the present version, but may differ in
detail to address new problems or concerns. See
<https://www.gnu.org/licenses/>.

Each version of the License is given a distinguishing version number.
If the Document specifies that a particular numbered version of this
License "or any later version" applies to it, you have the option of
following the terms and conditions either of that specified version or
of any later version that has been published (not as a draft) by the
Free Software Foundation. If the Document does not specify a version
number of this License, you may choose any version ever published (not
as a draft) by the Free Software Foundation. If the Document specifies
that a proxy can decide which future versions of this License can be
used, that proxy's public statement of acceptance of a version
permanently authorizes you to choose that version for the Document.

#### 11. RELICENSING

"Massive Multiauthor Collaboration Site" (or "MMC Site") means any
World Wide Web server that publishes copyrightable works and also
provides prominent facilities for anybody to edit those works. A
public wiki that anybody can edit is an example of such a server. A
"Massive Multiauthor Collaboration" (or "MMC") contained in the site
means any set of copyrightable works thus published on the MMC site.

"CC-BY-SA" means the Creative Commons Attribution-Share Alike 3.0
license published by Creative Commons Corporation, a not-for-profit
corporation with a principal place of business in San Francisco,
California, as well as future copyleft versions of that license
published by that same organization.

"Incorporate" means to publish or republish a Document, in whole or in
part, as part of another Document.

An MMC is "eligible for relicensing" if it is licensed under this
License, and if all works that were first published under this License
somewhere other than this MMC, and subsequently incorporated in whole
or in part into the MMC, (1) had no cover texts or invariant sections,
and (2) were thus incorporated prior to November 1, 2008.

The operator of an MMC Site may republish an MMC contained in the site
under CC-BY-SA on the same site at any time before August 1, 2009,
provided the MMC is eligible for relicensing.

