# Stack Overflow Developer Survey Analysis

An exploratory data analysis (EDA) of the **Stack Overflow Annual Developer Survey** dataset, built in a single Jupyter notebook (`ultimateProject.ipynb`) using `pandas`, `numpy`, `matplotlib`, and `seaborn`.

The goal is to dig into the raw survey responses and answer practical questions about who developers are, what they use, and how satisfied they are with their work.

## Questions Explored

**Chapter 1: Who are developers?**
- Which countries have the most respondents?
- What's the average age of developers?
- What education levels are most common (globally and in India specifically)?
- How satisfied are developers with their jobs, and which industries report the highest satisfaction?
- Which databases and cloud platforms are most used/admired among developers?
- Which industries employ the most developers, and which `DevType` (Data Engineer, Data Scientist, Analyst, Support Engineer, etc.) reports the highest job satisfaction?

**Chapter 2: Tools & tech stacks**
- What are the most common technology stacks among Data Engineers (office/communication tools, admired tech, etc.)?
- (In progress) Do developers with 10+ years of experience use AI tools more or less than beginners?

## Key Findings

**Top responding countries** — the US, Germany, and India lead by a wide margin:

![Top responding countries](assets/top_countries.png)

- Most respondents fall in the **25–34 age group**.
- A **Bachelor's degree** is the most common education level among developers overall, and also specifically among developers in India.

**Job satisfaction** — most developers rate their satisfaction fairly high (7-9 out of 10):

![Job satisfaction distribution](assets/job_satisfaction.png)

- Developers who rate job satisfaction **8/10 or higher** are concentrated in the **Software Development** industry.
- Analysis by `DevType` (Data Engineer, Data Scientist, Data/Business Analyst, Support Engineer) breaks down satisfaction distributions and commonly used office/communication stacks per role.

## Tech Stack

- Python 3
- pandas
- numpy
- matplotlib
- Jupyter Notebook

## Dataset

This analysis uses the **[2025 Stack Overflow Annual Developer Survey](https://survey.stackoverflow.co/)** results (`results.csv`) — roughly **50,000 rows and 192 columns**.

The raw CSV (~134 MB) is **not included in this repo** since it exceeds GitHub's comfortable file size limits. To reproduce the analysis:

1. Download the 2025 survey results from the [Stack Overflow Insights page](https://survey.stackoverflow.co/).
2. Place `results.csv` somewhere on your machine.
3. Update the file path in the first data-loading cell of the notebook:
   ```python
   df = pd.read_csv('path/to/your/results.csv', low_memory=False)
   ```

## Getting Started

1. Clone the repo:
   ```bash
   git clone https://github.com/SumitGo/StackOverflowAnalysis.git
   cd StackOverflowAnalysis
   ```
2. Install dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn jupyter
   ```
3. Download the Stack Overflow Developer Survey CSV and update the file path in the notebook.
4. Launch Jupyter and run the notebook:
   ```bash
   jupyter notebook ultimateProject.ipynb
   ```

## Project Status

This is an active/ongoing exploration notebook — some cells are scratch work or left incomplete (e.g. the "which skill gets paid most" and "AI usage by experience level" questions are yet to be answered). Contributions or suggestions for further questions to explore are welcome.

## Author

[SumitGo](https://github.com/SumitGo)
