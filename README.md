# Wasserstoff-AiInternTask
#PDF Data Processing and Summarization Project
Description: This project processes PDF files to extract their content, summarize the text, and save the results to a MongoDB database.

System Requirements:
OS: Windows, Mac or Linux
Python Version: Python 3.10 or higher
Libraries: PyPDF2
           nltk
           pymongo
           
MongoDB: Access to a MongoDB Atlas Database

Set Up Instrctions:
    Step 1 : Clone the Repository
            git clone https://github.com/rishul02/wasserstoff-AiInternTask.git
             Navigate to Project folder: cd wasserstoff-AiInternTask
    Step 2 : Install Required Python Libraries
            
    Step 3 : Step Up MongoDB
            1. Create a MongoDB Cluster
            2. Create a Cluster and get the connection String
            3. Update the MongoDB connection string in your pdf_processing_pipeline.py using:
            client = MongoClient("mongodb+srv://<username>:<password>@cluster0.mongodb.net/<database_name>")
              Here Replace the Username , Password and database_name with your original credentials
    Step 4: Move your PDF files into the dataProcessing directory.

From Terminal:
1. pip install PyPDF2
2. pip install pdfplumber
3. use pdf_database
   db.pdf_metadata.find()

Explanation:
1. we used PyPDF2 for reading each PDF and extracting its content.
2. then we use nltk library to process extracted text
3. Used concurrent.futures.ThreadPoolExecutor for concurrent execution of functions, in multiple threads
4. Used pymongo.Mongoclient to interact with a MongoDB database
5. used nltk.corpus.stopwords to ignore unwanted words
6. used tqdm to show the extensible progress bar for loops
7. The summarized content is stored in a MongoDB collection for structured and easy retrieval.

            
     
            
            



