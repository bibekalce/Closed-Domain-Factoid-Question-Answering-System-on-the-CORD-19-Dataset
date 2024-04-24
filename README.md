Closed Domain Factoid Question-Answering System:
The project focuses on implementing and evaluating a Closed Domain Factoid Question-Answering System on COVID-19 research articles. Its primary objective is to extract relevant articles and information based on user queries.

User Utility:
![output_format](https://github.com/bibekalce/Closed-Domain-Factoid-Question-Answering-System-on-the-CORD-19-Dataset/assets/24669020/81d6dd7a-eaa8-4956-a5de-c339db8c80b5)


The system offers a user-friendly interface with intuitive controls, including checkboxes for sound and paper details for a query. Upon submitting a query, the system retrieves relevant documents and extracts the most pertinent answers. Leveraging the Google Text-to-Speech API (gTTS), both the query and answer are transformed into audio files, providing enhanced accessibility and usability for users.

Dataset:
The system utilizes a subset of the COVID-19 Open Research Dataset Challenge (CORD-19)(https://www.kaggle.com/datasets/allen-institute-for-ai/CORD-19-research-challenge), comprising 10,000 randomly sampled articles. This subset ensures computational feasibility while retaining the diversity and richness of the original dataset.
Components
Information Retrieval (IR) System: Retrieves relevant snippets of articles from the corpus.
Question-Answering (QA) System: Extracts answers from relevant snippets.
Methods Utilized
Coreference Resolution
Named Entity Recognition (NER)
Word Embedding (FastText)
BERT Model Fine-Tuning with SQuAD Dataset
Summarization using BART
Google Text-to-Speech for Output Utility
Methodology:
The preprocessing phase includes coreference resolution, data cleaning, and named entity extraction to ensure dataset quality and relevance. Subsequently, an inverted index facilitates efficient information retrieval. FastText is employed for word embedding, while a knowledge base enriches contextual understanding. Summarization techniques using BART condense snippets, and fine-tuned BERT models enhance question-answering accuracy.
Results:
The system's performance is evaluated using Mean Reciprocal Rank (MRR) and Mean Average Precision (MAP) metrics. Achieved accuracy compared to ground truth across 10 questions is 50%, with an average MRR of 0.72 and average MAP of 0.384.
Learnings and Limitations
The use of the whole document embedding may yield irrelevant documents, necessitating passage tokenization.
FastText proves effective for word embedding but is computationally expensive.
Utilization of the SQuAD dataset improves BERT's ability to handle new questions.
Challenges include coreference resolution accuracy and knowledge base expansion.
Future Work
Future endeavors could focus on enhancing Named Entity Recognition accuracy and refining query-document matching algorithms, paving the way for improved system performance and user experience.
