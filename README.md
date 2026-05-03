# Assignment 1 - Option 1: Transliteration Accuracy Testing

## Student Details
- Registration Number: ITxxxxxx
- Module: IT3040 - ITPM
- Assignment: Assignment 1 - Option 1

## Project Purpose
This project automates negative transliteration accuracy test cases for the Pixelssuite Chat Sinhala translator.
The test data is recorded in the Excel file named `Assignment 1 - Test cases.xlsx`.

## Files Included
- `test_automation.py` - Playwright automation script.
- `Assignment 1 - Test cases.xlsx` - Completed test case Excel file.
- `requirements.txt` - Python dependencies.
- `README.md` - Setup and execution instructions.
- `Git_Repository_Link.txt` - Public Git repository link.

## Prerequisites
Install the following before running the automation:

1. Python 3.11 or 3.12
2. Google Chrome or Playwright Chromium

## Setup Instructions
Open Command Prompt and navigate to the project folder:

```bash
cd /d D:\test_automation
```

Install dependencies:

```bash
pip install -U pip
pip install -r requirements.txt
playwright install
```

## How to Run the Tests
Run the following command from the project root folder:

```bash
python test_automation.py --excel "Assignment 1 - Test cases.xlsx" --url "https://www.pixelssuite.com/chat-translator" --wait-ms 5000 --type-delay-ms 80 --slow-mo-ms 200 --save-every 1 --keep-open
```

## Expected Automation Result
The script reads the test case input and expected output from Excel, enters each Singlish input into the Chat Sinhala translator, captures the actual Sinhala output, and writes the result back to the Excel file under:

- Actual output
- Status

A test case is marked as `Pass` only when the actual output exactly matches the expected output. Since this assignment focuses on failure scenarios, the selected negative test cases are expected to expose mismatches after automation execution.

## Important Notes
- Do not manually fill the `Actual output` and `Status` columns before running the script.
- After running automation, manually review the actual outputs and confirm the status values.
- Keep the GitHub repository public until marking is completed.