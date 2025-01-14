# NYU Redlining Lab: Digitizing Historical Mortgage Documents  

## 📜 Project Overview  
This project involves digitizing **280,000 historical mortgage document scans** (1930–1970) as part of the NYU Redlining Lab. The goal was to create a **publicly available dataset** by leveraging **computer vision** and **Generative AI (GenAI)** techniques for entity extraction, eliminating the need for manual digitization and achieving an estimated **cost saving of $300,000** for NYU.  

## 🛠️ Key Features  

- **Custom Entity Extraction Pipeline**: Developed a robust **3-stage** pipeline to extract entities and ensure high accuracy across **.TIF** FHA and VHA documents.  

### Pipeline Stages  

<p align="center">
  <img width="383" alt="Screenshot 2025-01-14 at 6 39 52 PM" src="https://github.com/user-attachments/assets/5136d5a6-9cb2-4b66-8f88-6ebe90435313" />
</p>


1.  **Text Extraction using Open-Source OCR**  
   - Utilized **docTR**, a state-of-the-art **two-step** (CNN + cRNN) deep-learning-based OCR model to extract text from **.TIF** scans.  

2.  **Entity Extracing using Prompt-Engineered LLMs**  
   - Tested **Llama**, **Mistral**, **OpenAI**, and **NVIDIA LLMs** to enhance contextual understanding of mortgages and perform **JSON-based entity extraction**.  

3. **Sanity Checks**  
   - Designed fail-safes to ensure:
     - Correct **JSON output structures**.  
     - Completeness of extracted entities.  
     - Flagging of model hallucinations.  

4. **Pipeline Validation**  
   - Implemented validation functions to assess pipeline accuracy against ground truth data using relevant metrics (e.g., **Levenshtein Distance**) across features and documents.

## 🔍 Objectives  
1. **Digitize and Preserve Historical Data**: Convert legacy mortgage documents into machine-readable formats for research and analysis - enabling the largest quantitative research on redlining to-date.  
2. **Ensure Accessibility**: Create a publicly available dataset and code to support academic and societal studies on redlining.  
3. **Automate Processes**: Eliminate manual data entry with advanced AI tools, improving efficiency and reducing costs.

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
  - Estimated total savings of **$300,000** by replacing manual digitization.  
  - **Cost per document**: **$0.006**.  
  - **Total cost for 280,000 documents**: **$1,773**.  

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
