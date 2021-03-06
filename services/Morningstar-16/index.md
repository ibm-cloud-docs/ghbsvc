---

copyright:

  years:  2017

lastupdated: "2017-10-18"

---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen:.screen}
{:codeblock:.codeblock}
{:pre: .pre}

<!--Please delete out content examples and coding that you are not using for your service. -->

# Morningstar Portfolio Statistics API
{: #gettingstarted}
<!-- Provide an appropriate ID above -->

<!-- Short description: REQUIRED
The short description section should include one to two sentences describing why a developer would want to use your service in an app. This should be conversational style. For search engine optimization, include the service long name and "Bluemix". Keep the {: shortdesc} after the first paragraph so that the framework renders it properly.

Examples: -->


Data on our wide ranging investment database can strengthen activities that range from conducting research and financial modeling, to developing new products, creating investor-friendly communication materials, and delivering industry-standard statistics.  The Morningstar Data API's provide a flexible, easy to implement access mechanism to allow you to access the data to support your business objectives.
{:shortdesc}


## Overview

The Morningstar Portfolios Statistics API will provide an aggregated view of a Portfolio's individual securities.  Common data elements withing this API include P/E, P/B and the average market cap of the portfolio.


## Getting Started

In order to access data via the URL, there are 3 pieces of information that need to be passed to Morningstar.

1. Identifier Type
2. Identifier
3. Authentication Code

### Identifier Type

The table below indicates the identifiers that can be used to accessed Managed Investment data via the API. 

| Identifier Name       | Definition           | Parameter Name  |
| ------------- |:-------------:| -----:|
| Morningstar® SecId      | The Morningstar® SecId is a 10 character alpha numeric code. Each individual investment is assigned a SecId when it is added to the Morningstar® Database. | mstarid |
| Ticker    | An identifier assigned by an Exchange for each individual investment.     |   ticker |


### Authentication Code

The final piece of the URL will be an authentication token that is added to the end of the URL.  Morningstar will provide details on how to create and refresh access codes.




## Accessing the  Data

#### Step 1
Select which identifier type you will use to access the information and enter the parameter name into the URL.  In this example, the ticker parameter has been added to the URL:

<http://api.morningstar.com/v2/service/mf/PortfolioStatistics/<B>ticker</B>/?accesscode={accesscode}

#### Step 2
Enter the ticker symbol that you want to retrieve into the URL.  The example below is ABCDX.

http://api.morningstar.com/v2/service/mf/PortfolioStatistics/ticker/<B>ABCDX</B>?accesscode={accesscode}

#### Step 3
Finally, enter your authentication code that was generated by Morningstar to retrieve the data.

<http://api.morningstar.com/v2/service/mf/PortfolioStatistics/ticker/ABCDX?accesscode=<B>yyhdjfhergegeifjfjhsfdsf765</B>



## Additional Details

In order to access Morningstar APIs or learn about other data available, please submit a request to the link shown below and a representative will reach out to discuss.

(https://developer.morningstar.com/contact-us)

## About Morningstar, Inc

Morningstar, Inc. is a leading provider of independent investment research in North America, Europe, Australia, and Asia. The company offers an extensive line of products and services for individual investors, financial advisors, asset managers, retirement plan providers and sponsors, and institutional investors in the private capital markets. Morningstar provides data and research insights on a wide range of investment offerings, including managed investment products, publicly listed companies, private capital markets, and real-time global market data. Morningstar also offers investment management services through its investment advisory subsidiaries, with more than $195 billion in assets under advisement and management as of Dec. 31, 2017. The company has operations in 27 countries.

<!-- Related links section: still REQUIRED but moved to toc file (in your same folder).  Edit there.
-->