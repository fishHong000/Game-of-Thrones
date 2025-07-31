# Game-of-Thrones

本次作業為預測角色是否死亡

資料集在以下網址：https://www.kaggle.com/mylesoneill/game-of-thrones

其中第二份資料的 character-deaths.csv

其中三個欄位 Death Year , Book of Death , Death Chapter 取其中一個欄位當預測目標用即可

請將欄位的空值轉成 0 (代表存活)，有數值的轉成 1 (代表死亡)


有開設 Kaggle 非正式競賽供同學評估模型使用，Kaggle 分數不會列入作業成績

HW1 Kaggle 網址：https://www.kaggle.com/t/94d5024975a943f0126e8a26060451a4


作業流程 & 要求：

※請使用python處理，可以使用任何套件
1.       將資料讀取進來(可用pandas套件)

2.       資料前處理

         2.1      把空值以0替代

         2.2      Death Year , Book of Death , Death Chapter 三者取一個，將有數值的轉成 1

         2.3      將 Allegiances 轉成 dummy 特徵 (底下有幾種分類就會變成幾個特徵，值是 0 或 1，本來的資料集就會再增加約 20 種特徵)

         2.4      亂數拆成訓練集 (75%) 與測試集 (25%) 

3.       使用 scikit-learn 的 DecisionTreeClassifier 進行預測 (可以先試著將 網頁範例 (iris) 跑出來在使用這次作業的資料集)

4.       做出 Confusion Matrix，並計算 Precision, Recall, Accuracy (提示：可使用 sklearn.metrics)

5.       產出決策樹的圖

