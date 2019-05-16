# 2nd-ML100days
https://ai100-2.cupoy.com/

### Preprocessing  
D01: plt.plot()  
D02: read data  
D03: dataframe  
D04: pandas  
D05: data['column name'].hist()  
     data.loc[data['column name']<data['column name'].quantile(0.99)]['column name'].hist()  
D06: Outlier, Emprical CDF畫圖  
D07: NAs, 標準化Z, mode()  
D08: pd.cut() 分組, groupby  

### EDA 
D09: 正、負相關、scatter plot  
D10: .corr(), 在pd中使用.sort_values()代替.sort()  
D11: np.linspace(切成x區間), sns.barplot(px, py)長條圖  
D12: pd.qcut(資料集[欄位名稱], 切分點個數) ---> 等頻切分  
D13: pd.cut() + sns.barplot(px,py) --->離散x長條圖  
D14: 根據不同的 HOUSETYPE_MODE 對 AMT_CREDIT 繪製 Histogram  
     資料集.loc[(資料集['HOUSETYPE_MODE'] == unique_house_type[i]), 'y欄位'].hist() --->直方圖  
D15: 隨機np矩陣, sns.heatmap() , sns.PairGrid()  
D16: logistic regression  

### Feature Engineering
D17: 簡介FE  
D18: 不同feature type (int64, float64, object) 的 敘述統計資料  
D19: 查詢各欄位空缺值數量、觀察替換不同補缺方式(&不同特徵縮放方式)對特徵的影響  
D20: 調整或去除離群值
D21: 當離群資料比例太高，或平均值沒有代表性時(平均薪資)，可以考慮去除偏態  
去除偏態包含 : 對數去偏、方跟去偏以及分布去偏  
用 box-cox 分布去偏時，需注意λ介於 0 到 0.5 之間，並且要注意轉換前的數值不可小於等於0(否則須先用.loc處理)