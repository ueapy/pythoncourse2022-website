# Installation instructions

For this course you will need to have Python installed on your laptop, inlcuding some extra packages. Follow the instructions below to set up your Python environment. Make sure you do this do this **before** the course, including running the test as below. There will be an **installation party** advertised in the invite email.
Feel free to contact [Jenny at Cefas](mailto:jennifer.graham@cefas.co.uk) or [Eliza at UEA](mailto:e.karlowska@uea.ac.uk) if you have any problems with the installation (but better do an internet search first!)
Note: The course is designed in Python 3.8 but even if you have a different version installed, 3.8 will be installed when creating a conda environment in step 3 below.

## 1. Install Python distribution

For Cefas users: Anaconda is very likely to be discontinued at Cefas in favour of free alternatives such as Miniforge or Mamba. If you want to be ahead of the curve install [Miniforge3](https://github.com/conda-forge/miniforge) instead of Anaconda in point 1.1 and 1.2.

1.1. [Download Anaconda with Python 3 for your OS](https://www.anaconda.com/download/). If you have a Cefas laptop, it is better **not to install** the older version on the Cefas Software Centre.

1.2. Install it following [these instructions](https://docs.anaconda.com/anaconda/install/). Be sure to select install "just me" when prompted.

## 2. Download course materials
From friday before the course (4th of June) the material for the workshop can be downloaded as a [zip file](https://github.com/ueapy/pythoncourse2021-materials/archive/master.zip) or can be cloned from our [GitHub repository](https://github.com/ueapy/pythoncourse2021-materials). 


### Option 1: Download ZIP file (easier)
Download the materials as a [zip file](https://github.com/ueapy/pythoncourse2021-materials/archive/master.zip) and unpack it in a suitable directory, for example, in `Downloads` folder. Jump to [3. Create the environment](installation.md#3.-Create-the-environment).

### Option 2: Using Git (allows restoring originals after modifications)
#### 2.1. Install Git
If you don't have git version control system installed, you can install it following these instructions:
##### Linux
Use your package manager. For example, using aptitude you would run the following terminal command: `sudo apt-get install git`
##### Mac
* The XCode command line tools need to be installed.
* Install XCode if it isn’t already. XCode is available in the Mac App Store for free.
* Launch XCode and accept the license agreement.
* Quit XCode.
* Open a new terminal and run the command xcode-select --install
* Select install on the pop-up menu.
##### Windows
Download and install [Git for Windows](https://git-scm.com/downloads).

#### 2.2. Clone the repository
2.2.1. Open the command line (Git bash, terminal or cmd.exe)

2.2.2. (Linux or Mac, optional) Change to a suitable directory (e.g. `cd /home/yourname/Documents`)

2.2.3. Clone the repo by typing

```
git clone https://github.com/ueapy/pythoncourse2022-materials.git
```
This should create a local copy of the course materials in the current directory.

Windows-users, double check that it has been cloned in the directory you wanted.


## 3. Create the environment
3.1. Make sure Anaconda is installed and the course materials are downloaded

3.2. Open the command line (i.e., search "Terminal" on Mac Spotlight Seach; search "Anaconda prompt" on Windows start menu)

3.3. Navigate to the cloned / downloaded folder (using `cd` command), for example:

```
cd C:\Users\myname\Downloads\pythoncourse2022-materials\
```

3.4. Create the environment using `conda` package manager:

```bash
conda env create -f environment.yml
```
This will take some time depending on your Internet speed (<15 minutes).
If you get stuck try typing return or, failing this, creating the environment again.

## 4. Activate the environment
### Linux / Mac
If your default shell is NOT bash, first type `bash`. Activate the relevant environment by typing:
```bash
conda activate course2022
```
### Windows
Still in the command line (Anaconda prompt), type:
```
conda activate course2022
```

## 5. Test the installation (essential!)
From the terminal type:
```
python -c "import seaborn"
```
If you don't get any errors then your installation was sucessful.

## 6. Launch Jupyter
Once the environment is activated, type 
```
jupyter notebook
```
in the command line. This should open Jupyter Notebook in your browser. 

## Still having trouble?
If you are unable to install Anaconda Python on your PC, contact the [course organisers](index.md#registration-and-enquiries).
Another option: launch the course in the cloud! [![Binder](http://mybinder.org/badge.svg)](http://mybinder.org:/repo/ueapy/pythoncourse2022-materials). This requires no installation but progress and modifications won't be saved.
