# Kaggle 練習：預測卡路里消耗 (Playground Series - S5E5)

這是一個在 Kaggle "Playground Series - Season 5, Episode 5" 比賽數據上進行的數據分析與機器學習練習專案，目標是預測運動時消耗的卡路里。

## 專案狀態

*   **目前進度：** 初步階段。
*   已完成數據載入、基本的前處理 (類別特徵 One-hot encoding)、以及使用線性回歸 (Linear Regression) 模型進行了初步的卡路里預測。
*   程式碼主要在 Jupyter Notebook (`predict-calorie-expenditure.ipynb`) 中。

## 數據來源

本專案使用的數據來自 Kaggle 的 **"Playground Series - Season 5, Episode 5"** 比賽。
您可以從以下連結訪問該比賽並下載數據：

*   **比賽主頁：** [Playground Series - Season 5, Episode 5](https://www.kaggle.com/competitions/playground-series-s5e5)
*   數據主要包含 `train.csv` (用於訓練模型) 和 `test.csv` (Kaggle 用於評分的測試數據)。

## 目前使用的技術

*   Python
*   Pandas (數據處理)
*   NumPy (數值計算)
*   Scikit-learn (線性回歸模型)
*   Jupyter Notebook (開發環境)

## 我的學習與挑戰 (初步)

*   **資料合併與前處理：** 練習了合併訓練集與測試集以進行一致的 One-hot encoding。
*   **基礎模型建立：** 成功使用 Scikit-learn 建立並訓練了一個線性回歸模型。
*   **後續目標：**
    *   進行更深入的探索性數據分析 (EDA) 並加入視覺化圖表。
    *   嘗試更複雜的特徵工程技巧。
    *   評估並比較不同機器學習模型的表現。
    *   更詳細地記錄分析過程和發現。

## 如何運行 (基本指引)

1.  從上述 Kaggle 比賽頁面下載 `train.csv` 和 `test.csv` 數據檔案。
2.  確保你的 Python 環境中安裝了 Pandas, NumPy, และ Scikit-learn。
3.  將數據檔案與 `predict-calorie-expenditure.ipynb` 放在同一目錄下，或修改 Notebook 中的數據讀取路徑。
4.  開啟並運行 Jupyter Notebook。

---
*這是一個正在進行中的學習專案，我將持續更新與改進。*