# Time-Series-Analysis-project
# Project Title:
Analysis and prediction of Microsoft_Stock.csv which contains stocks and credits of IT Form. Prediction of stocks in a future by three category in a "Open, High, Low"

# Problem statement:
This comprehensive dataset provides a detailed analysis of Microsoft Corporation's stock performance from 1986 to 2023. It encompasses various important parameters, including stock price, low price, *high * price, and trading volume, to provide a comprehensive overview of the company's market behavior throughout the years.
The dataset begins in 1986, marking the early years of Microsoft's presence in the stock market. As one of the pioneering companies in the technology industry, Microsoft's stock performance has been closely followed by investors, analysts, and enthusiasts alike. The dataset captures the fluctuations and trends in the stock market, reflecting the company's journey from its inception to its position as a global tech giant.

The stock price data offers a glimpse into the market valuation of Microsoft shares over time. By observing the daily closing prices, one can track the trajectory of the stock and identify key milestones in Microsoft's history. The dataset also includes the lowest and highest prices reached during each trading day, offering insight into the price range within which the stock fluctuated.
Trading volume data provides an additional dimension for understanding Microsoft's stock market activity. It highlights the level of investor interest and participation in buying and selling Microsoft shares during each trading day. Tracking trading volume can help identify periods of increased market activity or significant news events that influenced investor sentiment.

The dataset covers a span of several decades, enabling users to analyze long-term trends, market cycles, and historical patterns that have shaped Microsoft's stock performance. It can be used by researchers, investors, and analysts to conduct quantitative and qualitative studies, perform technical analyses, and gain insights into the dynamics of the technology industry and the broader market.
Please note that this dataset serves as a valuable historical resource and should be utilized alongside other relevant financial information and analysis to make informed decisions. The dataset captures Microsoft's stock performance up until 2023, ensuring that users have access to the latest available information.
# Discription:
The dataset provides the history daily price of microsoft stock depending on USD

# Visualizing Time Series

# Plot the time series data
plt.figure(figsize=(10,6))

plt.plot(data)

plt.xlabel("Data")

plt.ylabel("Value")

plt.title("Time series Analysis")

plt.show()

