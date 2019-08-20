# Machine Learning Workshop

## Install Python
### Windows & Mac OSX:
1. Download Miniconda (Python 3.7, 64bit) 
.exe Installer for Windows (Check "Add Anaconda to my PATH environment variable" (Windows only))
.pkg Installer for Mac
https://docs.conda.io/en/latest/miniconda.html

2. Open Anaconda Prompt or CMD
Install Jupyter Notebook & virtualenv
```sh
conda install jupyter
pip install virtualenv
```

3. Create a new virtual environment and activate it
```sh
virtualenv ml-workshop-env

# on windows
call ml-workshop-env\Scripts\activate

# on mac
source ml-workshop-env/bin/activate
```

4. Clone github repo & install package requirements
```sh
git clone https://github.com/nkaenzig/ml-workshop.git
cd ml-workshop
pip install -r requirements.txt
```


### Linux:
1. Check if Python is already installed
```sh
python3
```
If this opens a python prompt, skip step 2 and proceed with step 3 in section (Windows & Mac OSX)

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


