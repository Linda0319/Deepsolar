# Deepsolar-Project
### 專案詳細內容請看我的三篇 medium
- [（上）資料來源跟分析目的](https://linda-lin.medium.com/我的第一個數據專案-76e63a67c1d6)
- [（中）資料觀察跟資料前處理](https://linda-lin.medium.com/我的-c34c8669f5a7)
- [（下）建模預測及決策分析](https://medium.com/p/597254638fa/edit)

### code 主要分為「預測_Predict」、「決策_Decision」
- 目標 Y：給太陽能開發公司使用，家戶太陽能佈署密度（total_panel_area_residential），找出與太陽能部署密度相關的社會經濟地理等因素
- 預測使用：LR、DNN、Extra trees、XGBoost
- 特徵工程使用： SFS、LASSO、PCA、Feature Importance
- 特徵工程後：Extra trees、XGBoost 在 10% 差距門檻下都有達到 93% 預測正確率
- 決策使用：CART 畫決策樹，從決策樹發現最重要因子：經度（美西>美東）
  - 美西
  - 信度：7635/22590=33.8%，效度：7533/7635=98.7%
  - 使用煤比率（少） → 人口密度（高）→ 財產稅激勵措施年數（久） → 地區總面積（大） → 自住比率（高）
  - 美東
  - 信度：1529/22590=6.8%，效度：1467/1529=95.9%
  - 工業用電價格（高） → 地區總面積（大） →人口密度（高）→ 房價中位數（高） → 2012年投民主黨比率（高）

### 專案及資料來源介紹：
- 資料集來源： [Deep Solar Dataset — Kaggle](https://www.kaggle.com/tunguz/deep-solar-dataset)
- 資料集分析參考：[Samuel Kolpinizki Project — GitHub](https://github.com/sammykol83/UdacityDataScienceNanoDegree/tree/master/Project%20-%20Write%20A%20Data-Science%20Blog)
- 史丹佛太陽能佈署：[Stanford project called “Deep Solar” — Joule article](https://www.sciencedirect.com/science/article/pii/S2542435118305701)

### 特別感謝
- 財團法人自強工業科學基金會
- 黃登揚 黃老師
- 蔡智勇 蔡老師
- 陳松林 陳老師
