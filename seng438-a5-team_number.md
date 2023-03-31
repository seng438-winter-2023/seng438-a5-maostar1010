**SENG 438- Software Testing, Reliability, and Quality**

**Lab. Report \#5 – Software Reliability Assessment**
| Group \#:      |  14        |
| -------------- | ---------- |
| Student Names: |   Mary     |
|                |   Nicola   |
|                |   Tyler    |
|                |   Jaxon    |

# Introduction

# Assessment Using Reliability Growth Testing 

For our Reliability Growth Testing (RGT), we selected C-SFRAT as our preferred tool due to its user-friendly interface. However, we encountered compatibility issues with the initial data sets. To address this, we modified Failure Report 1 to comply with C-SFRAT's required format. We established a time interval of 1 hour and assumed that the failures were uniformly distributed.

To provide an example of our cleaned data set, let's consider the first hour. During this interval, 9 errors were recorded, hence the execution time per failure is 0.11 (in hours):

| T | FC  | E |
| - | -   | - |
| 1 | 9   | 0.11|

After running our data set through each model we decided to select two models to compare Geometric Mean (GM) with no covariate and Negative Binomial (Order 2) also with no covariate. The model comparsion can be found here. Additionally, we will be running the models on 66% of our subset, so we can gauge the accuracy of the predictions by predicting the last 4 intervals.

Time to Failure plot:


From the models the failure rate / mean time to failure (MTTF) are:

| Dataset       | Failure rate  | MTTF            |
|-              |-              |-                |
| original      | 42/12 = 3.5   | 1/3.5 = 0.2857  |
| GM(none)      | 45/12 = 3.75  | 1/3.75 = 0.267  |
| NB2(none)     | 42/12 = 3.5   | 1/3.5 = 0.2857  |

As we can see the NB2 model's prediction was very accurate. The GM's predicition was off and presumed more errors would have occured.


Intensity plot:

From the failure intensity plot we can see a general trend down in failure intensity per interval.

## Acceptable range of failure rate

The acceptable range of failure rates vary depending on the software. If the acceptable range of failure rate was below 4 then this dataset would be in the acceptable range. However, if a firm decided that 3 errors per hour was the cutoff then the dataset would be unacceptable.

# Assessment Using Reliability Demonstration Chart 

# Comparison of Results

# Discussion on Similarity and Differences of the Two Techniques

# How the team work/effort was divided and managed

# Difficulties encountered, challenges overcome, and lessons learned

# Comments/feedback on the lab itself
