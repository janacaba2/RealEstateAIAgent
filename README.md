# RealEstateAIAgent

This project is a prototype for a home matching application using Generative AI.
Customer preferences are established during a Q&A session.
Sample questions and customer responses are stored in the qa_data.json file.

The project is divided into four parts:
- HousingDataGenerator.ipynb: Generate dummy housing listings with GPT-3.5-Turbo Model. Resulting data is stored in a csv file.
- RealEstateAgent.ipynb: Save housing data to a vector-DB and then find the listings that best fit the preferences of a customer. Vector DB is leveraged via a Langchain retrieval chain.
- MultiModalRealEstateAgent.ipynb: Save housing data + images to a vector-DB by using CLIP model to embed text and image data and then take the average. Use vector-based similarity search using a customer Q&A + image embedding to retrieve most relevant DB results.
- CreateImages.ipynb: Use playground-v2-1024px-aesthetic model to create housing images based on input text that is created from given housing and Q&A data.

**Necessary settings:**
A personal open-ai api key and base are necessary and have to be set in the config.py file.
