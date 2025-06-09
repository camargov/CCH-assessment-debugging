## Programmer Assessment Q4

This repository contains a broken web app built with Dash. Please follow the tasks below.

Tasks:

1. Clone this repo to your machine.
2. Fix missing dependencies and fill authors section in `pyproject.toml`.
3. Fix bugs prevent the app `main.py` from running.
4. Change port the app ruuning on to `10030`.
5. Commit you changes.
6. Update `README.md` with a instruction
   1. Assuming the user has a fresh minimum Linux installation with no python.
   2. Setup python and virtual environment for this app, use the fixed `pyproject.toml`.
   3. How to run this app and how to access it without portforwarding.
7. Push all the changes to your own repository on Github, and provide a link to your own repo in your submission in the last.

### Installation for Linux

1. Install Python and pip

```
sudo apt install python3 python3-pip python3-venv -y
```

2. Check installastion was successful by checking python version

```
python3 --version
```

3. Create and activate a virtual environment

```
python3 -m venv venv
source venv/bin/activate
```

4. Install dependencies for python project

```
pip install .
```

5. Run the app

```
export FLASK_APP=main.py
flask run --host=0.0.0.0 --port=10030
```

6. Access without port forwarding
   Find the IP

```
ip a | grep inet
```

Then access the app using:

```
http://...
```
