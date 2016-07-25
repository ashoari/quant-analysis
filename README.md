# Table of Contents

1. [Project Definition] (README.md#Project Definition)
2. [Description of Data Source] (README.md#Description of Data Source)
3. [Repository Structure] (README.md#Repository Structure)
4. [Investigation] (README.md#Investigation)

This file explains the high level description of my project. 

##Project Definition
[Back to Table of Contents] (README.md#table-of-contents)
My project is a stock correlator project. It seeks to correlate the historical price change of a stock with the price of a commodity such as oil. For example, the price of crude oil is dependent on global economy factors in addition to production rate but traders know that the price of oil producing companies are affected by the price of crude oil. So when oil price increases we expect the price of giant oil producing to climb and vice versa. My project has two phases and can be extended to extract more useful information.

1-	The first phase compare the correlation of any individual stock (positive or negative correlation) and compare it with average correlation of oil and gas companies with oil to identify new opportunities especially identify which companies are affected in the negative direction with the price of oil. For example I am interested to examine the price of cargo transportation companies, utility companies and airlines because they are suppose to benefit from the low oil price (their sales price do not generally depends on the crude oil but their expenses are)

2-	One easy to implement correlation indicator is to visualize if an oil company stock increases and decreaeses along with oil price (i.e. the sign of the changes having values between +1,-1) from previous day and we compare this vector with that of the crude oil in a single plot. We have done this at the beginning of the Jupyter notebook
 
3-	In the second phase, we consider the price of individual companies in the oil and gas sector and see how their correlation compares with other companies and the average correlation of major oil and gas producing companies. We use a rolling correlation and track it over time. If that specific company does not follow even the average correlation that could be an indication that the company has some fundamental internal problem. For example petrobras (PBR) is now under security investigation for alleged bribery accusation and its price fluctuated sporadically and not follow the trend of crude oil closely. 
 
##Description of Data Source
[Back to Table of Contents] (README.md#table-of-contents)

The trade data for my project is available through following API:
https://www.quandl.com/

Link to the description of the public data is as follows:
https://www.quandl.com/blog/getting-started-with-the-quandl-api
https://github.com/quandl/quandl-python/blob/master/FOR_ANALYSTS.md


##Repository Structure
[Back to Table of Contents] (README.md#table-of-contents)
My code has been developed with Python 3.5 in a Jupyter notebook which also keeps all the investigatory plots. All the libraries used are imported at the beginning. The main file used to evaluate the feasibility of the project is Arian_correlationv2.ipynb. The files under ./Others folder is borrowed from another project (parent repository) for possible future extension but has not been used in the evaluation so far.  

	├── README.md 
	├── Arian_correlationv2.ipynb
	├──  Arian_correlation.ipynb 
	│  	
	└── Others
	 	   ├── 
	                └── 
        		│   ├── 
        		│   │   └── 

        


##Investigation
[Back to Table of Contents] (README.md#table-of-contents)

The last plot in 'Arian_correlationv2.ipynb' shows the rolling correlation of the stock price of 'Exxon' , 'Petrobaras' and the average correlation of major oil producing companies with the price of Crude oil. As can be seen 'Exxon' lost its dependency with average correlation from 01 March till 08 March.

