# Team NYC Carbon Emissions App

Team NYC's project is a dashboard that provides informative analytics on maritime traffic and CO2 emissions.

## Project Structure
The project loosely follows a model-view-controller structure. 

#### Views
"Views" are plotly components that usually take a dataframe as an input and process them to store into a plotly figure

#### Model
The model is where data structures and ORM logic is stored to query the necessary data. This can be either through a pickle, json, or postgres connection

#### Controller
The controller would be the application logic that weaves together functions from the views and the models. Logic here shouldn't be too complex, and anything that can be written as a function or something larger should be tossed into the util/ directory.

## Getting Started

### Running the app locally

First create a virtual environment with conda or venv inside a temp folder, then activate it.

```
virtualenv venv

# Windows
venv\Scripts\activate
# Or Linux
source venv/bin/activate

```

Clone the git repo, then install the requirements with pip

```

git clone https://github.gatech.edu/nzaker3/teamnyc-project
cd app
pip install -r requirements.txt

```

Run the app

```

python app.py

```


## Built With

- [Dash](https://dash.plot.ly/) - Main server and interactive components
- [Plotly Python](https://plot.ly/python/) - Used to create the interactive plots

