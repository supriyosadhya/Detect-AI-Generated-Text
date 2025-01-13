# Detect-AI-Generated-Text
AI generated text is largely prevalent nowadays, especially with the popularity of ChatGPT. The use of AI generated text has become very common especially in the field of academia. Hence, the detection of AI generated text has becoming increasingly important.

Dataset
In this project I use two datasets from Kaggle which contains both human written essays and AI generated texts in response to certain queries.
train_essay.csv - https://www.kaggle.com/competitions/llm-detect-ai-generated-text/data train_drcat_02.csv - https://www.kaggle.com/datasets/thedrcat/daigt-proper-train-
dataset?select=train_drcat_02.csv
We combine the two datasets and mainly focus on two columns ‘text’ containing the actual human written or AI generated text and ‘label’ which is 0 for human written text and 1 for AI generated text. we combined 1300 AI generated texts from train_drcat_02.csv to train_essay.csv
We divide this combined dataset into train, validation, and test set in the ratio 70:15:15

Approach
I treated this as a text classification problem and used three different models to solve it. First I used a multinomial Naive Bayes classifier, secondly I used LSTM and thirdly I used a pre-trained BERT model.
