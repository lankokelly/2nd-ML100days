# 2nd-ML100days

## Preprocessing  
D1: plt.plot()  
D2: read data  
D3: dataframe  
D4: pandas  
D5: data['column name'].hist()  
    data.loc[data['column name']<data['column name'].quantile(0.99)]['column name'].hist()  
D6: Outlier, Emprical CDF畫圖  
D7: NAs, 標準化Z, mode()  
D8: pd.cut() 分組, groupby  
D9: 正、負相關、scatter plot  
D10: .corr(), 在pd中使用.sort_values()代替.sort()  
D11: np.linspace(切成x區間), seaborn繪圖套件, sns.barplot(px, py)長條圖  
D12: pd.qcut(資料集[欄位名稱], 切分點個數) ---> 等頻切分  
D13: pd.cut() + sns.barplot(px,py) --->離散x長條圖  
D14: 根據不同的 HOUSETYPE_MODE 對 AMT_CREDIT 繪製 Histogram  
資料集.loc[(資料集['HOUSETYPE_MODE'] == unique_house_type[i]), 'y欄位'].hist() --->直方圖  