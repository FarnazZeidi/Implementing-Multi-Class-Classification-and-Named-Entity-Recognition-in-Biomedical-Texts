# **Implementing Multi-Class Classification and Named Entity Recognition in Biomedical Texts**  

This repository demonstrates the application of **Multi-Class Classification** and **Named Entity Recognition (NER)** models on two biomedical datasets:  
1. **PubMed 20k RCT** [1] for Multi-Class Classification.  
2. **BC5CDR** [2] for Named Entity Recognition (NER).  

## **Models Used**  
Both Multi-Class Classification and NER tasks are implemented using two pre-trained BERT-based models:  
1. **bert-base-cased** [3]: A general-purpose language model trained on English texts.  
2. **biobert-base-cased-v1.2** [4]: A domain-specific BERT model pre-trained on biomedical literature.  

### **Training Parameters**  
Both models were fine-tuned using the **Simple Transformers library**[5], with the following configurations:  
- **Epochs**: 1 (extendable to 3 for improved performance).  
- **Batch Size**: 16 for both training and evaluation phases.  

---

## **Discussion**  

The experiments highlight the critical importance of domain-specific pretraining for NLP tasks in specialized fields like biomedicine. The **biobert-base-cased-v1.2** model consistently outperformed its general-purpose counterpart, **bert-base-cased**, across both Multi-Class Classification and NER tasks. This underscores the effectiveness of leveraging domain-specific knowledge for enhanced performance in biomedical NLP applications.  

---

## **References**  

1. Dernoncourt, F., Lee, J. Y. (2017). "PubMed 200k RCT: A Dataset for Sequential Sentence Classification in Medical Abstracts." *International Joint Conference on Natural Language Processing (IJCNLP).*  
2. Li, J., et al. (2016). "BioCreative V CDR Task Corpus: A Resource for Chemical Disease Relation Extraction." *Database.*  
3. Hugging Face Transformers Model: bert-base-cased. https://huggingface.co/google-bert/bert-base-cased
4. Hugging Face Transformers Model: biobert-base-cased-v1.2: https://huggingface.co/dmis-lab/biobert-base-cased-v1.2 
5. Simple Transformers Documentation: [https://simpletransformers.ai/](https://simpletransformers.ai/).  

---  

