# ChessQuest
### *Or: How Chess Data Knows Me Better Than I Do*

A personal data visualisation project built around my own chess games, played on [chess.com](https://www.chess.com) between January and May 2026.

Instead of looking outward for improvement, more tutorials, more theory, I decided to turn the lens on myself and ask: *what does my data actually say about how I play?*

---

## Requirements

To run the notebook, install the required packages by uncommenting and executing the first cell:

```
!pip install pandas numpy matplotlib plotly kaleido requests
!plotly_get_chrome
```

Plotly renders are set to `"colab"` throughout. If you are running the notebook in a local Jupyter environment, replace `pio.renderers.default = "colab"` with `pio.renderers.default = "svg"` in each cell.

## Files

**`ChessQuest.ipynb`**
The main Jupyter Notebook. Contains the full analysis, from data gathering and cleaning to visualisation and interpretation. Structured around two core questions: an exploratory overview of my general statistics, and a knowledge discovery investigation into whether losing streaks affect my accuracy.

**`chess_games.csv`**
The cleaned dataset exported from the chess.com API. Contains 166 games spanning January–May 2026, with attributes including game outcome, player ratings, accuracy scores, opening, colour played, and temporal metadata.

**`visualisation.jpg`**
A summary visualisation of the project's key findings, designed in Canva. Intended as a standalone visual overview of the most actionable insights from the analysis.

---

## Tools & Transparency

Data was retrieved via the [chess.com Public API](https://www.chess.com/news/view/published-data-api) using Python. Visualisations in the notebook were coded with the assistance of Claude (Anthropic). All written analysis and interpretations are my own. The summary visual was designed independently in Canva.
