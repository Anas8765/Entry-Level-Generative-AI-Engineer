# Generative-AI-Engineer

There are two notebooks: one is for summarizing the contents of any kind of book, and the other is for creating a personalized study plan for students. Both of these notebooks use AI to solve their respective tasks.

# Summarization of a book
In this notebook, it first takes the PDF of a book, converts it into text, and then uses the "facebook/bart-large-cnn" model from Hugging Face to generate a summary. The process of generating a summary occurs at every 20 complete sentences, followed by the next set of 20 complete sentences. It then compiles all the summarized text by joining all those sentences and converts that text into a PDF, thus providing a summary of the entire book in a PDF file. The completion of text summarization takes time, depending on the size of the book. And the summarization itself is abstractive summary of the entire text.

# Prompt Engineering
In this notebook, a quantized version of the 'meta-llama/Llama-2-13b-chat-hf' model from Hugging Face is used to create a study plan for students. A prompt template is provided using the Langchain library, and based on the prompts of different types of students, it generates a personalized study plan for them. In this notebook, students can input their own prompts into these variables to create a study plan for themselves:
name = ""
field_of_study = ""
year_of_study = ""
list_of_subjects = ""
preferred_learning_styles = ""
personal_objectives = ""
challenges = ""
extracurricular_activities = ""
