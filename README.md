# INFORM-Pilot
Data transformations for data extracted from Qualtrics surveys for SQL / Tableau Ingestion. Three survey are converted to Pandas dataframes, transofrmed wide to long, and merged to a single dataframe.

These datasets are stored in a number of csvs on our team's Google Drive. This repo contains scripts to join these datasets as well as analyses performed with the data.

## Getting Started

### Prerequisites

First, you'll need Python 3.7. We recommend using `pyenv` to get this (as well as other versions of Python).

Then you'll need Jupyter Notebook. You can find directions on how to get that [here](https://jupyter.org/install). They recommend downloading Anaconda to get it, but we suggest using `pip` if you're already using `pyenv` to manage your python versions.

Then you'll want to clone this repo and `cd` in to it:

```bash
git clone https://github.com/GSA/INFORM-Pilot.git
cd INFORM-Pilot
```

We use `pipenv` for a virtual environment. You can find instructions on installing that [here](https://pipenv.readthedocs.io/en/latest/install/#installing-pipenv).

Once you've got `pipenv` installed, you can start up the virtual environment using:

```bash
pipenv install
```

Next, activate the Pipenv shell:

```bash
pipenv shell
```

This will spawn a new shell subprocess, which can be deactivated by using `exit`.

One of the required packages you just installed is `ipykernel`. We use this to create a kernel that uses our virtual enivronment for the Jupyter Notebook:

```bash
ipython kernel install --user --name=wb2
```

At this point, you can start jupyter with `jupyter notebook`. Open this notebook and select the kernel (wb2) that you just created.

### Getting the Data

The data files are too large to keep in the repository, so we keep them in our team's google drive.

#### INFORM Survey Data

This is the survey data collectedin Qualtrics, which included study participants. Download the INFORM data [here](https://drive.google.com/drive/u/0/folders/1NQgTDiHXiJ_IRqkrWOfA9cE_ysR8dgac). There's a csv for each survey. Once you've downloaded those files, move them into the `data/INFORM-Pilot` directory.

## License

This project is licensed under the Creative Commons Zero v1.0 Universal License - see the [LICENSE.md](https://github.com/GSA/wb2/blob/master/LICENSE) file for details
