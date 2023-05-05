How to install [BabyAGI] to Ubuntu 22.04

You will need to take care of some prerequisites (python3-venv isnt strictly necessary but for the sake of keeping things clean on the system lets use virtualenvs for python): 

```apt install make g++ python3-pip python3-venv python3-dev```

get the code from github:

```git clone https://github.com/yoheinakajima/babyagi.git```

create venv and install requirements

```
cd babyagi
python3 -m venv .venv/
. .venv/bin/activate
pip install -r requirement.txt
```

You might hit issues with installing hnswlib with pip, use `export HNSWLIB_NO_NATIVE=1` and rerun `pip install -r requirement.txt`
