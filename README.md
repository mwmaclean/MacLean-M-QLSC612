# MacLean-M-QLSC612 Practical Assignment
Contributors : Michèle MacLean

This exercise is part of the BrainHack QLSC6112 course and was designed to demonstrate how researchers can (easily) produce false positives or inflated prediction rates via **p-hacking**.

# Objective
We were asked to generate a new variable (named `partY`) of random noise, add it to the existing `brainsize.csv` dataset and find associations using the existing variables in `brainsize.csv`. Then, we needed to generate a second, new variable (named `partY2`) also of random noise (with a different random seed) and re-run the same previous associations or prediction models using this new variable as the outcome measure.

The variables included in the data set are: 1) Gender, 2) Full Scale IQ (FSIQ) 3) Verbal IQ (VIQ), 4) Performance IQ (PIQ), 5) Height, 6) Weight 7) Brain size (MRI_Count)

## Summary
There is increasing evidence that elevated body mass index (BMI) in healthy adults could influence the anatomical structure and function of the brain. To our knowledge, previous research has been misled by including socially awkward people in the sample. We compared groups of neurotypical individuals for BMI against brain size (MRI_Count), measured using magnetic resonance imaging, and performance IQ. We show that within a reasonable threshold of social activity, measured by the infamous partY score, BMI is associated with brain size and performance IQ. Perhaps, based on these findings, in order to further explore the causality between these variables, a dieting study allowing increase in BMI count could show anatomical and functional brain changes for socially active people. ''Qu'ils mangent de la brioche!'' - Marie Antoinette

## Steps to get started
These following steps will allow you to get a copy of the workflow up and running on your computer.
1. You may clone this repo by copying the following in your terminal
`git clone https://github.com/mwmaclean/MacLean-M-QLSC612.git`

2. Install required packages
`$ pip install -r requirements.txt`

This mainly inludes the following:
* pandas
* numpy
* matplotlib
* seaborn
* scipy.stats
* statsmodels

3. Run the jupyter notebook myanalysis.pynb which is in the 'Code' directory. 
If you do not already have Jupyter, you can also: [Install Here](https://jupyter.org/install)

# Expected outputs 
## Included Figures
* Combined scatter plots of all variables:
    **Fig 1.** Scatter plots of variables 'FSIQ', 'VIQ', 'PIQ', 'Weight', 'Height', 'MRI_Count', 'partY' and 'partY2'
* A figure showing the evoluton of p-values for both PIQ and brain size (MRI_Count) along with the choice of the partY threshold:
    **Fig 2.** Evolution of p-values for MRI_Count and PIQ
* A linear regression showing the association of BMI with PIQ and brain size (MRI_Count) for individuals with a high partY score: 
    **Fig 3.** a) MRI_Count as a function of BMI b)PIQ as a function of BMI

## Outputs for statistical tests
* Descriptive statistics of all variables, including variables 'partY' and 'partY2' (e.g. count, mean, standard deviation)
* Regression results for the 'partY' variable
* Regression results for the second 'partY2' variable

# Tools
This project relies on the following tools:
* GitHub for forking a repository, renaming & assembling all the resources.
* Python version 3.7.6, used with miniconda
* Jupyter Notebook to create and document the code and analyze data 
* Data visualization tools (e.g. Numpy, Matplotlib, Seaborn).
* Visual Studio Code to edit text

# Acknowledgments
Thanks to the BrainHack School for providing the instructions and necessary tools for this assignment.

# License
This assignement is licensed under: Creative Commons Zero v1.0 Universal