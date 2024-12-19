# **Applied Statistics assessment**

This Github repo contains the project repo completed as part of the Applied Statistics module done as part of the Higher Diploma in Computing (Data Analysis) at ATU Galway. 
This assessment is broken into tasks and project. 

## **Assessment**
This repo contains two Jupyter Notebooks; *tasks.ipynb* for tasks and *project.ipynb* for the project with further information provided below in their respective sections. 

### **Tasks**
For the Tasks project tasks.ipynb - this Jupyter Notebook contains Tasks 1 - 4
- Task 1: Permutations and Combinations - Lady Tasting Tea.
      
    Suppose we alter the Lady Tasting Tea experiment to involve twelve cups of tea. Six have the milk in first and the other six having tea in first. A person claims they have the special power of being able to tell whether the tea or the milk went into a cup first upon tasting it. You agree to accept their claim if they can tell which of the six cups in your experiment had the milk in first. Calculate, using Python, the probability that they select the correct six cups. Suppose, now, you are willing to accept one error. Once they select the six cups they think had the milk in first, you will give them the benefit of the doubt should they have selected at least five of the correct cups. Calculate the probability, assuming they have no special powers, that the person makes at most one error.  

- Task 2: numpy's Normal Distribution - Generating normally distributed data

    In this task you will assess whether *numpy.random.normal()* properly generates normal values. To begin, generate a sample of one hundred thousand values using the function with mean 10.0 and standard deviation 3.0. Use the *scipy.stats.shapiro()* function to test whether your sample came from a normal distribution. Explain the results and output. Plot a histogram of your values and plot the corresponding normal distribution probability density function on top of it.  

- Task 3: t-Test Calculation - t-test calculation using python and *scipy.stats*

    Consider the below dataset containing resting heart rates for patients before and after embarking on a two-week exercise program. Calculate the t-statistic based on this data set, using Python. Compare it to the value given by *scipy.stats*.

    **Table 1:** Data for test
    |Patient ID	   |0	|1	|2	|3	|4	|5	|6	|7	|8	|9| 
    |:-------------|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
    |Before        |63	 |68   |70   |	64 |74	 |67   |70	 |57   |66	 | 65  |
    |After	       |64	 |64   |68   |	64 |73   |	70 |72   |	54 |61   |	63 |

- Task 4: ANOVA - Type II Error

    In this test we will estimate the probability of committing a type II error in specific circumstances. To begin, create a variable called no_type_ii and set it to 0. Now use a loop to perform the following test 10,000 times.

    1. Use *numpy.random.normal* to generate three samples with 100 values each. Give each a standard deviation of 0.1. Give the first sample a mean of 4.9, the second a mean of 5.0, and the third a mean of 5.1.

    2. Perform one-way anova on the three samples and add 1 to no_type_ii whenever a type II error occurs.

### **Project**
THe *project.ipynb* Jupyter Notebook contains the project aspect of this module analyzing the [PlantGrowth R dataset](https://vincentarelbundock.github.io/Rdatasets/index.html) available from RDatasets. 

Your task is to perform t-tests and ANOVA on this dataset while describing the dataset and explaining your work. In doing this you should:
- Download and save the dataset (`PlantGrowth.csv`) to your repository.
- Describe the data set in your notebook.
- Describe what a t-test is, how it works, and what the assumptions are.
- Perform a t-test to determine whether there is a significant difference between the two treatment groups `trt1` and `rt2`.
- Perform ANOVA to determine whether there is a significant difference between the three treatment groups `ctrl`, `trt1`, and `trt2`.
- Explain why it is more appropriate to apply ANOVA rather than several t-tests when analyzing more than two groups.

## **Development and Environment**
Both the tasks and projected were completed in [`Visual Studio Code`](https://code.visualstudio.com/) using python (V3.11) though [`Anaconda`](https://www.anaconda.com/). No additional python modules needed as this was done using modules available within Anaconda, however the `requirements.txt` file shows the python modules used as part of this assessment. 

## **Repository structure** 
This repository has the below structure 

```
/applied_statistics_assessment
├── /PlantGrowth.csv        # File used for project           
├── project.ipynb           # Project Jupyter Notebook
├── .gitignore              # .gitignore file
├── README.md               # README.md file 
├── requirements.txt        # python dependencies
├── img/                    # directory of image files used in repo
└── tasks.ipynb             # Tasks Jupyter Notebook
```


## **Running this repository**
This repo can be run in two ways;
- Running locally
- Github codespaces

### **Running this repository locally** 

To be run locally, the user must have [`Anaconda`](https://www.anaconda.com/) (or similar) and an IDE ([`Visual Studio Code`](https://code.visualstudio.com/) was used for this project). 

1. Clone the repository
```
$ git clone https://github.com/EllenMcG/applied_statistics_assessment.git
```

2. Open the required Jupyter Notebook (`project.ipynb` and/or `tasks.ipynb`) in `Visual Studio Code` and run

#### **Dependencies** 
Note: if user is not using an IDE but just using python then the dependencies need to be installed first listed in the `requirements.txt` file below.

``` 
$ pip install -r requirements.txt
```

### **Running this repositry on Github Codespaces**

GitHub Codespaces is an online IDE that allows you to run your project in a cloud-based environment without needing to set up anything on your local machine. Here's how to get started:

1. Open the repository in GitHub Codespaces:
- Go to the repository's page on GitHub.
- Click the green Code button.
- Select Open with Codespaces.

2. Start the Jupyter Notebook in Codespaces:
Once your Codespace is ready:
- Open the integrated terminal in GitHub Codespaces.
- Make sure your virtual environment is activated (if you're using one). If not, you can skip this step.
- Open the required Jupyter Notebook (`project.ipynb` and/or `tasks.ipynb`)  in `Visual Studio Code` and run 
