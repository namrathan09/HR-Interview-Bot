In today’s competitive job market, the recruitment process can be time-consuming and inefficient. HireSmart is an AI-based interview bot designed to streamline hiring by automating data extraction, resume matching, and interview evaluation. Combining RPA, AI models, and NLP, the system offers an efficient and objective solution for recruiters and job seekers.

Phase 1: Storing and Matching Data
In the first phase, the extracted data from the Excel file is loaded into ChromaDB, a vector database used for managing and searching relevant job data efficiently. 
A website interface is created where users can log in with valid credentials. 
Once successfully authenticated, users are allowed to upload their resumes. 
The uploaded resumes are then analyzed using the AI model "EleutherAI/gpt-neo-1.3B" to extract key skills and match them with job roles and company information. 
This phase determines the similarity between a candidate’s skills and the available job descriptions in the form of cosine similiarity.

Phase 2: AI-Based Interview and Evaluation
In the second phase, users are provided with an opportunity to proceed to the interview stage based on the matched job roles. 
The system generates pre-defined technical questions that candidates must answer. 
These responses are then evaluated using the SentenceTransformer model 'paraphrase-MiniLM-L6-v2', which analyzes and scores the answers based on semantic similarity. 
This phase ensures a fair and objective evaluation of candidates' technical knowledge (any answer close to the pre-defined answer is acceptable)



