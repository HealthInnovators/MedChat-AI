# MedChat AI

### Overview:
MedChat AI is an open-source language model (LLM) specifically designed for healthcare chat applications. It aims to provide accurate, reliable, and context-aware responses to inquiries related to medical information, health advice, symptom analysis, and more. The model will be trained on a diverse dataset sourced from reputable medical literature, clinical guidelines, and anonymized patient data (in compliance with privacy regulations) to ensure its effectiveness and safety in providing healthcare-related information.

### Useful Links

## HealthLLM Framework to build RAG Chat health applications

  -  https://arxiv.org/pdf/2402.00746
  -  https://youtu.be/Us44JYUVX9g?si=LvCeXm6U2vtWBzoz
  -  https://www.llamaindex.ai/

## Models

  -  BioBERT (Clinical model trained on discharge data) - https://sparknlp.org/2020/08/25/biobert_discharge_base_cased.html | https://huggingface.co/emilyalsentzer/Bio_Discharge_Summary_BERT | https://arxiv.org/pdf/1904.03323
  
  -  ClinicalBERT (Clinical model trained on EHR data) - https://arxiv.org/abs/1904.05342 | https://huggingface.co/medicalai/ClinicalBERT

  -  BioMistral (Medical model trained on PubMed central data) - https://arxiv.org/abs/2402.10373 | https://huggingface.co/BioMistral/BioMistral-7B | https://huggingface.co/MaziyarPanahi/BioMistral-7B-GGUF (Quantized Model - Runs on local computer cpu)

  -  Qwen 2 (Vision + Text (multimodal) language model) - https://huggingface.co/HuggingFaceM4/idefics2-8b | https://huggingface.co/docs/transformers/main/en/model_doc/idefics2 | https://huggingface.co/blog/idefics2

  -  Llama 3 (General purpose model) - https://llama.meta.com/llama3/

## Opensource Vector Databases:

  -  Chroma - https://www.trychroma.com/
  -  Qdrant - https://qdrant.tech/
  -  Milvus - https://milvus.io/

Model Fine-tuning - https://github.com/hiyouga/LLaMA-Factory

## Use cases for RAG Chatbot - https://www.youtube.com/watch?v=3OGpbWLQQbo

**Chatbot for discharge summaries** - https://sparknlp.org/2020/08/25/biobert_discharge_base_cased.html | https://huggingface.co/emilyalsentzer/Bio_Discharge_Summary_BERT | https://arxiv.org/pdf/1904.03323

**Chatbot for Medicare health insurance policy** - https://www.medicare.gov/publications/10050-Medicare-and-You.pdf (Medicare is the largest insurance organization in USA)

**Clinical trial recruitment chatbot** - Clinical trial recruitment chatbot for Revolutionizing Mental Health Decentralized Clinical Trials for Psilocybin and Psilocin.

**Chatbot for medical record and personal data** (This requires downloading the medical record and data)

  -  Medical Information Mart for Intensive Care (Medical record data) - https://mimic.mit.edu/ | https://github.com/MIT-LCP/mimic-code | 
     https://mimic.mit.edu/docs/gettingstarted/
  -  Download health data from iPhone via Apple HealthKit - https://developer.apple.com/documentation/healthkit

  -  Download your medical record on your iPhone via Apple HealthKit - https://support.apple.com/en-ca/guide/iphone/iphc30019594/ios

  -  Google Fit (Lets you download your health data on Android) - https://www.google.com/fit/

  -  Blue Button (You can download your medical record using the blue button) - https://www.healthit.gov/topic/patient-access-information-individuals-get-it-check-it-use-it/blue-button

  -  Open Data Kit (Lets you acquire data from wearable devices) - https://getodk.org/
    
  -  Electronic Health Records (EHRs) Datasets - https://som-shahlab.github.io/ehrshot-website/

  -  Electronic Health Records (EHRs) Data Exploration - https://www.kaggle.com/code/gpreda/electronic-health-records-ehrs-data-exploration

  -  Medical Records Dataset - https://www.kaggle.com/datasets/cankatsrc/medical-records-dataset

  -  Synthea Dataset Jsons - https://www.kaggle.com/datasets/krsna540/synthea-dataset-jsons-ehr

  -  Apple Watch and Fitbit Kaggle data - https://www.kaggle.com/datasets/aleespinosa/apple-watch-and-fitbit-data

  -  Smartwatch Data Analysis - https://www.kaggle.com/code/amirmotefaker/smartwatch-data-analysis

  -  Activity recognition using wearables Kaggle datasets - https://www.kaggle.com/c/activity-recognition-wearables/overview

  -  FitBit Fitness Tracker Kaggle Data - https://www.kaggle.com/datasets/arashnic/fitbit/code


