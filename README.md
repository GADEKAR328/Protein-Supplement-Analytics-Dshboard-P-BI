<div align="center">

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&height=220&color=0:1A2A6C,50:B21F1F,100:FDBB2D&text=Protein%20Supplement%20Analytics&fontSize=38&fontColor=ffffff&animation=scaleIn" width="100%">
</p>

<br/>

[![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)](https://powerbi.microsoft.com)
[![Excel](https://img.shields.io/badge/Excel-217346?style=for-the-badge&logo=microsoftexcel&logoColor=white)](https://microsoft.com/excel)
[![DAX](https://img.shields.io/badge/DAX-20%20Formulas-1A3C5E?style=for-the-badge&logo=databricks&logoColor=white)](#dax-engineering)
[![Dataset](https://img.shields.io/badge/Dataset-30%20Brands-2D6A1F?style=for-the-badge&logo=databricks&logoColor=white)](#data-model)
[![Columns](https://img.shields.io/badge/Calculated%20Columns-5-blueviolet?style=for-the-badge)](#dax-engineering)
[![Measures](https://img.shields.io/badge/Measures-15-orange?style=for-the-badge)](#dax-engineering)
[![Status](https://img.shields.io/badge/Status-Completed%20%E2%9C%85-success?style=for-the-badge)](#)

<br/>

![Visitors](https://visitor-badge.laobi.icu/badge?page_id=GADEKAR328.Protein-Supplement-Analytics-Dshboard-P-BI)
[![GitHub stars](https://img.shields.io/github/stars/GADEKAR328/Protein-Supplement-Analytics-Dshboard-P-BI?style=social)](https://github.com/GADEKAR328/Protein-Supplement-Analytics-Dshboard-P-BI/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/GADEKAR328/Protein-Supplement-Analytics-Dshboard-P-BI?style=social)](https://github.com/GADEKAR328/Protein-Supplement-Analytics-Dshboard-P-BI/network)

<br/>

> ### 💬 *"What's really in your protein?"*
> *A data-driven safety & nutrition investigation across 30 Indian supplement brands*
> *Amazon.in · Flipkart · Brand Websites · FSSAI · NSF · Informed Sport*

<br/>

</div>

---

## 🖥️ Dashboard Preview

<div align="center">

[![Dashboard Preview](https://github.com/GADEKAR328/Protein-Supplement-Analytics-Dshboard-P-BI/blob/ca790e708508364aac44bdfa8f022f897436ac51/Protein%20Supplement%20Dshboard.jpg?raw=true)](https://github.com/GADEKAR328/Protein-Supplement-Analytics-Dshboard-P-BI/blob/ca790e708508364aac44bdfa8f022f897436ac51/Protein%20Supplement%20Dshboard.jpg?raw=true)

*📌 Click image to view full resolution · Built entirely in Power BI Desktop*

</div>

---

## 📌 Project Overview

<div align="center">

```
╔══════════════════════════════════════════════════════════════════════╗
║   India's protein supplement market is worth ₹5,000 Cr+ and is       ║
║   largely unregulated — amino spiking, proprietary blends,           ║
║   undisclosed sweeteners and heavy metal contamination are           ║
║   widespread. Young athletes and gym-goers are most vulnerable.      ║
╚══════════════════════════════════════════════════════════════════════╝
```

</div>

This dashboard was built to answer **three questions** a data analyst would investigate:

| ❓ Question | 📊 Answer |
|---|---|
| Which brands are safe to buy for daily use? | Ranked by a **composite Clean Label Score (0–100)** |
| Which brands offer the best protein per rupee? | Measured by **Price per gram of protein (INR/g)** |
| Which products carry risk for young Indian users? | Flagged using a **3-signal safety model** |

### 🎯 Project Goals

- ✅ Analyse **30 Indian supplement brands** across Amazon, Flipkart and brand websites
- ✅ Build a **composite safety scoring system** based on FSSAI + WHO 2023 guidelines
- ✅ Identify **value vs safety trade-offs** across Whey, Plant, Gainer, BCAA and Creatine categories
- ✅ Create an **interactive Power BI dashboard** with slicers, conditional formatting and drill-through capability
- ✅ Engineer **20 DAX formulas** (5 calculated columns + 15 measures) from scratch
- ✅ Deliver **plain-language safety alerts** any buyer — not just a data analyst — can act on

---

## 📊 Dashboard Visuals at a Glance

### Dashboard Architecture

```
┌─────────────────────────────────────────────────────────────────────────┐
│                       ROW 1 — KPI COMMAND STRIP                         │
│                                                                         │
│  ┌──────────┐  ┌──────────────┐  ┌────────────┐  ┌───────────────────┐  │
│  │ 30       │  │ 22.71g       │  │ 1          │  │ 6                 │  │
│  │ Brands   │  │ Avg Protein  │  │ High Risk  │  │ Prop. Blends      │  │
│  └──────────┘  └──────────────┘  └────────────┘  └───────────────────┘  │
│  ┌──────────────────┐  ┌───────────────────────────────────────────────┐│
│  │ 56.7%            │  │ 68.30 Clean Label Score                       ││
│  │ Certified        │  │ ◀ Primary KPI Card                           │ │
│  └──────────────────┘  └───────────────────────────────────────────────┘│
├──────────────────────────────────┬──────────────────────────────────────┤
│  ROW 2A — Clean Label Score Bar  │  ROW 2B — Sweetener Risk Donut       │
│                                  │                                      │
│  Fast&Up    ████████████████  87 │   🟢 Green  ████████████   56.7%     │
│  Tata 1mg   ███████████████  86  │   🟡 Yellow ███████        26.7%     │
│  NAKPRO     ████████████  78     │   🟠 Orange ████           16.7%     │
│  MuscleBlze ███████████  70      │                                      │
│  GNC        ██████  40           │   CC-02 Sweetener_Risk as legend     │
│  BigMuscles ████  28             │   M-09 Sweetener Risk % as value     │
├──────────────┬───────────────────┴──────────────────────────────────────┤
│  ROW 3A      │  ROW 3B                   │  ROW 3C                      │
│  BCAA Chart  │  Protein Efficiency Index │  4 Slicers                   │
│  by Category │  Scatter Chart            │  Category · Platform         │
│  M-07 + Ref  │  Price vs Efficiency      │  Certification               │
│  Line @ 5g   │  Bubble = Clean Score     │  Sweetener Safety            │
├──────────────┴───────────────────────────┴──────────────────────────────┤
│                       ROW 4 — DATA TABLES                               │
│  ┌──────────────────────────────────┐  ┌──────────────────────────────┐ │
│  │ SAFETY MATRIX                    │  │ VALUE TABLE                  │ │
│  │ Brand · Certified · Sweet Risk   │  │ Brand · Tier · Price/g       │ │
│  │ Blend · Heavy Metal · M-06 Score │  │ Score · Safety Alert (CC-04) │ │
│  └──────────────────────────────────┘  └──────────────────────────────┘ │
└─────────────────────────────────────────────────────────────────────────┘
```

### Visual Summary Table

| # | Visual Type | Measure / Field | Key Insight Delivered |
|---|---|---|---|
| 1 | KPI Card ×6 | M-01 M-02 M-04 M-05 M-13 M-15 | Full market snapshot at a glance |
| 2 | Clustered Bar | M-15 Clean Label Score by Brand | Green ≥85 · Amber 65–84 · Red <65 |
| 3 | Donut Chart | M-09 by CC-02 Sweetener_Risk | Sweetener safety tier breakdown |
| 4 | Horizontal Bar | BCAA_Per_Serving_g avg by Category | MPS threshold reference line at 5g |
| 5 | Scatter Chart | Price vs Protein Efficiency Index | Top-right = best safe value brands |
| 6 | Matrix Visual | M-06 + M-15 with conditional format | Full brand safety heatmap |
| 7 | Table Visual | CC-03 CC-04 M-03 M-15 by Brand | Colour-coded buyer decision table |

---

## 🔍 Key Insights Uncovered

### 🔴 Safety Intelligence

<details>
<summary><b>Click to expand — Safety Findings</b></summary>

<br/>

| Finding | Count | Real-World Impact |
|---|---|---|
| Brands with HIGH amino spiking + HIGH heavy metal risk simultaneously | **6 / 30** | Most dangerous for teenage daily use |
| Brands using proprietary blends — hidden dosages | **6 / 30** | Buyers cannot verify actual ingredient amounts |
| Products with NO third-party certification | **13 / 30 (43.3%)** | No NSF · Informed Sport · Trustified verification |
| Brands scoring below 65 on Clean Label Score | **2 / 30** | Avoid — do not use without lab COA |
| Brands scoring above 85 — Buy confidently | **8 / 30** | Certified clean with transparent labelling |

**Analyst Insight:**
> The 3-signal safety model (Amino Spiking Risk = High AND Heavy Metal Risk = High AND Third_Party_Certified = No) identifies brands that simultaneously fail on all three safety dimensions. These are the products most likely to harm an uninformed teenage buyer using daily protein supplements without awareness of what they are consuming.

**Most dangerous combination found:**

```
Amino Spiking Risk = HIGH  ← cheap aminos inflating protein reading on label
+
Heavy Metal Risk   = HIGH  ← lead, arsenic, cadmium above safe daily limits
+
Third Party Cert   = NO    ← no independent lab verification exists
+
Proprietary Blend  = YES   ← exact dosages legally hidden from buyer
= CC-04 → "HIGH RISK — Avoid"
```

</details>

---

### 🟡 Sweetener Safety Landscape

<details>
<summary><b>Click to expand — Sweetener Findings</b></summary>

<br/>

```
Sweetener Distribution across 30 Indian Brands (FSSAI + WHO 2023)
──────────────────────────────────────────────────────────────────
🟢 CLEAN   (None / Stevia / Monk Fruit)      ████████████████████  56.7%
🟡 CAUTION (Sucralose / Ace-K)               ██████████            26.7%
🟠 HIGH    (Sucralose + Ace-K combined)       ██████                16.7%
🔴 AVOID   (Aspartame)                        ░░░░░░                 0.0%
──────────────────────────────────────────────────────────────────
Source: FSSAI approved sweeteners list + WHO 2023 non-sugar sweetener guidance
```

| Sweetener | CC-02 Tier | FSSAI Status | WHO 2023 |
|---|---|---|---|
| None | 🟢 Green | N/A | Ideal |
| Stevia | 🟢 Green | Approved | Acceptable |
| Monk Fruit | 🟢 Green | Approved | Acceptable |
| Sucralose | 🟡 Yellow | Approved | Caution |
| Ace-K | 🟡 Yellow | Approved | Caution |
| Sucralose + Ace-K | 🟠 Orange | Approved | High Caution |
| Aspartame | 🔴 Red | Approved | Avoid (IARC 2B possible carcinogen) |

**Analyst Insight:**
> The 0% Aspartame finding is not reassuring — it means brands use multi-sweetener combinations (Sucralose + Ace-K) to stay technically compliant while achieving maximum sweetness intensity at lower individual dosages per sweetener. This combination falls in the Orange tier per WHO 2023 guidance, which advises against long-term daily use.

</details>

---

### 🟢 Nutrition & Value Analysis

<details>
<summary><b>Click to expand — Nutrition & Value Findings</b></summary>

<br/>

**BCAA Per Serving by Category vs MPS Threshold:**

```
Category        Avg BCAA/Serving    MPS Status
──────────────────────────────────────────────
Gainer          7.3g  ███████████   ✅ Above 5g threshold
BCAA            7.0g  ██████████    ✅ Above 5g threshold
Whey WPI        5.9g  ████████      ✅ Above 5g threshold
Whey Blend      5.5g  ███████       ✅ Above 5g threshold
Whey WPC        5.3g  ███████       ✅ Above 5g threshold
Plant           5.1g  ███████       ✅ Above 5g threshold
Creatine        0.0g  —             ℹ️  Not applicable
──────────────────────────────────────────────
MPS Threshold: 5g leucine+isoleucine+valine per serving
```

**Protein Efficiency Index (Protein per 100 calories):**

| Category | Efficiency Score | Verdict |
|---|---|---|
| Whey Isolate (WPI) | 20–25 | ✅ Best — lean muscle without excess calories |
| Whey Concentrate (WPC) | 18–22 | ✅ Good |
| Plant-Based | 15–20 | ✅ Acceptable |
| BCAA | Varies | ℹ️ Supplement not meal replacement |
| **Mass Gainer** | **4–6** | **❌ Worst — high calorie, low protein ratio** |

**Value Tiers (Price per gram of protein):**

```
< ₹5/g    Excellent  AS-IT-IS (₹2.42) · NAKPRO (₹2.54) · Fast&Up (₹5.80)
₹5–10/g   Good       OZiva · Myprotein · MuscleBlaze
₹10–15/g  Average    Dymatize · GNC
> ₹15/g   Overpriced Some premium international imports
```

**Analyst Insight:**
> Mass Gainers are the most misleading category — high calorie density (4–6 protein per 100 calories) is aggressively marketed to teenagers seeking size gains, but the data shows they deliver the worst protein efficiency in the dataset while often being priced in the Average-to-Overpriced tier. Parents of teenage athletes should be particularly aware of this finding.

**Best overall buy:** Fast&Up — highest Clean Label Score (87) + Excellent value tier (₹5.80/g) + third-party certified.

**Best budget buy:** AS-IT-IS Nutrition — ₹2.42/g protein, certified, no proprietary blend, Stevia sweetener.

</details>

---

### 💰 Platform & Market Intelligence

<details>
<summary><b>Click to expand — Platform & Market Findings</b></summary>

<br/>

| Platform | Avg Price Per Serving | Price Position |
|---|---|---|
| Amazon.in | Varies by brand — M-14 measure tracks this | Competitive |
| Flipkart | Generally competitive vs Amazon | Competitive |
| Brand Website | Often highest — premium positioning | Premium |

**M-14 Platform Price Index** (hardcoded to Amazon in DAX, responds to Platform slicer for cross-filtering) enables side-by-side platform comparison directly in the dashboard.

**Market-level finding:**
> Using the Platform slicer on the dashboard, users can compare the same brand's price across Amazon, Flipkart and brand website simultaneously — revealing platform pricing gaps that recruiters find analytically insightful as a multi-source data integration demonstration.

</details>

---

## 🧮 DAX Engineering

<div align="center">

![DAX Badge](https://img.shields.io/badge/Calculated%20Columns-CC--01%20to%20CC--05-1A3C5E?style=flat-square&logo=databricks&logoColor=white)
![DAX Badge](https://img.shields.io/badge/Measures-M--01%20to%20M--15-2D6A1F?style=flat-square&logo=databricks&logoColor=white)
![DAX Badge](https://img.shields.io/badge/Techniques-RANKX%20%7C%20AVERAGEX%20%7C%20ALLEXCEPT%20%7C%20SWITCH%20%7C%20DIVIDE-854F0B?style=flat-square)

</div>

### Calculated Columns (CC-01 to CC-05)

> **How to add:** Right-click table name in Power BI Fields pane → New Column → paste formula

| ID | Column Name | Type | Purpose |
|---|---|---|---|
| CC-01 | `Leucine_Adequacy` | Calculated Column | Flags Adequate / Borderline / Inadequate vs 2500mg MPS threshold |
| CC-02 | `Sweetener_Risk` | Calculated Column | SWITCH → Green / Yellow / Orange / Red per FSSAI + WHO 2023 |
| CC-03 | `Value_Tier` | Calculated Column | VAR PPG = Price ÷ Protein → 4 buyer-friendly value buckets |
| CC-04 | `Safety_Alert` | Calculated Column | 3-signal AND/OR logic → HIGH RISK · CAUTION · SAFE plain text |
| CC-05 | `Category_Label` | Calculated Column | Short axis labels — WPI · WPC · Plant · Gainer · BCAA · Creatine |

<details>
<summary><b>View all 5 Calculated Column formulas</b></summary>

<br/>

**CC-01 — Leucine Adequacy Flag**
```dax
Leucine_Adequacy =
IF(
    protein_supplements_india[Leucine_mg] >= 2500,
    "Adequate",
    IF(protein_supplements_india[Leucine_mg] >= 1500,
        "Borderline",
        "Inadequate"
    )
)
```

**CC-02 — Sweetener Risk Label**
```dax
Sweetener_Risk =
SWITCH(protein_supplements_india[Sweetener_Used],
    "None",              "Green",
    "Stevia",            "Green",
    "Monk Fruit",        "Green",
    "Sucralose",         "Yellow",
    "Ace-K",             "Yellow",
    "Sucralose + Ace-K", "Orange",
    "Aspartame",         "Red",
    "Unknown"
)
```

**CC-03 — Value Tier**
```dax
Value_Tier =
VAR PPG = DIVIDE(
    protein_supplements_india[Price_Per_Serving_INR],
    protein_supplements_india[Protein_Per_Serving_g], 0)
RETURN
SWITCH(TRUE(),
    PPG <= 5,  "Excellent (<=5 INR/g)",
    PPG <= 10, "Good (5-10 INR/g)",
    PPG <= 15, "Average (10-15 INR/g)",
               "Overpriced (>15 INR/g)"
)
```

**CC-04 — Safety Alert Flag**
```dax
Safety_Alert =
IF(
    protein_supplements_india[Amino_Spiking_Risk] = "High"
    && protein_supplements_india[Has_Proprietary_Blend] = "Yes"
    && protein_supplements_india[Third_Party_Certified] = "No",
    "HIGH RISK - Avoid",
    IF(
        protein_supplements_india[Heavy_Metal_Risk] = "High"
        || protein_supplements_india[Amino_Spiking_Risk] = "Medium",
        "CAUTION - Verify COA",
        "SAFE - Buy with confidence"
    )
)
```

**CC-05 — Product Category Short Label**
```dax
Category_Label =
SWITCH(protein_supplements_india[Category],
    "Whey Concentrate", "Whey WPC",
    "Whey Isolate",     "Whey WPI",
    "Plant-Based",      "Plant",
    "Mass Gainer",      "Gainer",
    "Creatine",         "Creatine",
    "BCAA",             "BCAA",
    protein_supplements_india[Category]
)
```

</details>

---

### Measures (M-01 to M-15)

> **How to add:** Home tab in Power BI → New Measure → paste formula

| ID | Measure Name | Category | DAX Pattern |
|---|---|---|---|
| M-01 | Total Products | KPI | `COUNTROWS` |
| M-02 | Avg Protein Per Serving | Nutrition | `AVERAGE` |
| M-03 | Price Per Gram of Protein | Value | `DIVIDE` + `AVERAGE` |
| M-04 | Certified Products % | Safety | `FORMAT` + `DIVIDE` + `CALCULATE` |
| M-05 | Proprietary Blend Count | Safety | `CALCULATE` + `COUNTROWS` |
| M-06 | Composite Safety Score | Safety | Weighted VAR penalties composite |
| M-07 | Avg BCAA Per Category | Amino Acid | `CALCULATE` + `ALLEXCEPT` |
| M-08 | Adequate Leucine Products | Amino Acid | `CALCULATE` + CC-01 reference |
| M-09 | Sweetener Risk % | Ingredient Safety | `FORMAT` + `DIVIDE` + `ALL` |
| M-10 | Amino Spike Alert Count | Fraud Detection | `CALCULATE` + filter |
| M-11 | Protein Efficiency Index | Nutrition | `AVERAGEX` + `DIVIDE` |
| M-12 | Value Rank by Category | Value | `RANKX` + `EARLIER` + `DENSE` |
| M-13 | High Risk for Youth | Public Health | `CALCULATE` dual filter |
| M-14 | Platform Price Index | Market Insight | `AVERAGEX` + `FILTER` |
| M-15 | Clean Label Score | Composite Index | Multi-VAR weighted composite |

<details>
<summary><b>View all 15 Measure formulas</b></summary>

<br/>

**M-01 — Total Products**
```dax
Total Products = COUNTROWS(protein_supplements_india)
```

**M-02 — Average Protein Per Serving**
```dax
Avg Protein Per Serving =
AVERAGE(protein_supplements_india[Protein_Per_Serving_g])
```

**M-03 — Price Per Gram of Protein**
```dax
Price Per Gram of Protein =
DIVIDE(
    AVERAGE(protein_supplements_india[Price_Per_Serving_INR]),
    AVERAGE(protein_supplements_india[Protein_Per_Serving_g]), 0)
```

**M-04 — Third-Party Certified %**
```dax
Certified Products % =
FORMAT(
    DIVIDE(
        CALCULATE(COUNTROWS(protein_supplements_india),
            protein_supplements_india[Third_Party_Certified] = "Yes"),
        COUNTROWS(protein_supplements_india), 0
    ) * 100, "0.0"
) & "%"
```

**M-05 — Proprietary Blend Count**
```dax
Proprietary Blend Count =
CALCULATE(
    COUNTROWS(protein_supplements_india),
    protein_supplements_india[Has_Proprietary_Blend] = "Yes"
)
```

**M-06 — Composite Safety Score**
```dax
Safety Score =
VAR CertScore    = CALCULATE(COUNTROWS(protein_supplements_india),
                       protein_supplements_india[Third_Party_Certified]="Yes") * 30
VAR BlendPenalty = CALCULATE(COUNTROWS(protein_supplements_india),
                       protein_supplements_india[Has_Proprietary_Blend]="Yes") * -20
VAR SweetPenalty = CALCULATE(COUNTROWS(protein_supplements_india),
                       protein_supplements_india[Sweetener_Safety]="High Caution") * -15
                 + CALCULATE(COUNTROWS(protein_supplements_india),
                       protein_supplements_india[Sweetener_Safety]="Caution") * -5
VAR MetalPenalty = CALCULATE(COUNTROWS(protein_supplements_india),
                       protein_supplements_india[Heavy_Metal_Risk]="High") * -25
                 + CALCULATE(COUNTROWS(protein_supplements_india),
                       protein_supplements_india[Heavy_Metal_Risk]="Medium") * -10
VAR AminoSpike   = CALCULATE(COUNTROWS(protein_supplements_india),
                       protein_supplements_india[Amino_Spiking_Risk]="High") * -20
VAR Total = COUNTROWS(protein_supplements_india)
RETURN
DIVIDE(
    (Total * 100) + CertScore + BlendPenalty + SweetPenalty + MetalPenalty + AminoSpike,
    Total, 0)
```

**M-07 — Avg BCAA Per Category**
```dax
Avg BCAA Per Category =
CALCULATE(
    AVERAGE(protein_supplements_india[BCAA_Per_Serving_g]),
    ALLEXCEPT(protein_supplements_india, protein_supplements_india[Category])
)
```

**M-08 — Leucine Adequacy Count**
```dax
Adequate Leucine Products =
CALCULATE(
    COUNTROWS(protein_supplements_india),
    protein_supplements_india[Leucine_Adequacy] = "Adequate"
)
```

**M-09 — Sweetener Risk Distribution %**
```dax
Sweetener Risk % =
FORMAT(
    DIVIDE(
        COUNTROWS(protein_supplements_india),
        CALCULATE(COUNTROWS(protein_supplements_india),
            ALL(protein_supplements_india)), 0
    ) * 100, "0.0"
) & "%"
```

**M-10 — Amino Spiking Alert Count**
```dax
Amino Spike Alert Count =
CALCULATE(
    COUNTROWS(protein_supplements_india),
    protein_supplements_india[Amino_Spiking_Risk] = "High"
)
```

**M-11 — Protein Efficiency Index**
```dax
Protein Efficiency Index =
AVERAGEX(
    protein_supplements_india,
    DIVIDE(
        protein_supplements_india[Protein_Per_Serving_g],
        protein_supplements_india[Calories_Per_Serving], 0
    ) * 100
)
```

**M-12 — Best Value Rank by Category**
```dax
Value Rank =
VAR SelectedCategory = SELECTEDVALUE(protein_supplements_india[Category])
VAR CurrentValue =
    AVERAGEX(protein_supplements_india,
        DIVIDE(protein_supplements_india[Protein_Per_Serving_g],
               protein_supplements_india[Price_Per_Serving_INR], 0))
RETURN
RANKX(
    FILTER(ALL(protein_supplements_india),
        protein_supplements_india[Category] = SelectedCategory),
    AVERAGEX(
        FILTER(protein_supplements_india,
            protein_supplements_india[Brand]
            = EARLIER(protein_supplements_india[Brand])),
        DIVIDE(protein_supplements_india[Protein_Per_Serving_g],
               protein_supplements_india[Price_Per_Serving_INR], 0)),
    CurrentValue, DESC, DENSE)
```

**M-13 — High Risk Products for Young Users**
```dax
High Risk for Youth =
CALCULATE(
    COUNTROWS(protein_supplements_india),
    protein_supplements_india[Heavy_Metal_Risk]   = "High",
    protein_supplements_india[Amino_Spiking_Risk] = "High"
)
```

**M-14 — Platform Price Index**
```dax
Platform Price Index =
AVERAGEX(
    FILTER(protein_supplements_india,
        protein_supplements_india[Platform] = "Amazon"),
    protein_supplements_india[Price_Per_Serving_INR]
)
```

**M-15 — Clean Label Score (Flagship Measure)**
```dax
Clean Label Score =
VAR Transparency = AVERAGE(protein_supplements_india[Ingredient_Transparency_Score])
VAR Safety       = AVERAGE(protein_supplements_india[Overall_Safety_Score])
VAR Certified    =
    DIVIDE(CALCULATE(COUNTROWS(protein_supplements_india),
        protein_supplements_india[Third_Party_Certified] = "Yes"),
        COUNTROWS(protein_supplements_india), 0) * 10
VAR NoBlend      =
    DIVIDE(CALCULATE(COUNTROWS(protein_supplements_india),
        protein_supplements_india[Has_Proprietary_Blend] = "No"),
        COUNTROWS(protein_supplements_india), 0) * 10
VAR CleanSweet   =
    DIVIDE(CALCULATE(COUNTROWS(protein_supplements_india),
        protein_supplements_india[Sweetener_Safety] = "Clean"),
        COUNTROWS(protein_supplements_india), 0) * 10
RETURN
ROUND(
    (Transparency * 0.3 + Safety * 0.4 + Certified + NoBlend + CleanSweet) / 1.1, 1)
```

> **Score interpretation:** >85 = Buy confidently · 65–85 = Acceptable with caution · <65 = Avoid or verify lab COA first

</details>

---

## 🛠️ Tools & Tech Stack

<div align="center">

| Layer | Tool | Detail |
|---|---|---|
| 📊 Visualization | **Power BI Desktop** | 7 visual types · conditional formatting · analytics pane · bookmarks |
| 🧮 Computation | **DAX** | 5 calculated columns · 15 measures · RANKX · AVERAGEX · ALLEXCEPT · SWITCH · FORMAT |
| 🗃️ Data Source | **Microsoft Excel (.xlsx)** | 30 brands · 25+ attributes per product |
| 🔧 Data Prep | **Power Query** | Data type enforcement · column cleaning · decimal validation |
| 🎨 Design | **Custom dark theme** | Supplement photography · navy / green / amber / red safety colour palette |
| 📏 Regulatory | **FSSAI + WHO 2023 + NSF** | Sweetener tiers · heavy metal limits · certification standards |

</div>

---

## 📐 Data Model

<div align="center">

```
┌────────────────────────────────────────────────────────────┐
│           protein_supplements_india  (Single Table)        │
│                    30 rows · 25+ columns                   │
├────────────────┬───────────────────────────────────────────┤
│ IDENTITY       │ Brand · Category · Platform               │
├────────────────┼───────────────────────────────────────────┤
│ NUTRITION      │ Protein_Per_Serving_g                     │
│                │ Calories_Per_Serving                      │
│                │ BCAA_Per_Serving_g                        │
│                │ Leucine_mg                                │
├────────────────┼───────────────────────────────────────────┤
│ PRICING        │ Price_Per_Serving_INR                     │
├────────────────┼───────────────────────────────────────────┤
│ SAFETY         │ Third_Party_Certified (Yes/No)            │
│                │ Has_Proprietary_Blend (Yes/No)            │
│                │ Amino_Spiking_Risk (High/Medium/Low)      │
│                │ Heavy_Metal_Risk (High/Medium/Low)        │
│                │ Sweetener_Used                            │
│                │ Sweetener_Safety                          │
├────────────────┼───────────────────────────────────────────┤
│ SCORES         │ Ingredient_Transparency_Score (numeric)   │
│                │ Overall_Safety_Score (numeric)            │
└────────────────┴───────────────────────────────────────────┘
```

</div>

**Model type:** Single flat table — no relationships needed. All 5 calculated columns and 15 measures operate on this one table, keeping the model lean and performant.

---

## 📁 Repository Contents

```
📦 Protein-Supplement-Analytics-Dashboard-P-BI
 ┣ 📊 Protein Supplement Dashboard.jpg      ← Full dashboard screenshot (1.28 MB)
 ┣ 📋 protein_supplements_india.xlsx        ← Source dataset (30 brands × 25+ cols)
 ┣ 📄 Protein_Supplement_DAX_Formulas.pdf   ← All 20 DAX formulas reference sheet
 ┗ 📝 README.md                             ← This file
```

---

## 🎯 Business Impact & Real-World Use Cases

<div align="center">

| 👤 Audience | 🎯 Use Case | 📊 Dashboard Feature Used |
|---|---|---|
| **Data Analyst / BI Developer** | Demonstrates full Power BI analytical stack | DAX · conditional formatting · multi-visual layout |
| **Product / Brand Manager** | Competitive benchmarking — safety vs value | Safety Matrix · Clean Label Score bar |
| **Public Health Researcher** | Quantify supplement risk for underage users | M-13 High Risk for Youth · CC-04 Safety Alert |
| **Young Buyer / Parent** | Plain-language buy / avoid recommendation | CC-04 Safety Alert · M-15 Clean Label Score |
| **FSSAI / Regulator** | Identify brands requiring COA investigation | Safety matrix heatmap · amino spiking count |
| **Recruiter / Hiring Manager** | Assess DAX depth + business thinking + design | Entire dashboard + this README |

</div>

---

## 🏆 Skills Demonstrated

<div align="center">

| ⚙️ Skill | 📌 Evidence in this project |
|---|---|
| **DAX Authoring** | 15 measures including RANKX, AVERAGEX, ALLEXCEPT, weighted composites, FORMAT text measures |
| **Calculated Columns** | 5 columns — IF nesting, SWITCH pattern, VAR intermediate calculations |
| **Data Modelling** | Single-table model with enrichment via calculated columns |
| **Conditional Formatting** | Applied per-column in matrix visual across 5 dimensions simultaneously |
| **Visual Design** | 7 visual types · custom dark theme · colour palette tied to safety meaning |
| **Business Thinking** | Safety scoring built on FSSAI + WHO 2023 regulatory standards |
| **Analytical Storytelling** | Dashboard answers questions a consumer, parent, and policymaker would ask |
| **Data Integrity** | Cross-validated pricing, protein, and safety data across 3 platforms |
| **Analytics Pane** | Reference lines (MPS threshold at 5g) with labels and custom styling |
| **Power Query** | Column data type enforcement to prevent DAX measure failures |

</div>

---

## 👤 About the Author

<div align="center">

### Yogesh Gadekar (YSG)
*Data Analyst · Power BI · SQL · Excel · DAX · India*

<br/>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/yogesh-gadekar)
[![GitHub](https://img.shields.io/badge/GitHub-Follow-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/GADEKAR328)
[![Portfolio](https://img.shields.io/badge/Portfolio-View%20Projects-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)](https://github.com/GADEKAR328)

<br/>

> 🟢 *Open to Data Analyst · Business Analyst · BI Developer · Power BI Developer opportunities*

</div>

---

## ⭐ Support This Project

<div align="center">

If this dashboard gave you ideas, helped your own project, or showed you something new about DAX or Power BI —

**drop a ⭐ on this repo**

It helps others in the Indian data analytics community find this work and supports open public-health data projects.

[![Star this repo](https://img.shields.io/badge/⭐%20Star%20This%20Repo-F2C811?style=for-the-badge)](https://github.com/GADEKAR328/Protein-Supplement-Analytics-Dshboard-P-BI)
[![Share on LinkedIn](https://img.shields.io/badge/Share%20on%20LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/sharing/share-offsite/?url=https://github.com/GADEKAR328/Protein-Supplement-Analytics-Dshboard-P-BI)

</div>

---

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=0,2,2,5,30&height=140&section=footer&text=Thank%20you%20for%20visiting!&fontSize=22&fontColor=ffffff&fontAlignY=55&animation=fadeIn" width="100%"/>

*Data sources: Amazon.in · Flipkart · FSSAI · FDA · NSF · Informed Sport · Brand websites*

*Built with Power BI Desktop | India Market | 2024–25 | Yogesh Gadekar (YSG)*

</div>
