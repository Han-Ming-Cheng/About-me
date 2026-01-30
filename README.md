# 韓明澄 MING-CHENG HAN

📍 台灣 | 📧 han890131@gmail.com | 📱 0978-941-275  
🎓 國立臺北大學 統計研究所  
🎓 國立彰化師範大學 數學系統計資訊組  

---

## 👋 關於我

我是具備統計、邏輯思維與程式基礎的資料分析者，熱愛嘗試新技術、擅長實作與跨領域整合。面對問題具備獨立解決與主動學習的能力，也能在團隊中有效溝通協作，將所學知識靈活應用於實務中，創造具體成果。

---

## 🔧 技術能力

- **資料分析與模型建構**：熟悉迴歸模型、決策樹、羅吉斯迴歸、PCA、SVD、監督式學習與分類器比較。
- **深度學習應用**：使用 PyTorch 架設 CNN，理解核心參數設計與影像特徵提取。
- **資料處理與視覺化**：擅長缺失值處理、常態化、異常值篩選、視覺化解釋模型結果。
- **報告撰寫與說明能力**：熟悉 LaTeX 撰寫報告與技術文件，具備圖文並茂的說明能力。
- **AI 應用知識**：參與 NVIDIA「Building RAG Agents with LLMs」研習，了解語意檢索與 LLM 架構。
- **程式語言**：Python、R、SAS、C++

---

## 🚀 精選專案 (Featured Projects)

### 🤖 美股智慧 AI 分析平台 (US Stock AI Analysis App)
**`Python`** **`Streamlit`** **`Google Gemini API`** **`ETL`**
> 一個整合 GenAI 的全端數據應用，能自動化解讀財報並提供互動式技術分析。

