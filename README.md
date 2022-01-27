
![1__TntFs2nymL715CKoSOTAg](https://user-images.githubusercontent.com/26355917/151268386-7e16c093-6385-46f7-a1ee-eb406e7c64aa.jpeg)


# Portfolio Optimization of High-Value Tech Stocks

#### The purpose of this project is to analyze financial data, by calculating financial statistics to understand the individual performance of an asset, how groups of assets are related, and how to allocate investments across assets for optimal performance


![](https://media.giphy.com/media/VV39rWFojtqYD0UlHY/giphy.gif)

# Table of contents

- [Adjusted closing prices over time](#table-of-contents)
- [Daily Simple Rate of return](#installation)
- [Correlations between stocks](#usage)
- [MEAN-VARIANCE PORTFOLIO OPTIMIZATION](#development)
- [Efficient Frontier](#license)
- [Summary](#footer)

# Adjusted closing prices over time

Let’s first look at how the price of each stock has evolved over a year

![1_cmC_lkCJ6_b00piNkrxpPw](https://user-images.githubusercontent.com/26355917/151270238-a12afd6c-6279-4fad-8879-a68d9dc06495.png)

Amazon and Google’s stock price was relatively more expensive than others. But since Apple, Microsoft and Facebook are at the bottom, it is hard to see the movement of these three.

# Daily Simple Rate of return
By plotting daily returns, we can see the stock's volatility

![1_wPWPTNVqREUe9VM58Wc4vQ](https://user-images.githubusercontent.com/26355917/151270544-5205bc87-7814-4cc4-aba3-da16b81a8864.png)

Netflix has the highest returns in the first quarter and a couple of negative spikes indicating negative returns. From the above plot, we can roughly see that Amazon and Netflix looks like risky stock, and Google seems to be the most stable one among them.

# Correlations between stocks

It would be nice if every asset made large, consistent positive returns every period. If that were the case, we could invest all of our money in the asset with the highest expected return. But, the return of any given asset is unpredictable.
This is the place where you give instructions to developers on how to modify the code.

![1_rAfBUxr-0C2i0cAIZ0v7-w](https://user-images.githubusercontent.com/26355917/151270685-cde50106-c3ff-454a-a673-2b26369b14ed.png)

We quantify the risk of a portfolio, by calculating the variance of each asset, and the covariance between each asset and every other asset.

#### If two assets have a positive covariance, then they respond similarly to market forces. Assets with a negative covariance will not

The Covariance Matrix above indicates, None of the stocks are negatively correlated. Apple and Google are highly correlated, while Microsoft and Amazon exhibit the lowest correlation.

# MEAN-VARIANCE Portfolio Optimization

The fundamental goal of portfolio theory is to allocate investments between multiple assets optimally. Markowitz mean-variance optimization (MVO) is an approach to choose how to allocate money between multiple assets by considering the risk-return trade-off of asset combinations.


# Efficient Frontier
The efficient frontier is a set of portfolios that give us the highest return for the lowest possible risk.
This method returns a set of portfolios where:
* The expected return is greater than any other with the same or lesser risk
* The risk is less than any other with the same expected return

![1_FVv86gDfn5iY-Qv5S9sToA](https://user-images.githubusercontent.com/26355917/151271044-8fc530f3-ae8e-4488-bdc9-5bbb41cc4e0b.png)

The blue dots above indicate a set of portfolios, Using return_portfolios() function that accepts the expected returns and covariance matrix for a collection of assets, I generated random 5000 portfolios of random asset weights.

#### Given that our goal is to minimize volatility and maximize expected return, the portfolios that fall on the left-most edge are the best portfolios.

![1_2rkNGBxbTskhIlsABZwqUw](https://user-images.githubusercontent.com/26355917/151271110-ef964daa-b11a-4464-8168-5c600d61fa1e.png)

# Summary

The yellow line is on top falls on the portfolios that maximize the expected return at all risks, and minimize the risk at all expected returns. The vertical red lines in the figure above display the standard deviation of each asset.

As you can see from the above plot, the stocks with the least risk are Google at around 0.00225 and Microsoft at around 0.00175, these stocks are optimized for historical risk and return data.

Thank you for reading!
