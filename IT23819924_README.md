# IT3040 – ITPM Assignment 1

## Transliteration Accuracy Testing (Option 1)

### Student Details

Student ID: IT23819924
Module: IT3040 – ITPM
Year/Semester: Year 3 – Semester 1

---

## Project Overview

This project evaluates the accuracy of the Sinhala Chat Transliteration system available at:
https://www.pixelssuite.com/chat-translator

The objective is to identify scenarios where the system fails to correctly convert Singlish (chat style Sinhala written in English letters) into proper Sinhala text.

---

## Objectives

Identify 50 negative test cases where transliteration fails
Cover all 24 Singlish input types specified in the assignment
Automate testing using Playwright
Analyze system weaknesses based on results

---

## Testing Approach

 Designed 50 test cases focusing on incorrect transliteration scenarios
 Each test case includes:

  Input (Singlish text)
  Expected Sinhala output
  Actual output (generated automatically)
  Status (Pass/Fail)
 Majority of test cases are expected to FAIL as per assignment requirement

---

## Technologies Used

Python 3.11+
Playwright
OpenPyXL
Google Chrome / Chromium

---



## Setup Instructions

### 1. Install Dependencies

```bash
pip install playwright openpyxl
playwright install
```

---

### 2. Run the Automation Script

```bash
python test_automation/test_automation.py --excel "IT23819924_Assignment 1 - Test cases.xlsx" --url "https://www.pixelssuite.com/chat-translator" --wait-ms 5000 --type-delay-ms 80 --slow-mo-ms 200 --save-every 1 --keep-open
```

---

## Test Execution

 The script automatically:

   Inputs Singlish text into the web application
   Captures Sinhala output
   Writes results into the Excel file

---

## Output

 Results are recorded in:

  Actual Output column
  Status (Pass/Fail) column

---

## Notes

 Only Chat Sinhala transliteration is tested
 Backend, APIs, performance, and security testing are not included
 Additional columns for:

   Singlish input types
   Evidence / rationale
    were filled manually after execution

---

## Important

 Ensure all dependencies are installed before running
 Excel file must be closed before execution
 GitHub repository must be publicly accessible

---



##  Conclusion

This project demonstrates automated testing of Sinhala transliteration accuracy and highlights weaknesses in chat style language processing.

---
