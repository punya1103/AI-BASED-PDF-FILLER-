README File
PDF Form Filler Project
This project reads company data from a structured text file and automatically fills out a PDF form with the extracted data. After the form is filled, a pop-up message confirms the success of the operation.

Table of Contents
Project Overview
Requirements
Installation
Usage
File Structure
License
Project Overview
This script automates the process of reading data from a text file, mapping it to corresponding fields in a PDF form, and generating a filled PDF. A pop-up message informs the user upon successful completion.

Features
Extracts data from a structured text file.
Fills PDF form fields based on predefined mappings.
Displays a pop-up message after the PDF is filled and saved.
Requirements
The project requires the following Python packages:

PyPDF2: For reading and writing PDF files.
tkinter: For displaying pop-up messages (part of Python standard library).
Installation
Clone or Download the Project:

bash
Copy code
git clone https://github.com/yourusername/pdf-form-filler.git
cd pdf-form-filler
Install Dependencies:

Use pip to install the required packages:

bash
Copy code
pip install -r requirements.txt
Usage
Prepare Input Data:

Ensure the new_data.txt file contains the company data in a format like:

yaml
Copy code
Company Name: TechNova Solutions Inc.
Founded: 2005
CEO: Ellie Kang
Industry: Information Technology
Revenue: $2 Billion
...
Run the Script:

To generate the filled PDF and display the success message:

bash
Copy code
python script.py
The script will generate a filled PDF form in the output directory and pop up a success message.

File Structure
graphql
Copy code
.
├── data
│   ├── new_data.txt                # Input text file containing the company data
│   ├── new_dummy_form.pdf          # Input PDF form template
├── output                          # Directory where the filled PDFs will be saved
├── script.py                       # Main Python script
├── README.md                       # Documentation (this file)
├── requirements.txt                # Python dependencies file


requirements.txt
bash
Copy code
PyPDF2==3.0.0
PyPDF2: Used for manipulating PDF files.
tkinter: Included by default with Python (no need to install separately).