Run instructions — COMPAS Audit Notebook

1) Create a virtual environment (recommended) and activate it.

PowerShell (Windows):

```powershell
python -m venv .venv; .\.venv\Scripts\Activate.ps1
```

2) Install dependencies

```powershell
pip install -r assignment\requirements.txt
```

If `aif360` fails to install via pip on Windows, consider using WSL, conda, or follow the AIF360 installation notes from the project repository:
https://github.com/Trusted-AI/AIF360

3) Launch Jupyter Notebook / Lab

```powershell
jupyter notebook assignment\audit_compas_notebook.ipynb
```

4) In the notebook
- If package imports fail, run the installation cell (or run the pip install line at the top of the notebook).\n- Run cells in order.\n- Review visualizations and the generated metrics in output cells.

Notes
- If you have trouble installing `aif360` on Windows, use a conda environment (Linux subsystem or cloud runtime is usually easier).\n- The notebook uses a simple logistic regression for demonstration; replace with more advanced models or AIF360 mitigation algorithms as needed.\n