# Insurance Claim Tone Classifier

## Overview

This project uses a Large Language Model (LLM) to classify insurance claim descriptions.

The classifier identifies:

* Claim Type (Motor, Property, Liability)
* Tone (Calm, Frustrated, Urgent)
* Legal Action (Yes, No)

## Technologies Used

* Python
* Pandas
* LiteLLM
* Groq API

## Project Workflow

1. Read insurance claims from a CSV file.
2. Generate a prompt for each claim.
3. Send the prompt to the LLM.
4. Receive classification results.
5. Convert the response into structured JSON.
6. Save results into output.json.

## Files

* insurance_claims.csv → Input claims
* classifier.py → Main application
* output.json → Generated classifications

## Run the Project

pip install -r requirements.txt

python classifier.py

## Important:
Create a .env file and add:

GROQ_API_KEY=your_api_key_here