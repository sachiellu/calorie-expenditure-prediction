# Kaggle 練習：預測卡路里消耗 (Playground Series - S5E5)

這是一個在 Kaggle "Playground Series - Season 5, Episode 5" 比賽數據上進行的數據分析與機器學習練習專案，目標是預測運動時消耗的卡路里。

## 專案目標

利用已知的運動相關數據 (如年齡、身高、體重、心律、運動時長、性別)來學習模型，預測「Calories_Burned(消耗的卡路里)」這個目標變數。

## 專案狀態

*   **目前進度：** 初步階段。
*   完成數據載入、基本前處理 (類別特徵 One-hot encoding)、以及使用線性回歸 (Linear Regression) 模型進行了初步的卡路里預測。
*   程式碼主要在 Jupyter Notebook (`predict-calorie-expenditure.ipynb`) 中。

## 數據來源

本專案使用的數據來自 Kaggle 的 **"Playground Series - Season 5, Episode 5"** 比賽。
您可以從以下連結訪問該比賽並下載數據：

*   **比賽主頁：** [Playground Series - Season 5, Episode 5](https://www.kaggle.com/competitions/playground-series-s5e5)
*   數據主要包含 `train.csv` (用於訓練模型) 和 `test.csv` (Kaggle 用於評分的測試數據)。


## 我的分析與學習過程

### 初期探索與模型選擇
在專案初期，我先確立目標，利用提供的數據特徵預測卡路里消耗量。

在模型方面，我選擇用**線性回歸(Linear Regression)**開始，作為基礎模型。目標先確認數據處理與模型訓練流程跑通並且可以正確讀取輸入、處理數據並產生輸出。

### 問題挑戰與解決方法
在數據處理前階段，我遇到的問題是**資料型態的不一致性**。

*   **問題描述:** 一開始嘗試讀取資料欄位時，發現無法如預期獲取所有欄位，檢查後發現部分欄位資料被轉換成了布林值或其他不同類型的格式。
*   **解決方法:** 我花了一些時間重新檢視數據載入和初步處理的步驟，例如打印欄位資訊、檢查欄位資料型態等，定位到問題所在。然後我挑整了處理流程，確保在進行特徵工程或模型訓練前，所有數據都具有一致且正確的格式。

### 主要學習與收穫 ###
通過初步的練習，我加深了以下的理解和實踐:

*   **數據檢視與理解:** 更熟練使用 Pandas功能來檢視數據形狀(.shape)、欄位名稱(.columns)、空值狀況(.isnull().sum()) 以及欄位的資料型態 (.info()或.dtypes)。
*   **基礎數據前處理:** 使用了類別特徵 One-hot encoding。 
*   **模型訓練流程:**   對於數據準備、模型實例化、訓練到初步預測的整個 Scikit-learn 流程的認識。
*   **問題排查:**       體驗在實際操作中遇到數據問題並逐步排查解決的過程。

## 使用技術 ##

*   Python
*   Pandas (數據處理)
*   NumPy (數值計算)
*   Scikit-learn (線性回歸模型)
*   Jupyter Notebook (開發環境)

## 如何運行 (基本指引)

1.  從上述 Kaggle 比賽頁面下載 `train.csv` 和 `test.csv` 數據檔案。
2.  確保 Python 環境中安裝了 Pandas, NumPy, และ Scikit-learn。
3.  將數據檔案與 `predict-calorie-expenditure.ipynb` 放在同一目錄下，或修改 Notebook 中的數據讀取路徑。
4.  開啟並運行 Jupyter Notebook。

---
*這是一個正在進行中的學習專案，我將持續更新與改進。*

## 未來計畫與優化方向(Google Ai Studio直接擷取未來方向)

這個專案目前還處於非常初級的階段，未來我計畫從以下幾個方面進行優化和深入學習：

*   **深入探索性數據分析 (EDA)：**
    *   利用視覺化工具 (如 Matplotlib, Seaborn) 更深入地分析各特徵的分佈、特徵之間的相關性，以及特徵與目標變數「Calories_Burned」之間的關係。
*   **特徵工程：**
    *   探索並嘗試創建新的、更有預測能力的特徵。
    *   研究更高級的特徵縮放 (Feature Scaling) 和編碼 (Encoding) 方法。
*   **模型選擇與優化：**
    *   嘗試更多不同的機器學習模型，例如決策樹、隨機森林、梯度提升機 (XGBoost, LightGBM) 等。
    *   學習模型評估指標 (如 MAE, MSE, RMSE, R²) 並用於比較不同模型的表現。
    *   進行交叉驗證 (Cross-Validation) 以獲得更可靠的模型評估結果。
    *   學習並實踐超參數調整 (Hyperparameter Tuning)。
*   **程式碼與呈現：**
    *   使 Notebook 結構更清晰，添加更詳細的 Markdown 註解和分析說明。
    *   確保程式碼的可讀性和可維護性。
