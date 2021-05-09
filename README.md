# stock-price-visualization 
import pandas as pd
from investpy import Stock
from datetime import datetime
import matplotlib.pyplot as plt
from investpy import get_historical_data
start = datetime(2010, 1, 1)
end = datetime(2020, 12, 31)
df = get_historical_data("SBIN", start, end, output_format='pandas')
plt.figure(figsize=(10,10))
plt.plot(df.index, df['close'])
plt.xlabel("date")
plt.ylabel("INR")
plt.title("SBIN Stock Price 1/1/2010 - 31/12/2020")



https://aditya211998.github.io/stock-price-visualization/ Tap here for quick review of my code
