# NIRPS-data-handling-session

## Clone the current repository

First create a folder in a convenient place before cloning it. Let's assume, to five an example, that we create the [place_a_name_here] folder on the home directory. From the terminal:

``` bash
>>> cd [place_a_name_here]
```
And then clone the repository:

``` bash
>>> git clone https://github.com/EduardoCristo/NIRPS-data-handling-session.git
```

Finally navigate to the repository folder:

``` bash
>>> cd NIRPS-data-handling-session
```

## Create a conda environment and install the required packages

Lets start by creating a NIRPS_dhs conda environment running python 3.9

``` bash
>>> conda create --name NIRPS_dhs python=3.9
```

Next activate it

``` bash
>>> conda activate NIRPS_dhs
```

Install the requirements for all the packages we will be using.

``` bash
>>> pip install -r requirements.txt
```

## Make NIRPS_dhs appear as a kernel in jupyter

Start to install ipython to the NIRPS_dhs environment

``` bash
>>>  conda install -c anaconda ipykernel
```

Make the connection between the environment and jupyter
``` bash
>>> python -m ipykernel install --user --name=NIRPS_dhs
```

Start jupyter and check if NIRPS_dhs is one of the available kernels.

****
****

## Install Romain Allart's telluric correction tool
The tool itself does not require anything more to install other than the requirements, which were dealt already. The telluric correction is performed inside the folder structure provided in the repository.

Clone the repository to the folder created before:

``` bash
>>> git clone https://github.com/RomainAllart/Telluric_correction.git
```

And that is it! You can now test if it is running properly with the provided example:

``` bash
>>> cd Telluric_correction
>>> python run_telluric_correction.py
```

****
****


## Install Line-by-line code


Clone the repository to the folder created before

``` bash
>>> git clone https://github.com/njcuk9999/lbl
```
Go to the Line-by-line code folder

``` bash
>>> cd lbl
```

Install it

``` bash
>>> pip install -U -e .
```
#
## Data to download

Click the below links to download the required data:

[NIRPS APERO data](https://udemontreal-my.sharepoint.com/personal/charles_cadieux_1_umontreal_ca/_layouts/15/onedrive.aspx?id=%2Fpersonal%2Fcharles%5Fcadieux%5F1%5Fumontreal%5Fca%2FDocuments%2FPROXIMA%5FNIRPS%5FHE%5FAPERO%2Etar&parent=%2Fpersonal%2Fcharles%5Fcadieux%5F1%5Fumontreal%5Fca%2FDocuments&ga=1)

[NIRPS DRS data](https://udemontreal-my.sharepoint.com/personal/charles_cadieux_1_umontreal_ca/_layouts/15/onedrive.aspx?id=%2Fpersonal%2Fcharles%5Fcadieux%5F1%5Fumontreal%5Fca%2FDocuments%2FPROXIMA%5FNIRPS%5FHE%5FESO%2Etar&parent=%2Fpersonal%2Fcharles%5Fcadieux%5F1%5Fumontreal%5Fca%2FDocuments&ga=1)