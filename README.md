# Simulations to estimate π
[![made-with-python](https://img.shields.io/badge/python-3.8.8-blue)](https://www.python.org/)
## Project Description
Pi is an irrational number, and thus it can never be written as a fraction of two whole numbers, and its decimal expansion therefore does not terminate or repeat. No exact value of Pi has been found. There are only approximations of Pi which have been recorded which sometimes result in an error when performing precised calculations. This project is aimed at estimating π using some randomness via Monte Carlo Methods. We also aim to look at convergence of different methods estimating Pi analysed using different numbers of sample points during simulation procedure and then averaging over these independent approximations. I’ll implement eight versions to do this.

## How to Install and Run the Project

### Install

* Since the script uses Anaconda Distribution of python, user must first install Anaconda according to their system requirements [from here](https://www.anaconda.com/products/distribution). The instructions to install can be [found here](https://docs.anaconda.com/anaconda/install/#). After the installation, open Anaconda Navigator and click Launch on the [Jupyter Notebook](https://docs.jupyter.org/en/latest/) application.
  
  <img width="773" alt="image" src="https://user-images.githubusercontent.com/105721523/180783465-7d3752a8-66ce-45b6-b845-9143029e197f.png">
  
  *Note that Jupyter python script has an extension of **.pynb** unlike **.py** for other python scripts. So the user should open the script using Jupyter Notebook.*

* Afterwards, the user must clone the Git repository on the local machine. On the GitHub, navigate to the repository, select the ***Code*** button (in green) and then select the button beside the link to copy the repository link.

 <img width="773" alt="image" src="https://user-images.githubusercontent.com/105721523/180784692-7e05de36-1c07-4865-b71b-e68ed54dab46.png">
 
 * If you chose to copy the link, then open a terminal window and navigate to the directory where you want to copy the repository using `cd PATH-TO_DIRECTORY`. Type git clone then paste the link to the repository you copied earlier.
 
  ```
   git clone URL-OF-REPOSITORY
  ```
  
  * Lastly, go to the Jupyter Notebook launched earlier and navigate to the directory where you copied the repo or where you downloaded the ZIP. Select the project folder and double click on the ***ACM40960_Project_21200378.pynb*** file to open it in Jupyter Notebook.


### Running the Script

The Jupyter file should be run chronologically. Failure to do so may result in errors. To execute a code block, select the block (a blue bar is displayed on the left of the code block), then either press `Shift + Return` or press the *play button (RUN)* on the toolbar above. Also, from the Cells Menu you can select Run Cells to run the code block.

*Note: Some of the code blocks take longer to run. The runtimes (in seconds) for Additional Simulations are as follows:*

   <img width="150" height = "200" alt="image" src="https://user-images.githubusercontent.com/105721523/180786323-a15dfb66-13f3-44d6-a63d-30318840c057.png">

## Packages

All the following packages used in this project come with the Anaconda Distribution and doesn’t require any additional installation.

```
from time import time
import time
import math
import fractions
from scipy import *
import pandas as pd
import numpy as np
import seaborn as sns
import matplotlib.pyplot as plt
import matplotlib.ticker as ticker
import plotly.graph_objects as go
import plotly.express as px
```

## Functional Blocks

| **Functions**   | Task            |
| --------------- | --------------- |
| random()       |  This function uses Lehmer Random Number Generator to generate values between (0,1)| 
| resetSeed()    |  This function takes an argument of a real number and reset or initialise the state of random number generator.| 
| calcPi()       |  This function stores the simulated values of pi in global variables, calculate mean and standard deviation of the values and also calculate the difference between the average of simulated values and the true pi. It returns a data-frame with mean, standard deviation and difference from true pi for each seed and each N.|
| errbars()      |  This function takes mean and standard deviation and list of number of iterations obtained from calcPi() to generate error-bars for each N and each seed.|
| linearPlot()   |  This function takes in the data-frame returned by calcPi() as an argument to generate a linear plot between difference and N.|
| semiLogPlot()  |  This function takes in the data-frame returned by calcPi() as an argu- ment to generate a point plot between difference and N with y-axis (axis of difference/error) on logarithmic scale.|
| logLogPlot()   |  This function takes in the data-frame returned by calcPi() and list of number of iterations as arguments to generate a point plot between difference/error and N with both axes on logarithmic scale.|
| Archimedes()   |  |
| Buffon()       |  |
| AreaOfCircle() |  |
| funcAvg()      |  |
| MCInt1()       |  |
| MCInt2()       |  |
| MCInt3()       |  |
| MCInt4()       |  |
| probFunc()     |  |
| calculateProbability()    | |

## Results  



  ![final](https://user-images.githubusercontent.com/105721523/181045867-4c616132-259b-4eca-a7dd-becae810b0a7.png)




