# NYU Redlining Lab: Digitizing Historical Mortgage Documents  

## 📜 Project Overview  
This project involves digitizing **280,000 historical mortgage document scans** (1930–1970) using modern Data Science methods for NYU's Redlining Research Lab. We seek to eliminate the need for manual digitization of documents used for research - achieving an estimated internal **cost saving of $300,000**. The digitization process leverages **Computer Vision** and **GenAI** techniques to build an efficient entity extraction pipeline. The overarching goal is to create a **publicly available dataset of VHA and FHA documents using the pipeline and publish the codebase** for academic research, replicability, and policy making. 

## 🔍 Objectives  

1. **Digitize Historical Data for Quantitative Research**  
   - Convert legacy mortgage documents into machine-readable formats for downstream research and analysis - enabling the largest quantitative research on redlining to-date.  

2. **Ensure Accessibility**  
   - Create a publicly available dataset and code to support academic and societal studies on redlining.  

3. **Automate Processes to Save Cost**  
   - Eliminate manual data entry budgets with the pipeline

## 🛠️ Final Pilot Testing Outcome

- **Custom Entity Extraction Pipeline**: Developed a robust **3-stage** pipeline to extract entities and ensure high accuracy across **.TIF** document formats.  

### Pipeline Stages  

---

<p align="center">


   
  <img width="422" alt="Screenshot 2025-01-14 at 6 42 11 PM" src="https://github.com/user-attachments/assets/0f4c33ae-dafb-4e41-9697-9b19ac9c6e61" />

  
</p>

---

1. **Text Extraction using Open-Source OCR**  
   - Utilized **docTR**, a state-of-the-art **two-step** (CNN + cRNN) deep-learning-based OCR model to extract text from **.TIF** scans.  

2. **Entity Extraction using Prompt-Engineered LLMs**  
   - Tested **Llama**, **Mistral**, **OpenAI**, and **NVIDIA LLMs** to enhance contextual understanding of mortgages and perform **JSON-based entity extraction**.  

3. **Sanity Checks**  
   - Designed fail-safes to ensure:
     - Correct **JSON output structures**.  
     - Completeness of extracted entities.  
     - Flagging model hallucinations.  

4. **Pipeline Validation**  
   - Implemented validation functions to assess pipeline accuracy against ground truth data using relevant metrics (e.g., **Levenshtein Distance**) across features and documents.

## 🔧 Tools & Technologies  

### **Computer Vision & OCR Tested**  
- **docTR**: Open-source deep-learning OCR for high-accuracy text recognition from scanned images.  
- **easyOCR**  
- **Google Tesseract**  

### **LLMs & GenAI Tools Tested**  
- **OpenAI**: 4O-Mini & 4o  
- **Llama**: 3.1 8b  
- **Mistral AI**: NeMo 12B  
- **NVIDIA**: Nemotron 8b  
- **NuMind**: NuExtract  

### **Programming & Frameworks**  
- Python (for scripting and pipeline development)  
- PyTorch (for OCR and LLM integration)  

## 🏆 Impact  

- **Cost Savings**:  
  - Estimated Total Savings of **$300,000** by replacing manual digitization.  
  - **Cost per Document**: **$0.006**.  
  - **Total Projected Cost for 280,000 Documents**: **$1,773**.  

- **Model Accuracy**: **87%** accuracy on a test set of 25 documents using **OpenAI GPT-4o**.  
- **Processing Efficiency**: Each document processed in **26 seconds**.  

## 🚀 Future Scope  

- Deploy the pilot-testing approach across the corpus of 280,000 documents.  
- Initiate quantitative research on redlining from the resulting database.  
- Collaborate with other universities and institutions to digitize similar archives.  

## 📫 Contact  

For more details, reach out to:  
- **Uday Sapra**  
- Email: [uday.sapra@stern.nyu.edu](mailto:uday.sapra@stern.nyu.edu)  
- LinkedIn: [Uday Sapra](https://www.linkedin.com/in/uday-sapra/)  

**Thanks for exploring this project!**
