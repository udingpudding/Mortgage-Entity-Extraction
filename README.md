
# NYU Redlining Lab: Digitizing Historical Mortgage Documents  

## 📜 Project Overview  
This project involves digitizing **280,000 historical mortgage document scans** (1930–1970) as part of the NYU Redlining Lab. The goal was to create a **publicly available dataset** by leveraging **computer vision** and **Generative AI (GenAI)** techniques for entity extraction, eliminating the need for manual digitization and achieving an estimated **cost saving of $300,000** for NYU.  

## 🛠️ Key Features  
- **Custom Entity Extraction Pipeline**: Developed a robust **3-Stage** pipeline to extract entities and ensure high accuracy across **.TIF** FHA and VHA documents.
### Pipeline Stages 
- **Stage #1 Open-Source OCR**: Used **docTR**, a state-of-the-art **two-step** (CNN + cRNN) deep-learning-based OCR model, to extract text from .TIF scans. 
- **Stage #2 Prompt-Engineered LLMs**: Tested Prompt-Engineered **Llama**, **Mistral**, **OpenAI**, and **NVIDIA LLMs** for contextual mortgage understanding and JSON based Entity Extraction. 
- **Stage #3 Sanity Checks**: Designed fail-safes to ensure correct JSON output strucutres, completeness of extracted entities, and flag model hallucination. 
- **Stage #4 Validation**: Designed functions to test pipeline accuracy against ground truth using relevant metrics (Levenshtein Distance) - across features and documents.

---

## 🔍 Objectives  
1. **Digitize and Preserve Historical Data**: Convert legacy mortgage documents into machine-readable formats for research and analysis - enabling the largest quantitiative research on redlining to-date.  
2. **Ensure Accessibility**: Create a publicly available dataset and code to support academic and societal studies on redlining.  
3. **Automate Processes**: Eliminate manual data entry with advanced AI tools, improving efficiency and reducing costs.

---

## 🔧 Tools & Technologies  
### **Computer Vision & OCR**  
- **docTR**: Open-source deep-learning OCR for high-accuracy text recognition from scanned images.  

### **LLMs & GenAI Tools Tested**  
- **OpenAI**: 4O-Mini & 4o
- **Llama**: 3.1 8b
- **Mistral AI**: NeMo 12B
- **NVIDIA**: Nemotron 8b
- **NuMind**: NuExtract

### **Programming & Frameworks**  
- Python (for scripting and pipeline development)  
- PyTorch (for OCR and LLM integration)  

---

## 🏆 Impact  


- **Cost Savings**:  
  - Estimated total savings of **$300,000** by replacing manual digitization.  
  - **Cost per document**: **$0.006**.  
  - **Total cost for 280,000 documents**: **$1,773**.  
- **Model Accuracy**: **87%** accuracy on a test set of 25 documents using **OpenAI GPT-4o**.  
- **Processing Efficiency**: Each document processed in **26 seconds**.  

---

## 🚀 Future Scope  
- Deploy the pilot-testing approach across the corpus of 280,000 documents. 
- Initiate quantitative research on redlining from resulting database. 
- Collaborate with other universities and institutions to digitize similar archives.  

---
## 📫 Contact  
For more details, reach out to:  
- **Uday Sapra**  
- Email: [uday.sapra@stern.nyu.edu](mailto:uday.sapra@stern.nyu.edu)  
- LinkedIn: [Uday Sapra](https://www.linkedin.com/in/uday-sapra/)  

---

**Thanks for exploring this project! Your support helps make history accessible.**  