**MedPal** (Health Advocate AI) - https://docs.google.com/document/d/140chg3InY17M1cHWs5h8-TbLYf810MfDHz5eWt1iGe4/edit?usp=sharing
**LabPal** - Most lab procedures involve specific dietary protocols to following before the procedure, LabPal helps the patient follow these protocols in simple language. The lab procedure could get cancelled if the patient does not adhere to the protocols.
**SurgeryPal** - All surgical procedures involve specific protocols to following before the surgery, SurgeryPal helps the patient follow these protocols in simple language. The Surgery could get cancelled if the patient does not adhere to the protocols.
**AA Chat** - Alcoholics Anonymous Chat helps with addiction and connects to AA mentors. AA uploads all the training material and resources to our vector database.

Implementation - Watch this video to implement the BioMistral chatbot locally - https://www.youtube.com/watch?v=A_m3tCqdts4

### Project Structure:

Folders within the repository for different components:
**data**: This folder will store the training data for the LLM.
Focus on collecting publicly available healthcare chat conversations, medical information resources, and relevant research papers.
Ensure proper anonymization of any patient data.
**code**: This folder will hold the scripts for training, fine-tuning, and deploying the LLM.
We will consider using open-source libraries like Transformers (https://huggingface.co/docs/transformers/en/index) and libraries for medical text processing.
**docs**: This folder will include documentation on using the LLM, including installation instructions, API details, and usage examples.
**evaluations**: This folder will store the results of performance evaluations on the LLM, including metrics relevant to healthcare chat applications (e.g., accuracy, safety, bias detection).
**meeting-notes**: This folder will store the regular meeting minutes.

### Features:
- **Context-aware Responses:** OpenHealthChatLLM understands the context of the conversation and provides relevant responses tailored to the user's inquiries.
- **Medical Knowledge Base:** The model is trained on a vast repository of medical knowledge, covering various medical specialties and topics.
- **Privacy and Security:** OpenHealthChatLLM prioritizes user privacy and data security, ensuring compliance with healthcare regulations such as HIPAA (Health Insurance Portability and Accountability Act).
- **Customization:** Users can fine-tune the model for specific healthcare domains or integrate additional datasets to enhance its capabilities.
- **Scalability:** MedChat AI is designed to scale efficiently, allowing seamless integration into both small-scale applications and large-scale healthcare platforms.

### Contribution Guidelines:
We welcome contributions from developers, researchers, and healthcare professionals to improve OpenHealthChatLLM. Contributions can include but are not limited to:
- **Model Enhancements:** Improving the model's accuracy, performance, and efficiency.
- **Data Collection and Annotation:** Adding new datasets and annotating existing ones to expand the model's knowledge base.
- **Privacy and Security Improvements:** Implementing robust privacy measures and security protocols.
- **Documentation:** Writing and updating documentation to facilitate usage and development.
- **Bug Fixes:** Identifying and fixing bugs to ensure the reliability of the model.

### Getting Started:
To get started with MedChat AI, follow these steps:
1. Clone the repository: `git clone https://github.com/HealthInnovators/OpenHealthChatLLM`
2. Install dependencies: `pip install -r requirements.txt`
3. Explore the documentation to understand how to use and contribute to OpenHealthChatLLM.

### License:
MedChat AI is licensed under the MIT License.

### Contact:
For inquiries or suggestions, please contact the project maintainers at [kal@healthiai.org](mailto:kal@healthiai.org).

### Disclaimer:
MedChat AI is a research project and should not be used as a substitute for professional medical advice. Users are encouraged to consult qualified healthcare professionals for medical concerns and advice.
