# Machine Learning Workshop

## Install Python
### Windows & Mac OSX & Linux:
1. Install Python
- If you use linux: check section below, then proceed with step 2<br />
- If you use Windows/Mac;
Download Miniconda (Python 3.7, 64bit) <br />
.exe Installer for Windows (Check "Add Anaconda to my PATH environment variable" (Windows only))<br />
.pkg Installer for Mac<br />
https://docs.conda.io/en/latest/miniconda.html<br />

2. Open a terminal & install Jupyter Notebook & virtualenv
```sh
# windows/mac
conda install jupyter
conda install virtualenv

# linux
pip3 install jupyter
pip3 install virtualenv
```

3. Create a new virtual environment and activate it
```sh
virtualenv ml-workshop-env

# on windows
call ml-workshop-env\Scripts\activate

# on mac/linux
source ml-workshop-env/bin/activate
```

4. Clone github repo & install package requirements
```sh
git clone https://github.com/nkaenzig/ml-workshop.git
cd ml-workshop

# on windows
pip install -r requirements.txt

# on mac/linux
pip3 install -r requirements.txt
```


### Linux:
1. Check if Python is already installed
```sh
python3
```
If this opens a python prompt, skip step 2 and proceed with step 2 in section (Windows & Mac OSX)

2. Install Python
```sh
sudo apt-get update
sudo apt-get install python3.7
```

## Add kernel to Jupyter
```sh
# on windows
call ml-workshop-env\Scripts\activate

# on mac
source ml-workshop-env/bin/activate

pip install ipykernel
ipython kernel install --user --name=ml-workshop-env
```


