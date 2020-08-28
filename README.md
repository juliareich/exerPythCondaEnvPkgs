# Setting up Environments and Installing Packages Using Conda

## Summary of steps to complete

- [ ] Fork this repository so you have your own copy to work on.
- [ ] Clone the repository on your local machine. 
- [ ] Edit this README.md file on your machine.
- [ ] Run the Conda commands shown in the video and describe them in the table below.
- [ ] Push your changes to your GitHub repository.
- [ ] Submit a link to this GitHub repository in Canvas.

## 1. Fork & Clone this repository

* We did this in a previous assignment. Instructions are here: https://github.com/cmcntsh/N6806_Fall2020_DevNotes/blob/master/Projects/002%20-%20Practice%20Using%20Git%20and%20GitHub/README.md
* This can also be done directly in VSCode
  * Create a new folder on your machine where you want to put this repository if you don't already have one you want to use.
  * Copy the Clone or Download path for this repository from GitHub.
  * In VSCode from the command pallette (Ctrl-Shift-P) run Git: Clone
  * Paste the path into the path field which pops up
  * Select your new folder you created on your machine
  * A new folder for the repository with the repository files should be in the folder you selected showing in the Explorer window in VSCode on the left side.
  
## Edit your README.md file

* [ ] In an editor of your choice (i.e. VSCode) edit this README.md file to add the answers requested in the tables.

## Follow along with this tutorial

* Conda What and Why? (27 min): https://www.youtube.com/watch?v=23aQdrS58e0&list=PLG9A6ovzPqX6d9uWzx0UYN9pm0zzl5ofA&index=13&t=0s
  * He installs Miniconda. We will be using Anaconda. Don't install Miniconda.
  * Follow along with the rest of the tutorial.
  * Go ahead and create the environments as he creates them in the tutorial.

## Conda Concepts

* [ ] Describe the Conda concepts used in the video and listed in the table below.

|   Concept   |         Description or short answer         |
|     ---     |                     ---                     |
|What is the purpose of having different environments?     |(So that we can use Python to perform a variety of purposes.)|
|What is the default package manager in Python?            |(PIP)|
|How do you manage environments and packages in Anaconda?  |(by using Anaconda or Miniconda which uses Conda to manage both environments and packages)|
|`conda list`       |(lists packages installed on the computer)|
|`conda env list`       |(lists the environments available)|
|How do you keep your base environment unchanged?       |(we create a new environment in which we can install a different package without changing the base environment)|
|What is the link to the Conda cheat sheet? (link in video notes is broken)      |(https://docs.conda.io/projects/conda/en/4.6.0/_downloads/52a95608c49671267e40c689e0bc00ca/conda-cheatsheet.pdf)|
|`conda create --name XXXX`       |(creates a new environment)|
|`source activate XXXX`       |(activates the new environment)|
|`conda install YYYY`       |(installs a new package in the selected environment)|
|channels in Conda       |(describes the path Conda will search to see if the package is available)|
|`conda install -c ZZZZ YYYY`       |(installs a package from a different channel. One time only though, new channel is not available permanently)|
|`conda config --show channels`       |(allows you to see the channels available)|
|`conda config --add channels ZZZZ`       |(installs a channel in addition to the default channels. New channels are available in all environments)|
|conda-forge.org       |(a community led collection for conda packages. And packages which are only available through conda-forge)|
|`source deactivate`       |(source deactivate did not work. Conda deactivate deactivated the environment and returned me to my base)|
|`conda config --get channels`       |(shows the priority in which Conda will look for different channels)|

* After creating the environments he created in the video on your computer, what would the results of running the command `conda env list` look like with the da35 environment activated. Paste the output from your command prompt in the code block below.

```
#Paste your results here.

(da35) Julias-Air:~ juliareich$ conda env list
# conda environments:
#
base                     /opt/anaconda3
ai38                     /opt/anaconda3/envs/ai38
da35                  *  /opt/anaconda3/envs/da35
```
* What command would you use to remove the environments you created for this exercise from your computer?

```
#Type the command here.
In Anaconda Navigator I would select the environment and click remove.
Per the cheat sheet: conda env remove --name bio-env
```
