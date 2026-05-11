# E7PLAY Customer Segmentation & LTV Analysis

Behavioral segmentation and lifetime value analysis for E7PLAY 
badminton venues across three branches (三重、三多、新莊), 
with data-driven membership redesign recommendations.

國立政治大學 資料分析商業應用課程 · NCCU DA Business Project · 2023

---

## Business Problem

E7PLAY attracts a large number of new members but struggles to 
convert them into high-value regulars. 80% of revenue comes from 
Groups 2/3/4, yet Group 2 — the largest segment at 49% of members 
— contributes disproportionately less revenue than smaller, 
higher-value groups.

---

## Data
Data provided by industry partner. 
Raw data is not included in this repository.

---

## Methodology

**Step 1 — Customer Segmentation**

Members segmented into 5 groups based on repurchase behavior, 
visit frequency, and average spend per visit:

| Group | Profile | LTV |
|---|---|---|
| Group 1 | One-time members, no repurchase | Lowest |
| Group 2 | Short-term, low spend | Low |
| Group 3 | Short-term, higher spend (avg 2–3 per visit) | Low-Mid |
| Group 4 | High-frequency regulars, solo visits | High |
| Group 5 | High-frequency regulars, paired visits, avg LTV NT$9,419 | Highest |

**Step 2 — LTV Prediction via Correlation Analysis**

Early spending patterns (1M–36M) correlated against full LTV to 
estimate customer lifecycle by group. Groups 1/2/3 plateau within 
6 months; Groups 4/5 continue growing past 36 months.

**Step 3 — Branch-Level Operations Analysis**

Per-branch visit trends, group mix, and retention thresholds 
analyzed across 三重、三多、新莊 (Jan 2015 – May 2021).

---

## Key Findings

**Branch Comparison**

| | 三重館 | 三多館 | 新莊館 |
|---|---|---|---|
| Growth Driver | Group 2/3/4 | Group 4 | — |
| Core Segment | Group 2/3/4/5 | Group 4 | Group 2/4 |
| Risk | — | Lacks new customers | Losing both old and new |
| Strategy | Loyalty | Market expansion | Operations optimization |

**Retention Threshold**
- 三重 & 三多: visit frequency stabilizes after **6 visits**
- 新莊: requires **12 visits** to stabilize — longer conversion path

---

## Membership Redesign Recommendation

3-tier system designed to push each group toward higher LTV:

| Tier | Upgrade Condition | Target Group |
|---|---|---|
| 紅卡 (Red) | Free entry | Group 1 → 2/3 |
| 金卡 (Gold) | 6 visits within 6 months | Group 2/3 → 4/5 |
| 白金卡 (Platinum) | Top 100 spenders among Gold members | Retain Group 4/5 |

---

## Tools

Python · Pandas · Matplotlib · Regression Analysis

---

## Team

李叡、胡庭瑜、呂宜珊、江詠忻、黃筠茜（Athena）、鄔孟真

助教：劉紀昕 · 國立政治大學資管系

---

## 中文簡介

針對 E7PLAY 桌球館三個分館（三重、三多、新莊）進行消費者分群與 LTV 分析。
將會員依回購行為、消費次數與客單價分成五群，並透過短期消費金額與 LTV 
之相關性推估顧客生命週期。結合各分館營運現況，提出以提升顧客黏著度為
核心的三級會員制度優化建議。資料集區間：2015.1 – 2021.5。
