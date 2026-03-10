# AI Usage Log — IIT414W Lab 0
**Student:** Darienn López Plaza · darlopezp  
**Date:** March 9, 2026  
**Tools used:** GitHub Copilot (Claude Sonnet 4.6)

---

## Interaction 1 — Section 3 VER vs NOR Variance Comparison (setup_check.ipynb)

**1. Context**  
Needed to replace a TODO cell comparing Verstappen and Norris fast-lap time variance using standard deviation.

**2. Prompt(s)**  
> "resolve this cell and explain me the solution." (cell selected: Section 3 variance comparison cell)

**3. Relevant Output**  
Generated code that filters `fast_laps` by driver, builds a summary DataFrame with `FastLaps`, `BestSec`, `MeanSec`, `StdSec`, and prints a dynamic interpretation sentence based on the sign of `diff_std`.

**4. Validation**  
Checked that `fast_laps` variable was already defined in the cell above; confirmed the column names matched. The interpretation sentence logic (more/less variance) was verified by reading the conditional.

**5. Adaptations**  
None — the variable names and logic matched the existing session data.

**6. Final Decision**  
Used as-is.

---

## Interaction 2 — Section 5 ML Taxonomy Table (setup_check.ipynb)

**1. Context**  
Needed to create a 3-row DataFrame mapping ML paradigms (Supervised, Unsupervised, RL) to F1 use cases and misuse risks.

**2. Prompt(s)**  
> "Generate the dataframe about the different types of ML models of this cell with a column for F1 use cases and missuse risk." (cell selected: Section 5 ML taxonomy TODO)

**3. Relevant Output**  
Generated a `pd.DataFrame` with three rows: Supervised (top-10 prediction, leakage risk), Unsupervised (circuit clustering, scaling artifact risk), and RL (pit stop optimization, single-season overfitting risk).

**4. Validation**  
Cross-checked each paradigm-to-use-case mapping against the ML Taxonomy markdown cell already in the notebook. Confirmed all three matched the course definitions.

**5. Adaptations**  
None needed.

**6. Final Decision**  
Used as-is.

---

## Interaction 3 — data_check.ipynb Full Structure

**1. Context**  
Needed to complete `data_check.ipynb` from scratch with four cells: FastF1 session load, Jolpica API query, and a markdown summary.

**2. Prompt(s)**  
> "i need to edit this notebook to get the next required structure: Cell 1 — Reproducibility Header… Cell 2 — FastF1 Session Load… Cell 3 — Jolpica API Query… Cell 4 — Data Shape Summary…"

**3. Relevant Output**  
- Cell 2: Code loading 2024 Bahrain Race with `session.load()`, printing session name, event, results shape, columns, and `session.laps.head()`.  
- Cell 3: `requests.get()` call to `https://api.jolpi.ca/ergast/f1/2024/driverstandings/`, printing status code, record count, and first 3 driver entries.  
- Cell 4: Markdown summarizing session choice, dataset shapes, and a surprising observation about lap data richness.

**4. Validation**  
Checked that the Jolpica URL matches the official endpoint from the course instructions. Verified `session.results.shape` and `session.laps.head()` use the correct FastF1 API calls from the existing course notebook.

**5. Adaptations**  
Cache path set to `../data/fastf1_cache` to match the pattern used in `setup_check.ipynb` and used the correct url.

**6. Final Decision**  
Used as-is with the adaptations

---

## Interaction 4 — README.md Setup Instructions

**1. Context**  
Needed to add step-by-step environment setup instructions to `README.md` for pip venv

**2. Prompt(s)**  
> "generate the step by step to create the environment from requirements.txt. Include the exact shell commands."

**3. Relevant Output**  
Numbered steps and exact shell commands, plus a verification step pointing to `setup_check.ipynb` and extra for conda that I don't use.

**4. Validation**  
Verified each command against standard Python.

**5. Adaptations**  
Delete the conda instructions, because this project doesn't use conda for envs.

**6. Final Decision**  
Used with the adaptations.
