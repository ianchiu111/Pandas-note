### 代名詞說明
1. df 為 DataFrame 的名稱 → Ndf 為 New DataFrame
2. CN 為 Column Name → NCN 為 New Column Name
3. 

### 資料的匯入與檢查
- `df = pd.read_csv('file.csv')` → 將 csv file 匯入成 DataFrame
- `df.info()` `df.shape()` `df.columns` → 可以了解 DataFrame的相關資料
- `df.head(5)` `df.tail(10)` → 查看 DataFrame 的前5筆、最後10筆資料
- `df.CN.nunique()` → 查看 CN 欄位中，unique 值的數量
- ✴️`df.CN.value_counts()` → 計算 df 中 CN 各數值的出現次數
- `df.isnull().sum()` → 檢查 df 中 CN NULL 值的數量
- 

### 資料的處理
#### 處理 null 值
- ✴️`df['CN'].fillna(A, replace = True)` → 將 A 替代為 null 值
#### 處理時間資料
- 
#### GroupBy
- 

### Merge
- `Ndf = pd.merge(df1, df2, on = 'CN', how = {choice}`
  - {choice} : inner, outer, right, left

### Dummy Variables
```
1. `✴️需要再補一下筆記資料`
2. `概念與 ML 的 one-hot encoding 類似，主要將資料以 True False 來呈現`
```
- 
- 
