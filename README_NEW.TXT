The original challenge was to create a shareable project that would assist in buying and selling decisions for different stocks; it would address items including how volatile is a stock, and how much of that volatility can be accounted for as a leading or lag indicator from social media. Also, discussed was what is the correlation and time-sensitivity of these and other factors?

As the team lost members, we had to refocus our efforts and examine just one stock to keep the volume of data to a reasonable level. In order to obtain the data and learn how best to refine it for our intended goals we used a small set of potential leading indicators of stock price performance.

We originally began looking for a free and easy means to obtain information to be able complete this task. The research led the group to discover the IEX platform ("Data provided by IEX Cloud”) which had most of the desired data sets. This is a paid for service, but is very timely in its information, therefore became the path we selected.

Stock prices have a great deal of interest, (The U.S. stock market is currently $34 trillion, compared to the rest of the world's $44 trillion in capital. The U.S. holds 43% of world market value, but it houses only 17% of the world's stocks.) there are several pricing models available that could cause a price performance impact. A list to show the potential different price models can be found at: https://en.wikipedia.org/wiki/Pricing_strategies. Stock prices are determined in the marketplace, where seller supply meets buyer demand. But have you ever wondered about what drives the stock market—that is, what factors affect a stock's price? Unfortunately, there is no clean equation that tells us exactly how a stock price will behave. That said, we do know a few things about the forces that move a stock up or down. These forces fall into three categories: fundamental factors, technical factors, and market sentiment. It is this last area were the team is focused to see if the data is available to find a leading indicator - market sentiment.

This project is not to teach the user any financial terms, formulas or theories; it is to determine if a leading indicator can be obtained from social media. Not all social media formats will be selected, just those that offer easy, fast and potentially free access to current trends.

Lastly, as we are all workings toward increasing our data science understanding, the data is being gathered and formatted to conduct the first of many potential analyses. Regression analysis: which will examine the influence / correlation of one or more independent parameter(s) on a dependent parameter(s). If a correlation is found, next would be predictive analyses, using predictive modelling, or potentially machine learning methods, to determine if social media is a leading or lagging indicator of stock price performance; and if so what are the constrains around such a model.

This project is a beta release from a DSCI511 Group Team Project; their data dictionary and methods for obtaining information used to try to detect leading indicator of price performance.

Installation
There is no current version of the package available for installation.

Importing Database
There is no current version of the database available for importing.

Requirements
Below are the specifications which this project was built. We appreciate feedback on other platforms

System Requirements
This project was developed with the following specifications: Windows 10 Python 3.7

License & Support
This project, when released, will be under an MIT-style license.

Acknowledgements
The project is built by 3 Drexel MSDS21 first year students that include: Justin Goheen, Kevin Fitzpatrick, and Joe Larson.






Full description of dataset outputs are below:

File: balance_sheet.csv
Description: quarterly balance sheet
Size: 4 rows by 28 columns
Format: csv with the following columns and example data as below:
{'accountsPayable': 35794000000,
 'capitalSurplus': 31817000000,
 'commonStock': 495000000,
 'currentAssets': 79054000000,
 'currentCash': 23557000000,
 'currentLongTermDebt': 12219000000,
 'goodwill': 14734000000,
 'intangibleAssets': 0,
 'inventory': 18766000000,
 'longTermDebt': 59530000000,
 'longTermInvestments': 568000000,
 'minorityInterest': 0,
 'netTangibleAssets': 41774000000,
 'otherAssets': 13967000000,
 'otherCurrentAssets': nan,
 'otherCurrentLiabilities': 21281000000,
 'otherLiabilities': 10925000000,
 'propertyPlantEquipment': 90776000000,
 'receivables': 16585000000,
 'reportDate': '2019-09-30',
 'retainedEarnings': 27952000000,
 'shareholderEquity': 56508000000,
 'shortTermInvestments': 20146000000,
 'ticker': 'amzn',
 'totalAssets': 199099000000,
 'totalCurrentLiabilities': 72136000000,
 'totalLiabilities': 142591000000,
 'treasuryStock': 1837000000}



File: news_last30.csv
Description: news articles, last 30 items
Size: 30 rows by 10 columns
Format: csv with the following columns and example data as below:
{'datetime': 1575301175000,
 'hasPaywall': False,
 'headline': 'Tech giants set to spend £25bn on advertising this year',
 'image': 'https://cloud.iexapis.com/v1/news/image/d9853ea8-652c-4277-a2ce-79418baff2b9',
 'lang': 'en',
 'related': 'AMZN',
 'source': 'City AM',
 'summary': 'Eight tech titans including Google, Facebook and Amazon dominate '
            'the global advertising industry and will spend £25bn on '
            'advertising this […] The post Tech giants set to spend £25bn on '
            'advertising this year appeared first on CityAM .',
 'ticker': 'amzn',
 'url': 'https://cloud.iexapis.com/v1/news/article/d9853ea8-652c-4277-a2ce-79418baff2b9'}



File: options_201912.csv
Description: options that expire on YYYMM above
Size: 1458 rows by 15 columns
Format: csv with the following columns and example data as below:
{'ask': 41.900002,
 'bid': 32.450001,
 'closingPrice': 37.349998,
 'contractSize': 100,
 'expirationDate': 20191220,
 'id': 'AMZN20191220C01795000',
 'isAdjusted': False,
 'lastUpdated': '2019-11-29',
 'openInterest': 239,
 'side': 'call',
 'strikePrice': 1795.0,
 'symbol': 'AMZN',
 'ticker': 'amzn',
 'type': 'equity',
 'volume': 52}



File: earnings.csv
Description: quarterly earnings
Size: 4 rows by 11 columns
Format: csv with the following columns and example data as below:
{'EPSReportDate': '2019-10-24',
 'EPSSurpriseDollar': -0.38,
 'actualEPS': 4.23,
 'announceTime': 'AMC',
 'consensusEPS': 4.61,
 'fiscalEndDate': '2019-09-30',
 'fiscalPeriod': 'Q3 2019',
 'numberOfEstimates': 43,
 'ticker': 'amzn',
 'yearAgo': 5.75,
 'yearAgoChangePercent': -0.2643}



File: options_202007.csv
Description: options that expire on YYYMM above
Size: 176 rows by 15 columns
Format: csv with the following columns and example data as below:
{'ask': 235.55000299999998,
 'bid': 219.75,
 'closingPrice': 0.0,
 'contractSize': 100,
 'expirationDate': 20200717,
 'id': 'AMZN20200717C01675000',
 'isAdjusted': False,
 'lastUpdated': '2019-11-29',
 'openInterest': 0,
 'side': 'call',
 'strikePrice': 1675,
 'symbol': 'AMZN',
 'ticker': 'amzn',
 'type': 'equity',
 'volume': 0}



File: social_sentiment.csv
Description: social sentiment from StockTwits
Size: 365 rows by 6 columns
Format: csv with the following columns and example data as below:
{'date': '2019-12-01',
 'negative': 0.15,
 'positive': 0.85,
 'sentiment': 0.20602256097560973,
 'ticker': 'amzn',
 'totalScores': 164}



File: options_202002.csv
Description: options that expire on YYYMM above
Size: 242 rows by 15 columns
Format: csv with the following columns and example data as below:
{'ask': 73.599998,
 'bid': 65.0,
 'closingPrice': 70.949997,
 'contractSize': 100,
 'expirationDate': 20200221,
 'id': 'AMZN20200221C01840000',
 'isAdjusted': False,
 'lastUpdated': '2019-11-29',
 'openInterest': 2049,
 'side': 'call',
 'strikePrice': 1840,
 'symbol': 'AMZN',
 'ticker': 'amzn',
 'type': 'equity',
 'volume': 35}



File: options_201911.csv
Description: options that expire on YYYMM above
Size: 534 rows by 15 columns
Format: csv with the following columns and example data as below:
{'ask': 201.649994,
 'bid': 185.800003,
 'closingPrice': 129.149994,
 'contractSize': 100,
 'expirationDate': 20191129,
 'id': 'AMZN20191129C01610000',
 'isAdjusted': False,
 'lastUpdated': '2019-11-29',
 'openInterest': 3,
 'side': 'call',
 'strikePrice': 1610.0,
 'symbol': 'AMZN',
 'ticker': 'amzn',
 'type': 'equity',
 'volume': 0}



File: options_202004.csv
Description: options that expire on YYYMM above
Size: 184 rows by 15 columns
Format: csv with the following columns and example data as below:
{'ask': 145.800003,
 'bid': 130.350006,
 'closingPrice': 141.399994,
 'contractSize': 100,
 'expirationDate': 20200417,
 'id': 'AMZN20200417C01760000',
 'isAdjusted': False,
 'lastUpdated': '2019-11-29',
 'openInterest': 234,
 'side': 'call',
 'strikePrice': 1760,
 'symbol': 'AMZN',
 'ticker': 'amzn',
 'type': 'equity',
 'volume': 0}



File: income_statement.csv
Description: quarterly income statement
Size: 4 rows by 17 columns
Format: csv with the following columns and example data as below:
{'costOfRevenue': 41302000000,
 'ebit': 3212000000,
 'grossProfit': 28679000000,
 'incomeTax': 494000000,
 'interestIncome': 396000000,
 'minorityInterest': 0,
 'netIncome': 2134000000,
 'netIncomeBasic': 2134000000,
 'operatingExpense': 66769000000,
 'operatingIncome': 3212000000,
 'otherIncomeExpenseNet': -580000000,
 'pretaxIncome': 2632000000,
 'reportDate': '2019-09-30',
 'researchAndDevelopment': 9200000000,
 'sellingGeneralAndAdmin': 16267000000,
 'ticker': 'amzn',
 'totalRevenue': 69981000000}



File: peers.csv
Description: list of company peers
Size: 8 rows by 2 columns
Format: csv with the following columns and example data as below:
{'0': 'OSTK', 'ticker': 'amzn'}



File: historical_prices.csv
Description: historical adjusted/unadjusted open, high, low, close, volume data for the past year with change/change percent
Size: 251 rows by 16 columns
Format: csv with the following columns and example data as below:
{'change': 0.0,
 'changeOverTime': 0.0,
 'changePercent': 0.0,
 'close': 1690.17,
 'date': '2018-11-30',
 'high': 1696.0,
 'label': 'Nov 30, 18',
 'low': 1666.5,
 'open': 1679.5,
 'ticker': 'amzn',
 'uClose': 1690.17,
 'uHigh': 1696.0,
 'uLow': 1666.5,
 'uOpen': 1679.5,
 'uVolume': 5761761,
 'volume': 5761761}



File: price_target.csv
Description: aggregate price targets
Size: 1 rows by 7 columns
Format: csv with the following columns and example data as below:
{'numberOfAnalysts': 45,
 'priceTargetAverage': 2178.08,
 'priceTargetHigh': 2573.4,
 'priceTargetLow': 1850,
 'symbol': 'AMZN',
 'ticker': 'amzn',
 'updatedDate': '2019-11-25'}



File: financials.csv
Description: quarterly financials
Size: 4 rows by 22 columns
Format: csv with the following columns and example data as below:
{'cashChange': 589000000,
 'cashFlow': 7892000000,
 'costOfRevenue': 41302000000,
 'currentAssets': 79054000000,
 'currentCash': 23557000000,
 'currentDebt': 15061000000,
 'grossProfit': 28679000000,
 'longTermDebt': 59530000000,
 'netIncome': 2134000000,
 'operatingExpense': 66769000000,
 'operatingIncome': 3212000000,
 'operatingRevenue': 69981000000,
 'reportDate': '2019-09-30',
 'researchAndDevelopment': 9200000000,
 'shareholderEquity': 56508000000,
 'shortTermDebt': 15061000000,
 'ticker': 'amzn',
 'totalAssets': 199099000000,
 'totalCash': 43703000000,
 'totalDebt': 74591000000,
 'totalLiabilities': 142591000000,
 'totalRevenue': 69981000000}



File: insider_transactions.csv
Description: list of insider transactions
Size: 559 rows by 9 columns
Format: csv with the following columns and example data as below:
{'directIndirect': 'D',
 'effectiveDate': 1574294400000,
 'fullName': 'Jeffrey P. Bezos',
 'reportedTitle': 'Chairman, CEO and President; Director',
 'ticker': 'amzn',
 'tranCode': 'G',
 'tranPrice': 0.0,
 'tranShares': -56702,
 'tranValue': 0.0}



File: options_202009.csv
Description: options that expire on YYYMM above
Size: 146 rows by 15 columns
Format: csv with the following columns and example data as below:
{'ask': 280.200012,
 'bid': 265.899994,
 'closingPrice': 268.149994,
 'contractSize': 100,
 'expirationDate': 20200918,
 'id': 'AMZN20200918C01640000',
 'isAdjusted': False,
 'lastUpdated': '2019-11-29',
 'openInterest': 14,
 'side': 'call',
 'strikePrice': 1640,
 'symbol': 'AMZN',
 'ticker': 'amzn',
 'type': 'equity',
 'volume': 0}



File: options_202101.csv
Description: options that expire on YYYMM above
Size: 362 rows by 15 columns
Format: csv with the following columns and example data as below:
{'ask': 159.649994,
 'bid': 144.800003,
 'closingPrice': 161.149994,
 'contractSize': 100,
 'expirationDate': 20210115,
 'id': 'AMZN20210115C01960000',
 'isAdjusted': False,
 'lastUpdated': '2019-11-29',
 'openInterest': 58,
 'side': 'call',
 'strikePrice': 1960,
 'symbol': 'AMZN',
 'ticker': 'amzn',
 'type': 'equity',
 'volume': 0}



File: options_202106.csv
Description: options that expire on YYYMM above
Size: 138 rows by 15 columns
Format: csv with the following columns and example data as below:
{'ask': 258.0,
 'bid': 238.0,
 'closingPrice': 213.57000699999998,
 'contractSize': 100,
 'expirationDate': 20210618,
 'id': 'AMZN20210618C01840000',
 'isAdjusted': False,
 'lastUpdated': '2019-11-29',
 'openInterest': 101,
 'side': 'call',
 'strikePrice': 1840,
 'symbol': 'AMZN',
 'ticker': 'amzn',
 'type': 'equity',
 'volume': 0}



File: options_202003.csv
Description: options that expire on YYYMM above
Size: 302 rows by 15 columns
Format: csv with the following columns and example data as below:
{'ask': 165.149994,
 'bid': 150.0,
 'closingPrice': 167.440002,
 'contractSize': 100,
 'expirationDate': 20200320,
 'id': 'AMZN20200320C01710000',
 'isAdjusted': False,
 'lastUpdated': '2019-11-29',
 'openInterest': 73,
 'side': 'call',
 'strikePrice': 1710,
 'symbol': 'AMZN',
 'ticker': 'amzn',
 'type': 'equity',
 'volume': 0}



File: recommendation_trends.csv
Description: aggregate analyst recommendations
Size: 8 rows by 11 columns
Format: csv with the following columns and example data as below:
{'consensusEndDate': nan,
 'consensusStartDate': 1574640000000,
 'corporateActionsAppliedDate': 936230400000,
 'ratingBuy': 43,
 'ratingHold': 2,
 'ratingNone': 0,
 'ratingOverweight': 4,
 'ratingScaleMark': 1.081633,
 'ratingSell': 0,
 'ratingUnderweight': 0,
 'ticker': 'amzn'}



File: cash_flow.csv
Description: quarterly cash flow statements
Size: 4 rows by 17 columns
Format: csv with the following columns and example data as below:
{'capitalExpenditures': -4697000000,
 'cashChange': 589000000,
 'cashFlow': 7892000000,
 'cashFlowFinancing': -1960000000,
 'changesInInventories': -381000000,
 'changesInReceivables': -156000000,
 'depreciation': 5563000000,
 'dividendsPaid': nan,
 'exchangeRateEffect': -270000000,
 'investingActivityOther': nan,
 'investments': -1289000000,
 'netBorrowings': -1960000000,
 'netIncome': 2134000000,
 'otherFinancingCashFlows': nan,
 'reportDate': '2019-09-30',
 'ticker': 'amzn',
 'totalInvestingCashFlows': -5073000000}



File: key_stats.csv
Description: key statistics
Size: 1 rows by 31 columns
Format: csv with the following columns and example data as below:
{'avg10Volume': 2862254.2,
 'avg30Volume': 2937443.93,
 'beta': 1.4829700814250064,
 'companyName': 'Amazon.com, Inc.',
 'day200MovingAvg': 1813.41,
 'day30ChangePercent': 0.0246,
 'day50MovingAvg': 1761.6,
 'day5ChangePercent': 0.0316,
 'dividendYield': nan,
 'employees': 647500,
 'exDividendDate': nan,
 'float': 437737188.112,
 'marketcap': 892831237600,
 'maxChangePercent': 69.509,
 'month1ChangePercent': 0.0216,
 'month3ChangePercent': 0.0081,
 'month6ChangePercent': -0.0101,
 'nextDividendDate': nan,
 'nextEarningsDate': '2020-02-01',
 'peRatio': 76.58,
 'sharesOutstanding': 495797000,
 'ticker': 'amzn',
 'ttmDividendRate': nan,
 'ttmEPS': 23.0682,
 'week52change': 0.065455,
 'week52high': 2035.8,
 'week52low': 1307,
 'year1ChangePercent': 0.076,
 'year2ChangePercent': 0.5507,
 'year5ChangePercent': 4.5239,
 'ytdChangePercent': 0.17}



File: options_202201.csv
Description: options that expire on YYYMM above
Size: 182 rows by 15 columns
Format: csv with the following columns and example data as below:
{'ask': 291.700012,
 'bid': 271.700012,
 'closingPrice': 246.229996,
 'contractSize': 100,
 'expirationDate': 20220121,
 'id': 'AMZN20220121C01885000',
 'isAdjusted': False,
 'lastUpdated': '2019-11-29',
 'openInterest': 17,
 'side': 'call',
 'strikePrice': 1885,
 'symbol': 'AMZN',
 'ticker': 'amzn',
 'type': 'equity',
 'volume': 0}



File: options_202006.csv
Description: options that expire on YYYMM above
Size: 236 rows by 15 columns
Format: csv with the following columns and example data as below:
{'ask': 246.149994,
 'bid': 227.44999700000002,
 'closingPrice': 253.75,
 'contractSize': 100,
 'expirationDate': 20200619,
 'id': 'AMZN20200619C01650000',
 'isAdjusted': False,
 'lastUpdated': '2019-11-29',
 'openInterest': 168,
 'side': 'call',
 'strikePrice': 1650,
 'symbol': 'AMZN',
 'ticker': 'amzn',
 'type': 'equity',
 'volume': 0}



File: options_202001.csv
Description: options that expire on YYYMM above
Size: 994 rows by 15 columns
Format: csv with the following columns and example data as below:
{'ask': 116.949997,
 'bid': 101.300003,
 'closingPrice': 113.449997,
 'contractSize': 100,
 'expirationDate': 20200117,
 'id': 'AMZN20200117C01720000',
 'isAdjusted': False,
 'lastUpdated': '2019-11-29',
 'openInterest': 713,
 'side': 'call',
 'strikePrice': 1720.0,
 'symbol': 'AMZN',
 'ticker': 'amzn',
 'type': 'equity',
 'volume': 4}



File: estimates.csv
Description: upcoming earnings estimates
Size: 1 rows by 7 columns
Format: csv with the following columns and example data as below:
{'announceTime': 'AMC',
 'consensusEPS': 4.09,
 'fiscalEndDate': '2019-12-31',
 'fiscalPeriod': 'Q4 2019',
 'numberOfEstimates': 45,
 'reportDate': '2020-02-01',
 'ticker': 'amzn'}



File: company_profile.csv
Description: company profile
Size: 2 rows by 20 columns
Format: csv with the following columns and example data as below:
{'CEO': 'Jeffrey P. Bezos',
 'address': '410 Terry Avenue North',
 'address2': nan,
 'city': 'Seattle',
 'companyName': 'Amazon.com, Inc.',
 'country': 'US',
 'description': 'Amazon.com, Inc. engages in the provision of online retail '
                'shopping services. It operates through the following business '
                'segments: North America, International, and Amazon Web '
                'Services (AWS). The North America segment includes retail '
                'sales of consumer products and subscriptions through North '
                'America-focused websites such as www.amazon.com and '
                'www.amazon.ca. The International segment offers retail sales '
                'of consumer products and subscriptions through '
                'internationally-focused websites. The Amazon Web Services '
                'segment involves in the global sales of compute, storage, '
                'database, and AWS service offerings for start-ups, '
                'enterprises, government agencies, and academic institutions. '
                'The company was founded by Jeffrey P. Bezos in July 1994 and '
                'is headquartered in Seattle, WA.',
 'employees': 647500,
 'exchange': 'NASDAQ',
 'industry': 'Internet Retail',
 'issueType': 'cs',
 'phone': '1.206.266.1000',
 'primarySicCode': 5961,
 'sector': 'Retail Trade',
 'securityName': 'Amazon.com, Inc.',
 'state': 'WA',
 'symbol': 'AMZN',
 'tags': 'Retail Trade',
 'website': 'http://www.amazon.com',
 'zip': '98109-5210'}