* **自動化 ETL 管線**：實作模組化的 Data Fetcher，自動串接 `yfinance` API 進行資料清洗、容錯處理與格式標準化。
* **RAG 與上下文注入**：將計算後的技術指標 (RSI, MA) 與財務數據 (P/E, EPS) 轉化為結構化 Prompt，結合 **Google Gemini** 模型進行即時財報解讀與風險評估。
* **AI 維護機制 (Guardrails)**：設計 `review_question` 邏輯層，有效過濾非財經相關問題並防止 AI 幻覺，確保回應的專業度與安全性。
* **客製化互動圖表**：透過 Streamlit 注入 JavaScript，實作 Plotly 進階繪圖功能（如畫線分析、Undo/Redo），突破原生套件限制。
* 🔗 [Demo](https://stock-ai-app-c6evappbapgfta6oozgqfx.streamlit.app/)
---

### ⚡ 偷電行為偵測系統 (Electricity Theft Detection)
**`PyTorch`** **`Wide & Deep CNN`** **`Anomaly Detection`** **`Hugging Face`**
> 針對 42,000+ 用戶的巨量電力數據，建置端到端的異常偵測管線。

* **深度學習架構**：實作 **Wide & Deep CNN** 模型，同時捕捉全域特徵與局部週期性特徵，有效識別異常波形。
* **極度不平衡資料處理**：針對竊電樣本稀缺（約 10:1）的問題，應用 **SMOTE** 與 **Random Under Bagging** 技術平衡樣本，大幅提升模型敏感度。
* **量化成果**：
    * **Wide & Deep CNN** 達到 **AUC 0.81**，**MAP@100 (前100名命中率) 達 91%** 。
    * **CBLOF (分群異常因子)** 模型在 **MAP@50 達到 98%** ，能精準鎖定高風險用戶供稽查優先參考。
* **系統落地**：整合 Hugging Face Spaces 實作 Web 介面，提供可視化的即時檢測服務。
* 🔗 [Demo](https://huggingface.co/spaces/peter572210355/demo_steal_electricity_detec)

---

### 🏭 千如電機產學合作：點膠製程良率監控
**`Design of Experiments (DOE)`** **`Decision Trees`** **`Root Cause Analysis`**
> 協助製造業客戶透過數據分析優化製程參數，解決良率不穩定問題。

* **實驗設計 (DOE)**：深入產線進行因子篩選，利用統計檢定 (T-test) 與決策樹分析，找出影響點膠品質的關鍵參數。
* **商業影響**：根據分析結果提出製程參數調整建議，成功協助廠商**提升產品良率約 18%** 。
* **溝通協作**：擔任技術團隊與廠務端的溝通橋樑，將複雜的統計結果轉化為可執行的現場操作建議。

---

### 🏥 Covid-19 死亡風險預測與因子分析
**`Machine Learning`** **`SMOTE`** **`Logistic Regression`** **`PCA`**
> 針對百萬筆醫療數據進行風險因子鑑別，解決醫療資料的類別不平衡難題。

* **特徵工程**：利用 **VIF (變異數膨脹因子)** 與 **PCA (主成分分析)** 處理多重共線性問題，篩選出住院類型與年齡為關鍵風險因子 。
* **模型優化**：原始模型對死亡樣本召回率僅 18%，經由 **SMOTE** 技術處理後，將**召回率 (Recall) 提升至 95%** ，顯著降低漏判高風險病患的機率。
* **可解釋性 AI**：透過邏輯斯迴歸係數分析，量化各變數（如住院、性別、共病）對死亡風險的具體影響倍率 。

---

### 📈 碩士論文：具時間差異的輪廓資料監控
**`Linear Mixed Models`** **`Profile Monitoring`** **`Algorithm Implementation`**
> 解決傳統 SPC 無法處理非等距時間序列 (Irregular Time-Series) 的痛點。

* **演算法開發**：自主開發基於 **Iterative GLS (迭代廣義最小平方)** 與 **BLUP** 的動態參數估計演算法 。
* **監控優化**：設計整合 CUSUM 與 EWMA 的高階控制圖架構，針對高維度輪廓資料進行監控。
* **模擬驗證**：建置 **Monte Carlo 模擬**環境，證實新方法在微小製程偏移 (Small Shift) 的偵測能力顯著優於傳統方法 。

---

## 🎯 未來目標

希望將我在資料分析與品質監控上的專業能力，應用於實務場域，協助企業提升決策效率與製程品質。我樂於挑戰並追求持續成長，期待能與優秀團隊共同打造有影響力的成果。

---
# MING-CHENG HAN | 韓明澄

📍 Taiwan | 📧 han890131@gmail.com | 📱 +886-978-941-275  
🎓 National Taiwan University - Graduate Institute of Statistics  
🎓 National Changhua University of Education - Department of Mathematics (Statistics & Information Division)  

---

## 👋 About Me

I am passionate about data analysis and problem-solving, with a strong background in statistics, logic, and programming. I enjoy exploring new technologies and transforming theoretical concepts into practical results through hands-on experience. I excel in cross-disciplinary teamwork, communication, and independent learning.

---

## 🔧 Technical Skills

- **Statistical Modeling & Machine Learning**: Linear regression, logistic regression, decision trees, PCA, SVD, and various supervised learning methods.
- **Deep Learning**: Familiar with CNN structures and core parameter design using PyTorch.
- **Big Data Projects**: Data preprocessing (missing values, normalization, outliers), classifier comparison and evaluation.
- **Visualization & Communication**: Skilled in presenting results using visual tools and LaTeX documentation.
- **Languages**: Python, R, SAS, C++
- **AI Research**: Completed NVIDIA workshop on *Building RAG Agents with LLMs*, focusing on retrieval-augmented generation (RAG) systems.

---

## 🚀 Featured Projects

### 🤖 US Stock AI Analysis Platform
**`Python`** **`Streamlit`** **`Google Gemini API`** **`ETL`**
> A full-stack data application integrating GenAI to automate financial report analysis and provide interactive technical insights.

* **Automated ETL Pipeline**: Implemented a modular Data Fetcher to automate data cleaning, error handling, and format standardization using the `yfinance` API.
* **RAG & Context Injection**: Transformed calculated technical indicators (RSI, MA) and financial data (P/E, EPS) into structured prompts, integrated with **Google Gemini** for real-time interpretation and risk assessment.
* **AI Guardrails**: Designed a `review_question` logic layer to effectively filter non-financial queries and prevent AI hallucinations, ensuring professional and safe responses (Analysis of `ai_analyzer.py`).
* **Custom Interactive Charts**: Injected JavaScript via Streamlit to implement advanced Plotly drawing features (e.g., trendline drawing, Undo/Redo), overcoming native library limitations (Analysis of `app.py`).
* 🔗 [Demo](https://stock-ai-app-c6evappbapgfta6oozgqfx.streamlit.app/)
---

### ⚡ Electricity Theft Detection System
**`PyTorch`** **`Wide & Deep CNN`** **`Anomaly Detection`** **`Hugging Face`**
> An end-to-end anomaly detection pipeline built for massive electricity usage data from over 42,000 users.

* **Deep Learning Architecture**: Implemented a **Wide & Deep CNN** model to capture both global features and local periodic patterns, effectively identifying abnormal usage waveforms.
* **Imbalanced Data Handling**: Applied **SMOTE** and **Random Under Bagging** techniques to address the extreme scarcity of theft samples (approx. 10:1 ratio), significantly improving model sensitivity.
* **Quantitative Results**:
    * **Wide & Deep CNN** achieved an **AUC of 0.81** and a **MAP@100 (Precision at 100) of 91%**.
    * **CBLOF (Cluster-based Local Outlier Factor)** model reached a **MAP@50 of 98%**, precisely targeting high-risk users for priority inspection.
* **System Deployment**: Integrated Hugging Face Spaces to deploy a web-based interface for real-time detection services.
* 🔗 [Hugging Face Demo](https://huggingface.co/spaces/peter572210355/demo_steal_electricity_detect)

---

### 🏭 Yield Improvement in Manufacturing (Industry Collaboration)
**`Design of Experiments (DOE)`** **`Decision Trees`** **`Root Cause Analysis`**
> Collaborated with ATEC Electronics to optimize manufacturing process parameters and resolve yield instability issues.

* **Design of Experiments (DOE)**: Conducted factor screening on the production line, utilizing statistical tests (T-test) and decision tree analysis to identify key parameters affecting dispensing quality.
* **Business Impact**: Proposed process parameter adjustments based on analysis results, successfully helping the client **increase product yield by approximately 18%**.
* **Communication & Collaboration**: Served as the bridge between the technical team and factory operations, translating complex statistical results into actionable operational recommendations.

---

### 🏥 COVID-19 Mortality Risk Prediction & Factor Analysis
**`Machine Learning`** **`SMOTE`** **`Logistic Regression`** **`PCA`**
> Analyzed over one million healthcare records to identify risk factors, solving the challenge of class imbalance in medical data.

* **Feature Engineering**: Utilized **VIF (Variance Inflation Factor)** and **PCA (Principal Component Analysis)** to handle multicollinearity, identifying patient type (hospitalization) and age as critical risk factors.
* **Model Optimization**: Addressed the issue where the original model had a recall of only 18% for mortality cases. By implementing **SMOTE**, the **Recall was boosted to 95%**, significantly reducing the chance of missing high-risk patients.
* **Explainable AI**: Quantified the specific impact of variables (e.g., hospitalization, gender, comorbidities) on mortality risk using Logistic Regression coefficients.

---

### 📈 Master's Thesis: Monitoring Time-Unequal Profile Data
**`Linear Mixed Models`** **`Profile Monitoring`** **`Algorithm Implementation`**
> Solved the limitation of traditional SPC in handling irregular time-series profile data.

* **Algorithm Development**: Independently developed a dynamic parameter estimation algorithm based on **Iterative GLS (Generalized Least Squares)** and **BLUP (Best Linear Unbiased Prediction)**.
* **Monitoring Optimization**: Designed an advanced control chart architecture integrating **CUSUM** and **EWMA** to monitor high-dimensional profile data.
* **Simulation & Validation**: Built a **Monte Carlo simulation** environment to prove that the proposed method significantly outperforms traditional methods in detecting **small process shifts**.

---

## 🎯 Career Goals

I aim to apply my analytical mindset and statistical knowledge in data-driven roles, particularly in **quality control**, **AI integration**, or **data analytics**. I am looking for opportunities to contribute to innovative and meaningful projects in a collaborative environment.

---
