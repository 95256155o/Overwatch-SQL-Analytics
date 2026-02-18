# Overwatch Competitive Data Analysis & Outcome Prediction

### Project Overview
This project is a statistical study based on a dataset of 100 personal competitive matches in Overwatch 2 (North America, Solo Queue, DPS Role, Diamond 5 - Master 5 range).

The primary objective is to identify statistical correlations between scoreboard metrics and match outcomes. The project explores whether winning and losing teams exhibit distinct data patterns and if match results can be predicted solely based on "snapshot" data from the scoreboard (KDA, MIT, Damage, Healing) during a game.

### Research Hypothesis
Can the final outcome of a match (Win/Loss) be predicted by analyzing the scoreboard data of the participating teams?
*   Do winning teams share specific statistical characteristics regardless of the map or game mode?
*   Is there a "winning formula" visible in the raw numbers that transcends hero composition?
*   Can a snapshot of data at a specific timestamp determine which team is currently in the winning position?

### Dataset Specifications
The dataset consists of 100 manually tracked matches with the following variables:
*   **Match Context:** Date, Time, Duration, Map, Game Mode.
*   **Rank/Environment:** NA Region, Solo Queue, Diamond/Master Tier.
*   **Team Composition:** Hero selections for both allied and enemy teams.
*   **Scoreboard Metrics:** Kills, Deaths, Assists, Damage, Healing, and Mitigation (MIT) for all 10 players.

### Data Structure & Schema
The data is organized into a relational database to facilitate querying and pattern recognition. The schema links match environments (Maps) to performance metrics (Scoreboard).

[INSERT ENTITY RELATIONSHIP DIAGRAM (ERD) HERE]

### Analytical Goals
1.  **Pattern Recognition:** Identify if high variance in specific stats (e.g., support deaths vs. tank damage) correlates strongly with loss rates.
2.  **Snapshot Prediction:** Test if looking at the scoreboard at the 5-minute or 10-minute mark can accurately predict the final winner.
3.  **Composition Analysis:** Analyze if certain statistical thresholds are required for specific compositions to succeed in the Diamond-Master bracket.

### Current Status
*   Data collection for the initial N=100 sample set is complete.
*   SQL database construction and normalization are in progress.
*   Preliminary analysis of "Winning Team" statistical profiles is underway.

---
© 2025 Jesse Luo.
