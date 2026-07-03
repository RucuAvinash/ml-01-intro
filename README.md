# ml-01-intro

[![Workflow Guide](https://img.shields.io/badge/Pro--Guide-pro--analytics--02-green)](https://denisecase.github.io/pro-analytics-02/workflow-b-apply-example-project/)
[![Python 3.14](https://img.shields.io/badge/python-3.14%2B-blue?logo=python)](./pyproject.toml)
[![MIT](https://img.shields.io/badge/license-see%20LICENSE-yellow.svg)](./LICENSE)

> Professional Python project: characterizing machine learning.

## Project Description

This project focuses on learning to find good data problems in a dataset,
and learning when machine learning (ML) might be helpful.

We learn to characterize:

- supervised (when we pick a target to predict)
- unsupervised (no target, just exploring, e.g. clustering)

In this project, we pick a dataset and a target.

If the target is:

- a discrete category column, we know it is a classification problem
- a continuous numeric column, we know it is a regression problem.

Some numbers are actually categories, for example a rating of 1, 2, 3.
May be better characterized as a category / discrete variable.

## Example Notebook + Your Notebook

Keep the example notebook as it is.
Either copy it or use it to build a new notebook that ends in _yourname.
See [docs/your-files.md] for more.

Links:

- [ml_01_rucu.ipynb](notebooks/ml_01_rucu.ipynb)

## Working Files

You'll work with these areas:

- **data/raw** - raw data for exploration (only if you add a dataset)
- **docs/** - project narrative and documentation
- **src/mlstudio/** - the app is an example; run only (no need to modify)
- **notebooks/** - interactive analysis
- **pyproject.toml** - update authorship & links
- **zensical.toml** - update authorship & links

## Instructions (pro-analytics-02)

Follow the
[step-by-step workflow guide](https://denisecase.github.io/pro-analytics-02/workflow-b-apply-example-project/)
to complete:

1. Phase 1. **Start & Run**
2. Phase 2. **Change Authorship**
3. Phase 3. **Read & Understand**
4. Phase 4. **Modify**
5. Phase 5. **Apply** <mark>(optional for Module 1)</mark>

**Completing Phases 1-4 is the goal for Module 1.**
Phase 5 is optional in Module 1.
If your environment is working well and you still have some time, you might try it.



## Command Reference

<details>
<summary>Show command reference</summary>

### In a machine terminal (open in your `Repos` folder)

After you get a copy of this repo in your own GitHub account,
open a machine terminal in your `Repos` folder:

```shell
# Replace username with YOUR GitHub username.
git clone https://github.com/RucuAvinash/ml-01-intro

cd ml-01-intro
code .
```

### In a VS Code terminal

These are listed for convenience.
For best results, follow the detailed instructions in
[pro-analytics-02 guide](https://denisecase.github.io/pro-analytics-02/).

```shell
uv self update
uv python pin 3.14
uv lock --upgrade
uv sync --extra dev --extra docs --upgrade

uvx pre-commit install
uvx pre-commit autoupdate

# git add all files and auto fix them as much as possible while working
git add -A
uvx pre-commit run --all-files
# repeat if changes were made
uvx pre-commit run --all-files

# run the example module to verify the environment (.venv/)
uv run python -m mlstudio.app_case

# run common chores: format, lint, run checks and tests...
uv run ruff format .
uv run ruff check . --fix
uv run python -m pyright
uv run python -m pytest
uv run python -m zensical build

# save progress after every major change (customize the commit message)
git add -A
git commit -m "update"
git push -u origin main
```

</details>

## Notes

- Use the **UP ARROW** and **DOWN ARROW** in the terminal to scroll through past commands.
- Use `CTRL+f` to find (and replace) text within a file.
- You do not need to add to or modify `tests/`. They are provided for example only.
- Many files are silent helpers. Explore as you like, but nothing is required.
- You do NOT need to understand everything; understanding builds naturally over time.

## Troubleshooting >>>

If you see something like this in your terminal: `>>>` or `...`
You accidentally started Python interactive mode.
It happens.
Press `Ctrl+c` (both keys together) or `Ctrl+Z` then `Enter` on Windows.


## Findings and Visuals

Take screenshots of your charts and provide them here with a discussion.
In Markdown, display a figure by using:
an exclamation mark immediately followed by square brackets containing a useful caption
immediately followed by parentheses containing the relative path to your figure.
Note: When you start typing the path with a dot (.) for "here, in this directory",
the IDE may help complete the path.

In your custom project, follow this example, but

- your figures and narrative should reflect your work,
- this `README.md` should include your commands, process, and visuals, and
- `docs/index.md` should include your narrative.

Remove unnecessary instructional comments in your custom files.

These are from the example app used to test the .venv/.
If possible, replace these to present interesting results from your custom project:

![Provide a Useful Caption] ![alt text](ML_Figure1.jpeg)

![Provide a Useful Caption]![alt text](ML_Figure2.jpeg)

![Provide a Useful Caption]![alt text](ML_Figure3.jpeg)
## Project Documentation

Additional project instructions, terms, and notes:
Made Technical modification to the .ipynb file- changed the classification model to a regression model by changing the target column to numeric field .
Ran all the cells and analyzed the results changed from classification to regression model.
Applied Skills to a new Problem by adding new data to the existing hours_scores data and predicting the model after running the python file with the following command
`uv run python -m mlstudio.app_rucu`
Ran the customized python file using the below command:
`uv run python -m mlstudio.app_rucu`


[docs/index.md](docs/index.md)

## Citation

[CITATION.cff](./CITATION.cff)

## License

[MIT](./LICENSE)
