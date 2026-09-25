# QM-Solver

An interactive web application for simplifying Boolean functions using the **Quine-McCluskey Tabular Method**, with **K-Map visualization** and **Truth Table Verification**.

## Features

* Supports **SOP (Sum of Products)** using Minterms
* Supports **POS (Product of Sums)** using Maxterms
* Supports **1 to 10 variables**
* Supports **Don't Care conditions**
* Allows choosing different **variable naming sets**
* Shows the solution **step by step** using the Tabular Method
* Generates a **Prime Implicant Chart**
* Provides **K-Map visualization for 2 to 5 variables**
* For more than 5 variables, the **Tabular Method and Truth Table Verification** remain available
* Verifies the optimized result using a **Truth Table**
* Supports **Dark Mode and Light Mode**
* Allows copying the **final Boolean expression**
* Allows printing the results or saving them as **PDF**

## Technologies Used

* HTML
* CSS
* JavaScript

## How to Use

1. Select the form type:

   * **SOP** – Sum of Products (Minterms)
   * **POS** – Product of Sums (Maxterms)

2. Select the number of variables from **1 to 10**.

3. Choose the desired **Variable Names Set**.

4. Enter the primary terms:

   * Minterms for SOP
   * Maxterms for POS

5. Optionally enter **Don't Care** terms.

6. Click **Run Tabular Method & K-Map**.

7. View the generated results, including:

   * Initial grouped table
   * Iteration tables
   * Prime Implicant Chart
   * K-Map representation for 2–5 variables
   * Truth Table Verification
   * Optimized Final Expression

8. Use **Copy Expression** to copy the final Boolean expression.

9. Use **Print Report / PDF** to print the results or save them as a PDF.

## Variable Support

The solver supports up to **10 variables**.

For example, the first variable naming set can use:

`A, B, C, D, E, F, G, H, I, J`

The second naming set uses variable names based on:

`V, W, X, Y, Z`

with additional variables used when more than 5 variables are selected.

## K-Map Support

The application provides K-Map visualization for:

* 2 variables
* 3 variables
* 4 variables
* 5 variables

For functions with more than 5 variables, the K-Map is not generated. Instead, the application displays a note explaining that the **Tabular Method and Truth Table Verification** are still fully operational.

## About the Algorithm

The **Quine-McCluskey algorithm** is a tabular method used to simplify Boolean functions and obtain optimized Boolean expressions.

The application groups terms according to their binary representations, combines terms that differ in one bit, identifies prime implicants, and generates a **Prime Implicant Chart** to help obtain the optimized result.

## Verification

After simplifying the Boolean function, the application generates a **Truth Table Verification Matrix** that compares:

* The original Boolean function
* The optimized function
* The resulting status for each input combination

This helps verify that the optimized expression matches the original function.

## Live Demo

🔗 https://fatmamohamed07.github.io/QM-Solver/

## Project Structure

The project is built as a client-side web application using:

* `HTML` for the structure
* `CSS` for styling and themes
* `JavaScript` for the Quine-McCluskey algorithm, K-Map generation, Prime Implicant Chart, and Truth Table Verification.
