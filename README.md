# Array Assignment

A small, notebook-based Python assignment exploring common array/list operations. The repository currently contains one Jupyter notebook, `Array Assignement.ipynb` (the filename uses the spelling “Assignement”), with examples for duplicate detection, right rotation, in-place reversal, finding a maximum, and removing duplicates from a sorted list.

## Requirements

- Python 3
- Jupyter Notebook or JupyterLab

The notebook uses only Python's standard library; there is no separate dependency manifest.

## Setup

Create and activate a virtual environment if desired, then install Jupyter:

```bash
python3 -m venv .venv
source .venv/bin/activate       # Windows: .venv\Scripts\activate
python3 -m pip install notebook
```

## Run the notebook

From the repository directory, start Jupyter:

```bash
jupyter notebook
```

Open `Array Assignement.ipynb` in the browser and run the cells in order. Alternatively, open the repository in JupyterLab and run the notebook there. The notebook includes sample inputs and prints results for each exercise.

## Exercises in the notebook

1. Check an array for duplicate values (`dup_arr`).
2. Rotate an array to the right by *k* positions (`rotate`).
3. Reverse an array in place (`reverse`).
4. Find the maximum element (`maximum`).
5. Remove repeated values from a sorted array (`duplicates`).

These are learning examples, not a packaged library or a tested command-line application. Some functions mutate their list argument, and their current implementations have edge cases and correctness issues. For example, `dup_arr` checks whether each item occurs in the same list (which is always true for a non-empty list) rather than checking for another occurrence; `reverse` refers to a global `arr` instead of its parameter. Review and test the implementations before relying on them.

## Suggested improvements

- Correct duplicate detection and add tests for empty, singleton, and duplicate-free inputs.
- Make each function operate on its arguments consistently, and document whether it mutates the input or returns a new list.
- Cover boundary cases such as empty arrays, `k = 0`, `k` larger than the array length, and negative rotation counts.
- Add automated tests for all exercises and expected outputs.
- Consider renaming the notebook to `Array Assignment.ipynb` (or another consistently spelled name) and adding a small Python module if the solutions are to be reused outside Jupyter.
