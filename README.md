# Statistical Analysis of IPL Player Performance Using Advanced Computational Methods

## Paper Link
https://www.ijcaonline.org/archives/volume186/number30/statistical-analysis-of-ipl-player-performance-using-advanced-computational-methods/

## Overview

This project provides a detailed statistical evaluation of player performance in the Indian Premier League (IPL) from 2008 to 2024, utilizing advanced metrics and Python-based data analysis. Traditional cricket statistics like batting average and strike rate often fall short in capturing the nuances of the fast-paced T20 format. This study applies Bayesian methods (Damodaran, 2006) to adjust batsmen scores, introduces the Combined Bowling Rate (CBR) metric (Lemmer, 2002) based on the harmonic mean of key bowling stats, and employs **stochastic dominance** to compare players across multiple matches for a deeper performance insight.

## Author

**Nirat J Patel**\
B.Tech – Information Technology\
L.D. College of Engineering, Ahmedabad\
22itnir068@ldce.ac.in

## Abstract

Cricket in India is rapidly expanding, largely due to the IPL, now valued at nearly $16.4 billion. This growth has spurred opportunities in Sports Analytics. The IPL, a franchise cricket tournament with player auctions, requires informed selections within budget constraints to build balanced teams. This paper analyzes player performance using IPL match and ball-by-ball datasets (2008–2024) from Kaggle. Batting performance is assessed with adjusted scores and stochastic dominance, while bowling performance leverages the CBR metric, combining average, economy, and strike rate. Python libraries (NumPy, pandas, Matplotlib) facilitate the analysis.

**Keywords**: Data Analysis, Indian Premier League, Player Performance, Cricket Analytics

## Introduction

Sports analytics has transformed how teams evaluate performance and strategize, with the IPL standing out as a leading T20 league globally. The high-stakes, fast-paced T20 format demands accurate performance metrics, benefiting both teams and fans seeking deeper insights. Traditional stats like batting average or bowling economy often overlook nuances, such as "not-out" biases. Building on Damodaran (2006) and Lemmer (2002), this project adapts ODI statistical methods to the T20 context, offering a robust Python-based framework for IPL analysis.

## 📁Project Structure

```
Statistical-Analysis-IPL-Performance/
├── data/                   # Raw datasets (matches.csv, deliveries.csv)
├── notebooks/              # Jupyter notebooks (EDA, analysis, visualization)
│   ├── eda.ipynb           # Exploratory data analysis
│   ├── main_analysis.ipynb # Metric computations and visualizations
├── figures/                # Output plots (stochastic dominance, performance charts)
├── paper.pdf               # Published research paper
├── requirements.txt        # Python dependencies
├── README.md               # Project overview (this file)
└── .gitignore              # Ignore temporary files
```

## Key Techniques

- **Bayesian Batting Score Adjustment**: Estimates "not-out" innings using prior data (Damodaran, 2006).
- **Stochastic Dominance Comparison**: Plots cumulative probabilities to identify dominant players.
- **Combined Bowling Rate (CBR)**: Harmonic mean of bowling average, economy, and strike rate (Lemmer, 2002).

## Datasets Used

- **IPL Matches**: Match-level data (2008–2024) with 1095 entries.
- **IPL Deliveries**: Ball-by-ball data (2008–2024) with 260,920 rows.

## Requirements

Main libraries used:

- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `jupyter`

## How to Run

1. Clone the repository:

   ```bash
   git clone https://github.com/YOUR_USERNAME/ipl-player-analysis.git
   ```
2. Navigate to the folder:

   ```bash
   cd ipl-player-analysis
   ```
3. Start Jupyter Notebook:

   ```bash
   jupyter notebook
   ```
4. Open notebooks from the `notebooks/` folder for analysis and visualization.

## Insights

- Virat Kohli stochastically dominates Rohit Sharma based on adjusted batting scores.
- Lasith Malinga, Rashid Khan, and Anil Kumble lead the CBR leaderboard for bowlers with 100+ overs.
- Damodaran’s Bayesian model effectively corrects "not-out" biases.

## Conclusion

Advanced metrics like the Bayesian approach and CBR provide deeper insights beyond traditional stats. While effective, these methods have limitations, such as not fully capturing contextual factors (e.g., fitness, match situations). Future work could integrate additional variables like all-rounder skills and psychological traits for a holistic evaluation, enhancing cricket analytics in India’s talent-rich landscape.

## 🔗 References

\[1\] Wood, G. H. (1945). Cricket scores and geometric progression. *Journal of Royal Statistical Society*, 108, 12–22.\
\[2\] Damodaran, U. (2006). Stochastic dominance and analysis of ODI batting performance: The Indian cricket team, 1989–2005. *Journal of Sports Science and Medicine*, 5, 503–508.\
\[3\] Lemmer, H. H. (2002). The combined bowling rate as a measure of bowling performance in cricket. *South African Journal for Research in Sport, Physical Education and Recreation*, 24(2), 37–44.\
\[4\] Kenney, J. F. & Keeping, E. S. (1954). *Mathematical Statistics* (3rd ed.). New York, NJ: D. van Nostrand.\
\[5\] IPL matches dataset. https://www.kaggle.com/datasets/patrickb1912/ipl-complete-dataset-20082020?select=matches.csv\
\[6\] IPL ball-by-ball dataset. https://www.kaggle.com/datasets/patrickb1912/ipl-complete-dataset-20082020?select=deliveries.csv\
\[7\] Fernández Ponce, J. M., et al. (2022). An Application of Stochastic Dominances in Sports Analytics. *Economía Aplicada*, 40(1). https://doi.org/10.25115/eea.v40i1.7002 
