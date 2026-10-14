# AGENTS.md

## Project overview
An applied-statistics project that explores the classic Iris dataset in a Jupyter notebook. The goal is to demonstrate good research, project management and statistics skills by completing this project in a organised, clear, concise and accurate manner.

## Setup
- Python 3.12.3
- Install dependencies: `pip install -r requirements.txt`
- Main libraries: `pandas`, `numpy`, `scipy`, `statsmodels`, `scikit-learn`,
  `matplotlib`, `seaborn`, `jupyter`
- Launch: `jupyter notebook`

## Project structure
- `problems.ipynb` — the main notebook
- `data/` — local copy of the dataset, if one is used (do not modify raw data files)
- `img/` — saved plots exported from the notebook
- `requirements.txt` — Python dependencies

## Data
- Load the dataset with `sklearn.datasets.load_iris(as_frame=True)`.
- 150 rows, 4 numeric features (sepal length/width, petal length/width, in cm)
  and 1 categorical target (species: setosa, versicolor, virginica).
- Never alter the original data in place; create new variables for transformed data.

## Notebook conventions
- Put all imports and settings in the first code cell.
- Set a random seed once at the top (e.g. `np.random.seed(42)`) so results are reproducible.
- Follow this section order, each with a Markdown heading:
  1. Problem 1: Exploring Petal Length
  2. Problem 2: Correlation Between Petal Length and Petal Width
  3. Problem 3: Comparing Species Using t-Tests
  4. Problem 4: Comparing the Species Using ANOVA
  8. Conclusions
- Before every analysis cell, add a Markdown cell explaining what is being done and why.
- After every result, add a short Markdown interpretation in plain language.
- Keep code cells short and focused; one idea per cell.
- The notebook must run cleanly with **Kernel → Restart & Run All**.

## Code cells
Code cells in notebooks should be short and with brief comments. Larger functions can usually be broken down into small functions. If a lot of code goes to one cell, you should explain the most important statements separately using code and markdown cells (e.g. 

Some of the statements in the function are complex, hence, you should explain them separately, as in the following few cells.

In the standard_deviation function, we use a list comprehension (Real Python: When to Use a List Comprehension in Python) to create a new list from data. The mean is subtracted from each value and the result is squared using the power operator **:).

## Style
Use clear, well-formatted LaTeX for mathematics.
Use short, self-contained code snippets.
Prefer concise explanations over long prose.
Prefer simple, clean examples that illustrate one idea at a time.
Avoid unnecessary abstraction or complexity.
Use consistent notation and terminology.
Show the mathematics and the corresponding computational implementation where useful.
Prioritise clarity, accuracy, and readability over completeness.

## Plots
- Every plot needs a title, labelled axes with units (cm), and a legend where relevant.
- Use a consistent colour for each species throughout the notebook.
- Save final figures to `img/` as PNG.

## Referencing
References should be included as hyperlinks. They should be placed where they are used, with context provided as to what they are and why they are relevant. The key is to keep them clear and easy to read.

For example, in a Markdown cell:

The `numpy.array` function ([see official documentation](https://numpy.org/doc/stable/reference/generated/numpy.array.html)) creates an array from a list or other data structure.

And in a code cell:

# The numpy.array function creates arrays from data structures.
# See: https://numpy.org/doc/stable/reference/generated/numpy.array.html
x = np.array([1, 2, 3])

## Code commenting


## Don't
- Don't leave cells with errors or unused experimental code in the final notebook.
- Don't add new libraries without listing them in `requirements.txt`.
- Don't change the analysis order or delete sections without asking.