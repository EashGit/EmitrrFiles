# Medical NLP Project

This project implements a Python-based NLP pipeline to analyze a physician-patient conversation. It performs three main tasks:
1.  **Medical Summarization:** Extracts key medical details (Symptoms, Diagnosis, Treatment, Prognosis).
2.  **Sentiment & Intent Analysis:** Analyzes patient utterances to detect sentiment (Anxious, Neutral, Reassured) and intent.
3.  **SOAP Note Generation:** Automatically structures the conversation into a clinical SOAP note (Subjective, Objective, Assessment, Plan).

---

## 🚀 Setup

1.  **Install Dependencies:**
    This project requires Python 3.7+ and the following libraries. You can install them all using pip:

    ```bash
    pip install torch transformers spacy
    ```

2.  **Download spaCy Model:**
    You also need to download the English language model for spaCy.

    ```bash
    python -m spacy download en_core_web_lg
    ```

---

## 🏃 How to Run

1.  **If using Google Colab:**
    * Run the setup commands in the first cell (prefixed with `!`).
    * Run the subsequent code cells for each task.

2.  **If running locally (e.g., as `.py` files):**
    * Save the project code (from the second section) as `medical_nlp.py`.
    * Make sure you are in the same directory as the file.
    * Run the script from your terminal:

    ```bash
    python medical_nlp.py
    ```

The script will run all three analysis tasks on the provided transcript and print the structured JSON outputs for each part to the console.