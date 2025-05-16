# Chest X-ray Diagnosis(AI Radiologist)
- This application basically takes the x-ray image of chest and classify it as covid attacked or pneumonia(non-covid) or normal and provides justification based on visual findings.
- Here is an finetuned LLM model which is finetuned from the base model unsloth/llama-3.2-11b-vision-instruct-unsloth-bnb-4bit using a covid_chestXray dataset with unsloth library for efficiently finetunning the base model.This finetuned LLM model processes the whole work in the application.
- Model repository:

     [![model repository](https://img.shields.io/badge/model_repository-1DA1F2?style=for-the-badge&logo=modelrepository&logoColor=white)](https://huggingface.co/Suman2004/covid_chestXray_radiologist)

- Dataset repository after the processing the raw csv data:

  [![dataset_repository](https://img.shields.io/badge/dataset_repository-1DA1F2?style=for-the-badge&logo=Sdatasetrepository&logoColor=white)](https://huggingface.co/datasets/Suman2004/covid_chestXray)

- ## Training Details
- Training graphs are given below

     ![Screenshot (299)](https://github.com/user-attachments/assets/0986755c-4672-4f36-820e-e2e26638234a)


- Run summary is given below
  
     ![Screenshot (298)](https://github.com/user-attachments/assets/7a3d62a6-9ce6-449b-a4a3-c51710029d98)

  

- ##  User Interface
- This system provides gradio user interface to user.

     ![Screenshot (291)](https://github.com/user-attachments/assets/03ef7086-1ef9-462d-bd42-99a9b461b312)


- Testing with an input:

     ![WhatsApp Image 2025-05-16 at 02 37 00_11ef36b3](https://github.com/user-attachments/assets/0ff10875-8aee-4f89-b69a-f9c6d30deee6)

  

- ## Deployment
- As,we use our own finetuned model so,for loading the model directly and processing the work,we need minimum 15 GB GPU storage which is available in hugging face space but, it is costly.So,that's why we test the model in google collab file with gradio interface.

