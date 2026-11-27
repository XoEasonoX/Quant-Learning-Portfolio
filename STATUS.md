# 程式練習 — STATUS.md

**最後更新：2026-11-27**

本文件為學習交接單一權威來源。新對話先讀取 GitHub 最新版；使用者明確更新的進度優先。不要假設未確認內容完成。

## 長期目標
- 目標：2029 年底前具備獨立建立自動化 Quant Trading System 的能力。
- Quant Trading / Quant Finance 為方向指引；培養可轉移的數學、統計、程式、資料、ML/AI能力，保留 DS、ML、SE、Risk / Model Validation 等選項。
- 不保證策略獲利，重視扎實能力與可驗證成果。

## 六條能力線
1. Programming & Algorithms：Python → LeetCode → Data Structures / Algorithms → OOP / Git。
2. Data Science & Engineering：NumPy、Pandas、SQL、資料清理、視覺化、時間序列。
3. Mathematics：校內數學、線代、微積分、實分析、機率、統計、最佳化、數值方法。
4. Statistics & Econometrics：推論、機率、假設檢定、迴歸、時間序列、計量經濟。
5. ML & AI：Google MLCC、Scikit-learn、神經網路、深度學習、金融 ML。
6. Quant Finance：市場、投資組合理論、資產定價、風險、研究、Backtesting、Execution、Automated Trading。

## LeetCode
### 已確認 AC
#1, #9, #13, #14, #19, #20, #21, #26, #27, #35, #49, #53, #69, #80, #83, #88, #121, #125, #136, #141, #142, #143, #155, #206, #217, #232, #234, #242, #268, #278, #283, #344, #347, #367, #448, #704, #739, #771, #876, #1903, #2425, #2427, #2586, #2683, #102, #104, #100, #226, #112, #572, #110, #543, #101, #617, #404, #257, #938, #700, #701, #653, #1047, #682, #496, #844, #901。

### 重要概念 / 近期題目
- #496 Next Greater Element I：Monotonic Stack；遇到更大元素時 pop 並建立對應，未解者為 -1。
- #844 Backspace String Compare：stack 處理 backspace；獨立完成。
- #653 Two Sum IV：DFS + complement + seen，避免節點自配對。
- #700 / #701 / #938：BST 搜尋、插入、範圍總和與剪枝。
- #543：postorder 高度，left + right 計算直徑。
- #110：O(n) bottom-up，-1 sentinel 判斷失衡。
- #257：路徑累積與 leaf result；spaced review 只依使用者明確指定安排。
- #901 Online Stock Span（2026-11-27）：AC，提示引導完成；理解 stack 儲存 (price, span)，遇到小於或等於當前價格時 pop 並吸收其 span，再 push (price, span)。記為 guided completion / solution understood，不視為完全獨立完成。

### 複習與教學原則
- 待複習佇列只由使用者明確指定；不自行添加。
- 不立即重寫剛 AC 題；先做新題再依指定 review。
- Socratic 教學：一次一個問題，逐級提示；除非使用者要求完整解答或疲倦求解。
- AC不代表能完全無提示重現；重要能力註明獨立／提示後／解答後理解。

### 下一步
- LeetCode：安排適合的新題；review 只依使用者明確指定的佇列。

## Pandas / Data Analysis
已學：
- DataFrame/Series、選取、filter、mean/max、vectorized operations、新欄位、shift 計算簡單報酬。
- Datetime、set_index、.loc 日期與區間。
- Returns、Cumulative Returns、Portfolio Value、std、annualized volatility（sqrt(252)）。
- Sharpe Ratio（先用 rf=0）、Annualized Sharpe。
- Drawdown / MDD：cummax peak、(Portfolio-peak)/peak、min drawdown，百分比格式化。

**下一步：** 整合 Returns、Portfolio Value、Volatility、Sharpe、Drawdown、MDD，完成簡單策略績效分析。

## Google Machine Learning Crash Course (MLCC)
已學：Intro、Linear Regression、MAE/MSE/RMSE、Gradient Descent、Hyperparameters、Gradient Descent interactive exercise。
**目前：** Linear Regression programming exercise `linear_regression_taxi.ipynb`。
套件安裝已成功：`%pip install google-ml-edu keras matplotlib numpy pandas tensorflow`（因 Colab Python 3.13 與教材固定版本相容問題調整）。不要重跑成功的 install cell，除非 runtime reset。
**下一步：** 從 `Load dependencies` cell 接續，依 notebook 順序進行。

## 學習安排原則
- 校內數學課優先兼顧，自學與休息平衡。
- 週自學參考約 12 小時，考週／疲勞可調整。
- Socratic Tutor；LeetCode流程：理解題目→設計→實作→轉移。

## Portfolio
- Repository：`XoEasonoX/Quant-Learning-Portfolio`。
- Portfolio 只保存使用者選擇的展示成果，不記錄日常流水帳；使用者決定是否保存。
- STATUS 交接與Portfolio成果分離。

## GitHub 交接機制（2026-11-27）
- GitHub 已連接並實測讀取本 repository。
- 單一進度來源：本文件（`STATUS.md`）。
- 新對話時，依 Project Instructions 指向的 GitHub URL 讀取最新版；不可假設只靠 Project 內舊檔。
- 每次學習結束，先整理進度再直接更新 GitHub STATUS.md，並確認 commit 成功；不要讓使用者自行下載/替換 Project Source。
- 若無法讀取或寫入 GitHub，明確告知，勿假稱已更新。
- GitHub URL：https://github.com/XoEasonoX/Quant-Learning-Portfolio/blob/main/STATUS.md

## 新對話交接流程
1. 讀取此 GitHub 文件最新版。
2. 核對使用者最新明確進度，不重複完成事項。
3. 依各線「下一步」接續；不推測未完成事項。
4. 學習結束時更新本文件，保持覆寫式精簡、下次起點明確。
