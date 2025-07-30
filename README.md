# STT_L3
CS 203: Software Tools & Techniques for AI
IIT Gandhinagar
Sem-II - 2024-25

________________________________________________________________

LAB 03

Total marks: 10
Submission deadline: 
Submission guidelines:
Code should be added to a GitHub repository, and the repository details should be shared.
Late submissions will be penalized 20% per day.
Google form submission link:

Note: By submitting this assignment solution you confirm to follow the IITGN's honor code. We shall strictly penalize the submissions containing plagiarized text/code.
________________________________________________________________

In this lab, we will focus on dataset annotation and inter-annotator agreement calculation. Annotation is a critical step in supervised learning workflows, especially for tasks involving natural language processing (NLP). You will learn how to use Label Studio, an open-source annotation tool, to annotate a given Hindi-English dataset. Next, we will calculate inter-annotator agreement, which measures the consistency of annotations provided by different annotators.

This lab is to be completed in teams of size 2 students. Each team will annotate the data and then compute the inter-annotator agreement scores.

Task 1: Environment Setup
Note: All commands must be executed on the Linux terminal, & screenshot has to be provided after each execution of the command, along with a sentence explanation of the command working.
Execute the “history -c && history -w” command. It should clear all the history of the specific user.
Execute the “history” command and take the screenshot.
Execute command “sudo apt list | grep -i python3.10”. If the package for Python 3.10 is installed, then it is removed. 

Download and install Python 3.10 using tarball.
Make Pip environment using newly installed python3.10
Install label studio using pip.
Open, Register, and Check Label Studio on the web browser.
Execute “history > user_history.txt.” Upload user_history.txt file on Git Hub.
Task 2: Annotating a Dataset Using Label Studio
Import NLP and CV datasets. 
Each team has to annotate 20 data points from both NLP and CV datasets. Team 1 will be taking data points from 0 to 19, Team 2 from 20 to 39, and so on.
Each member will annotate 20 data points given to the Team from both NLP and CV datasets. (i.e. Team of two members will have 2 annotations of the same data point)
For NLP, add the following POS TAGS:  "NOUN", "PROPN", "VERB", "ADJ", "ADV", "ADP", "PRON", "DET", "CONJ", "PART", "PRON_WH", "PART_NEG", "NUM", "X"
Perform POS for the NLP dataset. Check this link, having 5 examples of 
Annotation.
For CV, add the following tags for annotation: Trucks, No Trucks.
Perform Classification Tasks for Images containing trucks or not.
Task 3: Implementing Inter-Annotator Agreement
Export the annotations in either JSON or CSV files.
Using Pyt hon code, calculate Cohen’s Kappa & Fleiss Kappa.
Use Cohen’s Kappa for the NLP Dataset Task.
Use Fleiss Kappa for the CV Dataset Task. Get the third annotation from any other teams and then calculate the Fleiss Kappa.
Output the agreement score and interpret its significance.


Evaluation Criteria

Environment Setup  (20%)
Proper setup of Python.
Screenshots before and after command execution.
Providing history in text format. (Executing commands like “sudo” or “apt” in history (Other than the command given in task 1 - bullet point 2) or using root user will result in marks deduction)
Proper documentation along with single-sentence command information.
Dataset Annotation (40%)
Proper setup and use of Label Studio for dataset annotation.
Completeness and consistency of annotations.
Inter-Annotator Agreement Calculation (40%)
Calculate IAA using Cohen’s Kappa.
The clear output of agreement scores and meaningful interpretation of the results. Export the annotation done by all the members.
Code should be clean, modular, and well-documented.
Effective use of functions and structure for readability and maintainability.
