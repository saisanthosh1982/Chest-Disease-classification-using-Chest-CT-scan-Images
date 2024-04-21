# Chest-Disease-classification-using-Chest-CT-scan-Images

## Required Commands


**1. Creating new GitHub repositry:**

Creating a new github repository is always a good idea while working with new project to store different versions of the project in a remote server so that if there are any bugs or any problems we can retrieve back the older version to the local system.

**2. Clonning the repository to local system:**

When we create a new github repository we need to clone the repository to local system to start working on the project, so we will be using git clone method to clone the repository to local system.

```bash
git clone https://github.com/username/repositry.git
```

In order to get the link click on the green coloured code option, be in the HTTPS option and then copy the link that is avalible there, It will be helping you further by the above command.

**3. Creating new conda environment:**

It is always a good practice to create a new conda environment when we are working on a new project, which helps us to have error free code and clash with the existing versions of libraries, so here we will be creating a new conda environment as follows:

```bash
conda create -n cti python=3.8 -y

conda activate cti
```
* conda create- helps to create conda environment.
* -n is used to create a new conda environment.
* cti- name of the environment we are going to use.
* python=3.8 - creating a new conda environment with python version 3.8
* -y is used to confirm the changes to the new conda environment.
* conda activate cti -  activates the new created repositry.

**4. Installing required libraries:**

Assuming you know what are the libraries you want to install for the project, you can add all of them to requirements.txt file and use the following command:
It is ok if you dont know what are the libraries you want to install, you can still add them at the last but it is a good practice to do that when you want your project to be run without any errors at production level.

```bash
pip install -r requirements.txt
```
**5. Making commits from local system:**

If you want to make the commits from the local environment with git-bash you can use the following commands:

```bash
git add .

git commit -m "Updated"

git push origin main
```
Else you can use the VS code itself to make the commits with few integrations, search stackoverflow for the configuration.

**6. Will be updated soon:**
Ml-flow dagshub URL
* Go to dagshub and create a clone of your github repository then click on remote select experiments click on usinng mlflow tracking copy and paste here as below
```bash
MLFLOW_TRACKING_URI=https://dagshub.com/saisanthosh9154/mlflow_demo.mlflow \
MLFLOW_TRACKING_USERNAME=saisanthosh9154 \
MLFLOW_TRACKING_PASSWORD=8ac56ed76aac52d4377524ba8ae2dc307ac4bdc3 \
python script.py
```

Connect dagsHub URL using bash terminal 
```bash
export MLFLOW_TRACKING_URI=https://dagshub.com/saisanthosh9154/mlflow_demo.mlflow

export MLFLOW_TRACKING_USERNAME=saisanthosh9154

export MLFLOW_TRACKING_PASSWORD=8ac56ed76aac52d4377524ba8ae2dc307ac4bdc3
```