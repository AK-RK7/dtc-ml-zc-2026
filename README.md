# dtc-ml-zc-2026
A free, hands-on course from Data Talk Club on building, evaluating, and deploying machine learning systems.

### Environment Setup

Install uv
powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"

Add uv to PATH
$env:Path = "C:\Users\Admin3\.local\bin;$env:Path"

Initialize the project
uv init

Create virtual environment
uv venv

Allow PowerShell scripts
Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy RemoteSigned

Activate virtual environment
.\.venv\Scripts\Activate.ps1

Install dependencies
uv add numpy pandas matplotlib scikit-learn seaborn jupyter ipykernel

Verify installation
uv run python -c "import numpy, pandas, ipykernel; print('Environment OK')"