![image](https://github.com/Pavani1326/Time-Series-Analysis-project/assets/142418770/b7e80d15-4283-4478-a054-3b1f2be3c7b2)

# Perform seasonal decomposition

#The decomposition of time series is a statistical task that deconstructs a time series into several components, each representing one of the underlying categories of patterns.

decomposition = seasonal_decompose(data['Open'], model='additive', period=12)  # Assuming seasonality of 12 months

# Plot the decomposed components
trend=decomposition.trend

seasonal=decomposition.seasonal

residue=decomposition.resid # resid is used for residual


# plot the figure for visualization.
plt.figure(figsize=(12, 8))

plt.subplot(411)

plt.plot(data['Open'], label='Original')

plt.legend(loc='upper left')


# Visualize the trend .
plt.subplot(412)

plt.plot(data['Open'], label='Trend')

plt.legend(loc='upper left')


# visualioze the Seasonality
plt.subplot(413)

plt.plot(data['Open'], label='Seasonality')

plt.legend(loc='upper left')



# Visualize the Residuals.
plt.subplot(414)

plt.plot(data['Open'], label='Residuals')

plt.legend(loc='upper left')

plt.tight_layout()
plt.show()


![image](https://github.com/Pavani1326/Time-Series-Analysis-project/assets/142418770/c65d5f36-b27d-4253-987a-4158c70fe472)


# Perform seasonal decomposition

#The decomposition of time series is a statistical task that deconstructs a time series into several components, each representing one of the underlying categories of patterns.

decomposition = seasonal_decompose(data['High'], model='additive', period=12)  # Assuming seasonality of 12 months

# Plot the decomposed components
trend=decomposition.trend

seasonal=decomposition.seasonal

residue=decomposition.resid # resid is used for residual


# plot the figure for visualization.
plt.figure(figsize=(12, 8))

plt.subplot(411)

plt.plot(data['High'], label='Original')

plt.legend(loc='upper left')


# Visualize the trend .
plt.subplot(412)

plt.plot(data['High'], label='Trend')




# visualioze the Seasonality
plt.subplot(413)

plt.plot(data['High'], label='Seasonality')

plt.legend(loc='upper left')


# Visualize the Residuals.
plt.subplot(414)

plt.plot(data['High'], label='Residuals')

plt.legend(loc='upper left')

plt.tight_layout()

plt.show()

![image](https://github.com/Pavani1326/Time-Series-Analysis-project/assets/142418770/1315e6f2-a1be-4432-8e3f-a36163847954)

# Perform seasonal decomposition

#The decomposition of time series is a statistical task that deconstructs a time series into several components, each representing one of the underlying categories of patterns.

decomposition = seasonal_decompose(data['Low'], model='additive', period=12)  # Assuming seasonality of 12 months

# Plot the decomposed components
trend=decomposition.trend

seasonal=decomposition.seasonal

residue=decomposition.resid # resid is used for residual


# plot the figure for visualization.
plt.figure(figsize=(12, 8))

plt.subplot(411)

plt.plot(data['Low'], label='Original')

plt.legend(loc='upper left')


# Visualize the trend .
plt.subplot(412)

plt.plot(data['Low'], label='Trend')

plt.legend(loc='upper left')


# visualioze the Seasonality
plt.subplot(413)

plt.plot(data['Low'], label='Seasonality')

plt.legend(loc='upper left')


# Visualize the Residuals.
plt.subplot(414)

plt.plot(data['Low'], label='Residuals')

plt.legend(loc='upper left')

plt.tight_layout()

plt.show()

![image](https://github.com/Pavani1326/Time-Series-Analysis-project/assets/142418770/7cc4d1f6-976d-4d2d-822f-ee256f001995)

# Perform seasonal decomposition

#The decomposition of time series is a statistical task that deconstructs a time series into several components, each representing one of the underlying categories of patterns.

decomposition = seasonal_decompose(data['Close'], model='additive', period=12)  # Assuming seasonality of 12 months

# Plot the decomposed components
trend=decomposition.trend

seasonal=decomposition.seasonal

residue=decomposition.resid # resid is used for residual


# plot the figure for visualization.
plt.figure(figsize=(12, 8))

plt.subplot(411)

plt.plot(data['Close'], label='Original')

plt.legend(loc='upper left')


# Visualize the trend .
plt.subplot(412)

plt.plot(data['Close'], label='Trend

plt.legend(loc='upper left')


# visualioze the Seasonality
plt.subplot(413)

plt.plot(data['Close'], label='Seasonality')

plt.legend(loc='upper left')


# Visualize the Residuals.
plt.subplot(414)

plt.plot(data['Close'], label='Residuals')

plt.legend(loc='upper left')

plt.tight_layout()

plt.show()

![image](https://github.com/Pavani1326/Time-Series-Analysis-project/assets/142418770/e9529f48-648b-4e61-a4b0-6d4220baa775)

# Perform seasonal decomposition

#The decomposition of time series is a statistical task that deconstructs a time series into several components, each representing one of the underlying categories of patterns.

decomposition = seasonal_decompose(data['Volume'], model='additive', period=12)  # Assuming seasonality of 12 months

# Plot the decomposed components
trend=decomposition.trend

seasonal=decomposition.seasonal

residue=decomposition.resid # resid is used for residual


# plot the figure for visualization.
plt.figure(figsize=(12, 8))

plt.subplot(411)

plt.plot(data['Volume'], label='Original')

plt.legend(loc='upper left')


# Visualize the trend .
plt.subplot(412)

plt.plot(data['Volume'], label='Trend')

plt.legend(loc='upper left')


# visualioze the Seasonality
plt.subplot(413)

plt.plot(data['Volume'], label='Seasonality')

plt.legend(loc='upper left')


# Visualize the Residuals.
plt.subplot(414)

plt.plot(data['Volume'], label='Residuals')

plt.legend(loc='upper left')

plt.tight_layout()

plt.show()

![image](https://github.com/Pavani1326/Time-Series-Analysis-project/assets/142418770/712623db-0cac-45d6-a6bb-7cdcea99588e)



# Conclusion:
1.According to tha analysis of data this particular dataset we found that "Open", "High", "Low", "Close". As the columns in which tr in increasing manner but in the year 2020 -2021

2.Accoriding to the volume chart for particular this dataset year 2016-2017 give a little bit of to invesments in a stocks.after 2017 to upcomming year stocks will be fluctuated.

