# Predict-NBA-2021MVP
**我們利用過去20年來獲得前十名MVP投票數球員的資料作為訓練資料集，並利用本季熱門球員的資料做為測試集，以預測本季MVP。**

* 利用Selenium搭配BeautifulSoupq爬取我們需要的資料並解析頁面。
* 資料來源：https://www.basketball-reference.com/
  * 這個網站提供非常完整的NBA資料，有各個球員、球隊的戰績，數據非常清楚、詳細。
1. 訓練資料集：我們爬取過去20年的MVP球員資料。
 <img width="827" alt="截圖 2021-06-21 上午10 53 54" src="https://user-images.githubusercontent.com/84361729/122701042-fac72700-d27e-11eb-8b8e-4a2bc8cc8544.png">

2. 除了20年的MVP資料，也爬取20年間，每年獲得前10名的球員資料，也就是Rank1~Rank10的球員戰績。（以2020年MVP排名為例）
 <img width="931" alt="截圖 2021-06-21 上午10 54 42" src="https://user-images.githubusercontent.com/84361729/122701105-17635f00-d27f-11eb-9542-7e4e2b289a21.png">

3. 總共200筆資料成為訓練資料集(NBA_train_data.csv)。

4. 測試資料集：爬取熱門球員本季戰績作為預測數據(NBA_test_data.csv)。
 <img width="918" alt="截圖 2021-06-21 下午9 15 05" src="https://user-images.githubusercontent.com/84361729/122767989-c29f0300-d2d5-11eb-816a-151183b1a42b.png">

5. 訓練模型：


* 參考：https://www.kaggle.com/ishaanupadhyay/mvp-prediction-random-forest-and-others
