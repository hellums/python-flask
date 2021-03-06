# OVERVIEW
This project uses a [subset of IMDB listed movies](https://github.com/hellums/lacey-bacon/blob/root/watchlist.txt) and actors from Hallmark original movies, romantic comedies, mysteries, and dramas. Backend HTML/CSS rendering comes via Flask/Jinja2, with a Sqlite database.

This repo is a Flask version of a CLI program (lacey-bacon) and uses data generated from it, and includes a Docker container. All websites and images shown here belong to the original copyright holders and are used for academic and demonstration purposes only. Source and derived data is [publicly available and courtesy of IMDB](https://www.imdb.com/interfaces/).

## VIDEO WALKTHROUGH
[<img alt="romcomWeb video walkthrough" width="600px" src="images/romcomWeb.jpg" />](https://screencast-o-matic.com/watch/c3e6FLVFY4v)

## Mac/Linux instructions for command-line version:
(NOTE: Requires python version 3 and pip. The series of commands below will download the app, create a virtual environment, install python, pip, and the app's prerequisites in that virtual environment, and run the app using recently compiled data. 
  - >git clone https://github.com/hellums/python-flask.git
  - >cd python-flask
  - >python -m venv env
  - >source env/bin/activate
  - >pip install -r requirements.txt
  - >python romcomWeb.py
  - >in a web browser tab, go to http://localhost:5000/ 

## Windows instructions for command-line version:
If using VSC, a DOS command prompt terminal is highly recommended, NOT PowerShell.

Perform same steps as above, except replace the "source env/bin/activate" command in step 4 with 
  - >env\Scripts\activate (or activate.bat)

## To build a local Docker container (on port 5500): 
- > docker build -t python-flask .

## Clean Up
- To get everything back to normal and remove files, type deactivate, then remove the python-flask directory. Your system will be back to normal, as before the test.
