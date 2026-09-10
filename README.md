
## Setup

Requires **Python 3.14** (see `.python-version`).

```bash
# 1. create the virtual environment
python3 -m venv .venv

# 2. install dependencies
.venv/bin/pip install -r requirements.txt          # Windows: .venv\Scripts\pip install -r requirements.txt

# 3. register the Jupyter kernel
.venv/bin/python -m ipykernel install --user --name sta1 --display-name "Python (STA1 .venv)"
```


## Adding a dependency

```bash
.venv/bin/pip install <package>
```

Then add the package name to `requirements.txt` (one per line, alphabetical) and commit it.
After pulling changes, re-run step 2 to sync. The `.venv/` folder is git-ignored — never commit it.
