BMI Calculator

Overview

This is a simple and interactive Body Mass Index (BMI) calculator implemented in C++. The program takes user input for weight (in pounds) and height (in inches), calculates the BMI, and provides feedback based on the BMI value.

Features

Color Formatting: Outputs are styled using ANSI escape codes for better readability.

Looping Functionality: Allows users to calculate BMI for multiple entries without restarting the program.

Feedback: Provides customized advice based on the BMI value.

How to Use

Compile the Code:
Use a C++ compiler like g++ to compile the program. For example:

g++ -o bmi_calculator bmi_calculator.cpp

Run the Program:
Execute the compiled file:

./bmi_calculator

Input Details:

Enter your weight in pounds.

Enter your height in inches.

View Results:

The program will display your BMI and categorize it as follows:

Underweight: BMI < 18.5

Normal: BMI 18.5 – 24.9

Overweight: BMI ≥ 25

Continue or Exit:

After displaying the results, you can choose to calculate another BMI or exit the program by responding with 'Y' or 'N'.

Example Interaction

==============================================
            BMI CALCULATOR
==============================================
Please enter your weight (pounds): 150
Please enter your height (inches): 68

Your BMI is: 22.80
You are normal!

Would you like to enter the information again? (Y/N): N

Okay, see you next time!

Code Explanation

Libraries Used

iostream: For standard input and output.

iomanip: For formatting output (e.g., setting precision).

cmath: For mathematical calculations like pow.

limits: To clear the input buffer.

Key Functions

BMI Calculation:

bmi = (weight / pow(height, 2)) * 703;

This formula converts weight (in pounds) and height (in inches) to BMI.

User Feedback:
Based on the calculated BMI, the program categorizes the user as underweight, normal, or overweight and provides corresponding advice.

Loop:
A do-while loop ensures the program can be used multiple times in a single session.

ANSI Escape Codes

\033[0m: Resets formatting.

\033[1m: Bold text.

\033[32m: Green text (for positive feedback).

\033[31m: Red text (for warnings).

\033[33m: Yellow text (for advice).

\033[36m: Cyan text (for headers and prompts).

Notes

Ensure your terminal supports ANSI escape codes for proper color formatting.

The BMI formula used in the program is based on the imperial system.
