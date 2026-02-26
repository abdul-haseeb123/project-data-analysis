# Project Data Analysis

This project supports two environment setup methods:

- **Pip + `requirements.txt`**: [requirements.txt](requirements.txt)
- **Conda + `environment.yml`**: [environment.yml](environment.yml)

> Use one primary method to avoid dependency conflicts.

## 1) Setup with Pip (`requirements.txt`)

### Create virtual environment

#### Windows (PowerShell)

```powershell
python -m venv .venv
```

#### macOS/Linux

```bash
python3 -m venv .venv
```

### Activate virtual environment

#### Windows (PowerShell)

```powershell
.\.venv\Scripts\Activate.ps1
```

#### macOS/Linux

```bash
source .venv/bin/activate
```

### Install dependencies

```bash
pip install --upgrade pip
pip install -r requirements.txt
```

---

## 2) Setup with Conda (`environment.yml`)

### Create environment from file

```bash
conda env create -f environment.yml
```

### Activate environment

```bash
conda activate data-analysis-proj
```

### (Optional) Update environment after changes

```bash
conda env update -f environment.yml --prune
```

---

## 3) Install dependencies manually (if needed)

### Using conda

```bash
conda install <package-name>
```

### Using pip

```bash
pip install <package-name>
```

If you are inside a conda environment and need a pip-only package, run `pip install` after `conda activate data-analysis-proj`.

---
