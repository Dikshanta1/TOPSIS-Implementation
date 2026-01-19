# TOPSIS Implementation using Python

## Objective
The objective of this project is to implement the **TOPSIS (Technique for Order Preference by Similarity to Ideal Solution)** method to:

- Rank multiple alternatives based on multiple criteria  
- Analyze the effect of different weights and impacts on decision-making  
- Provide a clear and structured implementation suitable for academic evaluation  

---

## Methodology
The TOPSIS algorithm implemented in this project follows these steps:

1. Load and validate the input dataset  
2. Normalize the decision matrix  
3. Apply weights to represent the importance of each criterion  
4. Determine the ideal best and ideal worst solutions  
5. Compute Euclidean distances from ideal solutions  
6. Calculate TOPSIS scores  
7. Rank alternatives based on TOPSIS scores  

An alternative with a **higher TOPSIS score** is considered better.

---

## Results
- A ranked output table is generated containing:
  - **TOPSIS Score**
  - **Rank**
- Rank 1 represents the most preferred alternative  
- Results are exported to a CSV file for further analysis or submission  

---

## Input Validation Handled
The implementation strictly follows assignment requirements and validates:

- Correct number of command-line parameters  
- Handling of *File Not Found* exceptions  
- Input file must contain **three or more columns**  
- From the second to last columns must contain **numeric values only**  
- Number of **weights**, **impacts**, and **criteria columns** must be equal  
- Impacts must be either **'+' (benefit)** or **'-' (cost)**  
- Weights and impacts must be **comma-separated**  

Execution stops immediately if any validation fails.

---

## How to Run (Command-Line)

### Command Format

python topsis.py inputFileName Weights Impacts resultFileName

### Example

python topsis.py data.xlsx "1,1,1,1,1" "+,+,-,+,+" result.csv


## How to Run (Jupyter / Google Colab)
1. Open topsis.ipynb in Jupyter Notebook or Google Colab
2. Upload the input Excel file (data.xlsx)
3. Run all cells sequentially
4. View the TOPSIS scores and rankings in the output table

## Tools & Technologies Used

- Python
- Pandas
- NumPy
- Jupyter Notebook
- Google Colab
- GitHub

## Conclusion
This project demonstrates a complete and validated implementation of the TOPSIS method using Python.
It follows all prescribed academic constraints and provides a reliable approach for multi-criteria decision-making problems.

## Author
Developed as part of an academic assignment to demonstrate the practical implementation of the TOPSIS algorithm.
