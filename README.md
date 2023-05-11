# cis4400spring2023group0

import yfinance as yf
ticks = ["JPM", "BAC", "HSBC", "WFC", "RY", "TD", "C", "MUFG", "BMO", "UBS", "BNS", "SAN", "SMFG", "ING", "BBVA", "CM", "NWG", "BCS", "NU", "EWBC", "CS", "NTB", "SIVB", "SBNY"]
yf.download(ticks, start = "2020-03-01", end = "2023-03-31")["Adj Close"]

import matplotlib.pyplot as plt
%matplotlib inline

df.plot(figsize=(11,8))
plt.legend(bbox_to_anchor=(1.05,1),loc='upper left', borderaxespad=0)

df1 = pd.read_excel('/Users/ilona/Downloads/Financial ratios-qa.xlsx', sheet_name='JPM-Ratios')

df1.plot.bar(figsize=(20,14),x='Date', width=1)
plt.legend(bbox_to_anchor=(1.05,1),loc='upper left', borderaxespad=0)

df1.plot(figsize=(15,5), x='Date')
plt.legend(bbox_to_anchor=(1.05,1),loc='upper left', borderaxespad=0)

df2=df['JPM']

df2.plot(figsize=(15,5))
plt.legend(bbox_to_anchor=(1.05,1),loc='upper left', borderaxespad=0)

df3=df['SIVB']
df4=pd.read_excel('/Users/ilona/Downloads/Financial ratios-qa.xlsx', sheet_name='SIVB-Ratios')
df4.plot.bar(figsize=(20,10), x='Date', width=1)

plt.legend(bbox_to_anchor=(1.05,1),loc='upper left', borderaxespad=0)
df3.plot(figsize=(15,5))
plt.legend(bbox_to_anchor=(1.05,1),loc='upper left', borderaxespad=0)


