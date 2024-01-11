# RAG-method for Document QA 

## **App Running**

note : the customized API key is stored in the '.env' 
- open the 'main' folder
- open the app.py file
- run 'streamlit run app.py' in terminal

## Testing
Testing the app using two metrics, BERTScore and ROUGE:

### **BERTScore for similarity-based testing**
  - BERTScore calculate the similarity between predictions(app result) and references(ground truth).
  - The result is calculated for comparing the proposed (app result x ground truth) vs (other app result x ground truth)
  - The BERTScore metric result are showing the result of precision, recall, and F1-Score

### **ROUGE for overlap-based testing**
  - ROUGE calculate the overlapping score between predictions(app result) and references(ground truth).
  - The result is calculated for comparing the proposed (app result x ground truth) vs (other app result x ground truth)
  - The result contain rouge-1, rouge-2, rouge-l. Each of them shows the result of precision, recall, and F1-Score

## Documents
Information of document file for testing:
- We used 20 different documents for testing with 100 question test :
  - 5 research paper files (each file contains 5 question)
  - 5 news files (each file contains 5 question)
  - 5 financial report files (each file contains 5 question)
  - 5 recipes files (each file contains 5 question)
