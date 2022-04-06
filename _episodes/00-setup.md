---
title: "Setup"
teaching: 0
exercises: 10
questions:

objectives:
- "Install Anaconda"
- "Download the python jupyter notebook file"
- "Open jupyter notebooks"
---

To participate in this workshop, you will need to have the Anaconda distribution of Python installed on your computer, or you may use Anaconda on the UIC virtual labs to launch Jupyter notebooks. You will also need to download the code file used for this workshop. See instructions below for these steps. 


## Code Files
### Workshop Code:
Please download the following code to follow along with the workshop:  
[Python Code Part 1](../files/Intro_Python_Code_Part1.ipynb) - used for part 1/day 1  
[Python Code Part 2](../files/Intro_Python_Code_part2.ipynb) - used for part 2/day 2

### Practice Code:
[Part 1 practice exercise](../files/worksheet_1.ipynb) - implement concepts learned in part 1 (day 1).  
[Part 1 exercise solution](../files/worksheet_1_solution.ipynb) - solution for practice exercise

[Part 2 practice exercise](../files/Intro_Python_Exercise_part2.ipynb)

[Part 2 exercise solution](../files/Intro_Python_Exercise_part2_solutions.ipynb) - solution for practice exercise part2


## Software setup
We will be using Jupyter notebook for this workshop. We install the Anaconda navigator. Anaconda is an open source distribution, which provides the easiest way to code in python, especially for data science.

{% include install_instructions/python.html %}
{% include install_instructions/virtual_lab.html %}

{% comment %}
### INSTALLATION:
__For Windows Users:__

1) Go to the following link: https://www.anaconda.com/products/individual
2) Click on the download button and wait for the .EXE file to be downloaded.
3) Double click on the dowloaded file to launch the installer.
4) Click Next.
5) Read the Licensing agreement and click "I agree".
6) Select "Just me" and click "Next"
7) Select a destination folder to install Anaconda and click the Next button.
8) Uncheck the add Anaconda to your PATH environment variable and check the register Anaconda as your default Python. Click Install
9) Click Next
10) Click Next. There is an option to install Pycharm. However, we do not need this tool for this workshop.
11) After a successful installation you will see the “Thanks for installing Anaconda” dialog box

__For Mac Users:__

1) Download the macos installer by going to the following link https://www.anaconda.com/products/individual and clock on download
2) Open the file my double clicking on it and start the installation.
3) Answer the prompts on the screen.
4) Installation type, select "Install for me only"
5) Click on continue.
6) After a successful installation you will see the “Thanks for installing Anaconda” dialog box
{% endcomment %}
 
 
### Launching Jupyter on Anaconda    

We can use Anaconda Navigator to access Jupyter and other tools(pyCharm etc) provided in Anaconda.     

__For Windows Users:__    
1. Click Start    
2. Search and select Anaconda Navigator from the menu.    
3. Once the Navigator opens up. Select Jupyter Notebook from the tools available.  
4. Jupyter will open up on a new tab in the browser.   
5. Navigate to the required destination.  
6. Click on new - > Notebook  
7. The script file opens up.  

__For Mac Users:__  
1. Click Launchpad and select Anaconda Navigator. Or, use Cmd+Space to open Spotlight Search and type “Navigator” to open the program.  
2. Once the Navigator opens up. Select Jupyter Notebook from the tools available.  
3. Jupyter will open up on a new tab in the browser.   
4. Navigate to the required destination.  
5. Click on new - > Notebook  
6. The script file opens up.

> ## NOTE:  
> While we are using jupyter notebook for the purpose of this workshop, we can use any text editor to write our program and run it using terminal/command prompt.
> To do so-
> 1. Open the command prompt/terminal and type pip install python3
> 2. Once the installation is complete, open any editor and type you code in it. Make sure you save the file with a .py extension.
> 3. Go to the command prompt/terminal and navigate to the filder where the file is saved.
> 4. type python3 "name of the file".py   
{: .callout}

