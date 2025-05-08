# uni-ml-project

## Dev env setup

1. Download the data from the web.
1. Clone the repository on local machine.
1. Create a virtual enviroment.
1. Install dependencies.

```bash
wget https://ec.europa.eu/eurostat/cache/website/microdata/public-microdata-lfs/RO_PUF_LFS.zip
mv RO_PUF_LFS.zip ./data/raw/
unzip RO_PUF_LFS.zip

python -m venv venv

Set-ExecutionPolicy Unrestricted -Scope Process # Scope based, must be run each time cause windows is trash.

source ./venv/scripts/activate
.\venv\Scripts\activate

python -m pip install --upgrade pip

pip install -r requirements.txt
```

## Structure

```
uni-ml-project/
├── .venv/
├── data/                  # Datasets
│   ├── raw/               # Original datasets
│   └── processed/         # Cleaned datasets
├── notebooks/             # Jupyter notebooks
├── outputs/               # Model outputs
│   ├── models/            # Model saves
│   ├── plots/             # Plots for visualisation
│   └── reports/           # Metrics
├── project_requirements   # Requirements handed by the professor.
├── requirements.txt       # All installed packages
├── README.md              # Project overview and instructions
└── .gitignore             # Files to ignore in git (if you use git)
```
