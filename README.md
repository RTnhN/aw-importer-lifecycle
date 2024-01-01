aw-watcher-lifecycle
==================

This extension imports data from [lifecycle](https://apps.apple.com/us/app/life-cycle-track-your-time/id1064955217) by watching a folder for changes.

This watcher is currently in a early stage of development, please submit PRs if you find bugs!


## Usage

### Step 1: Install package

Install the requirements:

```sh
pip install .
```

First run (generates empty config that you need to fill out):
```sh
python aw-watcher-lifecycle/main.py
```

### Step 2: Enter config

You will need to add the path to the folder where you will add the csv files from lifecycle. You can also update the polling time.

### Step 3: Add the csv export to the folder

### Step 4: Restart the server and enable the watcher

Note: it might take a while to churn though all the data the first time or two depending on how long you have been using lifecycle. Once it is imported, it will not re-import the file (it will change the name of imported files) or re-import individual events since unique ids are given to the events based on the name, date, duration, and location.


