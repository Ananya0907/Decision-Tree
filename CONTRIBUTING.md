# Contributing to ML Arena 3

This repo contains the Decision tree problem.

## Notebook Paths

- Exploration: `exploration/exploration.ipynb`
- Library: `library/training.ipynb`
- Scratch: `scratch/training.ipynb`
- Optimization: Use `library/training.ipynb` or `scratch/training.ipynb` based on issue scope.


## Track Guidelines

### Exploration

* Focus on data understanding and visualization
* Explain key insights clearly

### Library

* Use standard ML libraries
* Report key metrics

### Scratch

* Do not use ML libraries
* Use NumPy, pandas, Python only

### Optimization

* Improve an existing model
* Compare before and after results

## Required in All Tracks

- Work on exactly one issue per pull request.
- Keep changes limited to the assigned notebook path.
- Keep outputs, metrics, and plots visible.
- Include `Closes #<issue-number>` in the pull request description.

## Workflow

1. Fork this repository on GitHub.
2. Clone your fork and enter the repo folder:

```bash
git clone https://github.com/<your-username>/Decision-Tree.git
cd Decision-Tree
```

3. Create a branch:

```bash
git checkout -b <track>/decision-tree-<short-task-name>
```

4. Open the notebook in Colab, complete changes, and download the updated `.ipynb`.
5. Replace the same notebook file in local repo.
6. Commit and push:

```bash
git add exploration/*.ipynb library/*.ipynb scratch/*.ipynb
git commit -m "<clear message>"
git push origin <branch-name>
```

7. Open a pull request and include:

```text
Closes #<issue-number>
```

## Review Checklist

- Notebook runs top to bottom without errors.
- Outputs and metrics are visible.
- Explanations are short and clear.
- Track rules are followed.
- Changes are reproducible.
- For optimization issues, before vs after benchmark is included.

Keep submissions simple, focused, and readable.
