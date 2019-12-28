# Conda Cheatsheet

>**NOTE:**
This tutorial is part of the series lead by Rachit Jain, an ex-Microsoft Software Engineer.<br/> 
With experience, you improve, but how many Senior Software Engineers are out there who share their complete journey of their growth?<br/>
Join Rachit in the journey to learn and master your technical skills and navigate into `Senior Software Engineering` roles, and becoming a 10x Developer.

Installation at https://docs.conda.io/en/latest/miniconda.html 

Watch the YouTube video for the demo [here](#videocomingsoon) on **Algorithms with Rachit**.

This is the list of `major Conda commands` that you would need while working as a Software Engineer.
- **Creating an environment**
  - Create an empty environment
    - ```bash
      conda create -n myfirstcondaenv 
      ```
  - Create conda environment with Python 3.7
    - ```bash
      conda create -n mysecondcondaenv python=3.7
      ```
  - Create conda environment from requirements.txt file
    - ```bash
      conda create -n myenv -f requirements.txt
      ```
- **Installing/Removing Packages**
  - Install from default channels into current environment
    - ```bash
      conda install scipy
      ```
  - Install from specific channel into current environment
    - ```bash
      conda install scipy --channel conda-forge
      ```
  - Install specific versions into specific environment
    - ```bash
      conda install scipy=0.15.0 curl=7.26.0 -n py34_env
      ```
  - Removing specific versions into specific environment
    - ```bash
      conda remove scipy=0.15.0 curl=7.26.0 -n py34_env
      ```
- **Searching for Packages**
  - Search for a package into default channels 
    - ```bash
      conda search scipy
      ```
  - Search for a package with specfic version
    - ```bash
      conda search python=3.9
      ```
  - Search for a package into specific channels only
    - ```bash
       conda search --override-channels  --channel mutirri iminuit
      ```
- **Listing packages in current environment**
  - Complete list of packages of current environment
    - ```bash
      conda list
      ```
  - Exporting the above list into a requirements.txt file
    - ```bash
      conda list --export > requirements.txt
      ```
  - Search for a specific package in current environment
    - ```bash
       conda list python=3.7
      ```
- **Other commands**
  - Listing all conda environments
    - ```bash
       conda env list
      ```
  - Delete an environment and everything in it
    - ```bash
       conda env remove -n myfirstenv
      ```
  - Conda information (conda version, about channels, etc)
    - ```bash
       conda info
      ```
  


For more cheatsheet commands, visit [this](https://docs.conda.io/projects/conda/en/4.6.0/_downloads/52a95608c49671267e40c689e0bc00ca/conda-cheatsheet.pdf).
