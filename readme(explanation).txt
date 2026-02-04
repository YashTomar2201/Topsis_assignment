TOPSIS - Multi-Criteria Decision Making Tool
This repository contains an implementation of the TOPSIS (Technique for Order of Preference by Similarity to Ideal Solution) algorithm.

This project was developed as part of an assignment to demonstrate how Python can be used to simplify complex decision-making processes, how to package logic for distribution, and how to deploy it as a web service.

What is TOPSIS?
Consider a scenario where you want to purchase a mobile phone. You have five options and need to compare them based on price, storage, camera quality, and design.

Price: Lower is better (Negative impact)

Storage: Higher is better (Positive impact)

Selecting the "best" option becomes difficult when criteria conflict. TOPSIS offers a mathematical solution to this problem. It calculates a score for each option based on its proximity to the "Ideal Best" value and its distance from the "Ideal Worst" value.

Project Overview
The project is organized into three primary components:

1. The Core Logic (Command Line Tool)
The foundational Python script (topsis.py) handles the mathematical computations.

Implementation Details:

Utilizes Pandas for reading CSV files and NumPy for efficient vector calculations.

Includes robust input validation (checking for file existence, verifying numeric columns, etc.) to prevent runtime errors.

Calculates the Euclidean distance for each row to generate a final "Topsis Score" and "Rank."

Usage:

Bash
python topsis.py data.csv "1,1,1,1,1" "+,+,-,+,+" result.csv