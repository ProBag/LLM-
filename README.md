# LLM

LLM is a popular technology that holds great promise for revolutionizing education, research, and practice. However, detecting AI-generated text is a challenge. A project was initiated to detect such text using two deep-learning models and BERT. They were trained using a dataset of essays written by students and LLMs. All three models were submitted to a competition.

Keywords: LLM (Large Language Model), NLP (Natural Language Processing), ChatGpt 3,3.5,4, BARD

# Data Collection 
The competition provides a dataset with 3 descriptive features and a target feature. 

The descriptive features are the unique identifiers of each essay, "id", an identifier to the prompt the essay is written to, "prompt_id", and the actual essay itself, "text". 

The target feature is a numerical field named "generated" which indicates whether the text is generated by an LLM (1) or written by a student (0). 

The dataset has 1,375 samples, with only three of them being generated by LLMs. 

This small amount of LLM-generated essays makes it difficult for the model to learn patterns from them adequately. 

Therefore, a new data collection called "daigt-v2-train-dataset" has been chosen instead. "DAIGT" is just the short form of the competition title without LLM. One of the participants in a discussion post shared that the prompts in the original datasets come from a dataset called "PERSUADE 2.0 corpus". By trial and error, the participants discovered the seven prompts that will be used in the testing dataset. This new dataset contains similar features to the original dataset, including text, label, prompt_name, source, and RDizzl3_seven. The first three columns are similar to the original dataset, where instead of using the identifier, the exact prompt name is used. The source refers to where the essay is coming from, including persuade corpus, ChatGPT, Llama 70B, and more. This new dataset has 44,840 essays and more balanced target classes for model training. More details about the dataset will be provided in the exploratory data analysis section.

<img width="339" alt="Screen Shot 2023-12-14 at 5 01 27 PM" src="https://github.com/ProBag/LLM-/assets/143302669/42e55cea-4e66-4476-b292-36a6980365a5">

<img width="492" alt="Screen Shot 2023-12-14 at 5 01 42 PM" src="https://github.com/ProBag/LLM-/assets/143302669/debfddf9-4a29-49e1-ab07-18ea5c325b48">

<img width="476" alt="Screen Shot 2023-12-14 at 5 01 57 PM" src="https://github.com/ProBag/LLM-/assets/143302669/80e7af3d-a8c2-4f0d-9e28-6dc9f65ab6a9">

<img width="652" alt="Screen Shot 2023-12-14 at 5 02 14 PM" src="https://github.com/ProBag/LLM-/assets/143302669/d1d34df1-bf49-49a3-a9a1-dd79e2cd13e6">

<img width="605" alt="Screen Shot 2023-12-14 at 5 02 31 PM" src="https://github.com/ProBag/LLM-/assets/143302669/11c0aa97-b321-40bf-9817-edfcdd603ec6">

# RNN
RNN is a step up in solving the persistence issue of traditional neural networks. When it comes to a text classification task, context and style are important factors that affect the model's prediction. Traditional neural networks cannot retain information in a paragraph. They can only view the entire article at once to gain knowledge, but they cannot capture the details between the lines. RNN's structure is essentially a loop, where an input is passed into a neural network. The network then outputs a result, and the result is passed on to the next network.

<img width="654" alt="Screen Shot 2023-12-14 at 5 03 23 PM" src="https://github.com/ProBag/LLM-/assets/143302669/1b903900-b654-4be5-a248-37ad370be335">
 credit - https://colah.github.io/posts/2015-08-Understanding-LSTMs/

The structure of Recurrent Neural Network (RNN) enables it to preserve information as a sequence of texts is inputted. RNN is known for its ability to handle problems related to sequence and text, such as speech recognition, translation, and sentiment classification.

# Bi-LSTM

LSTMs are designed to process sequential data and can capture long-term context, allowing them to capture nuances that RNNs might miss. Bi-LSTMs process data in both forward and backward directions, enabling them to capture context from both past and future states.

<img width="573" alt="Screen Shot 2023-12-14 at 5 04 42 PM" src="https://github.com/ProBag/LLM-/assets/143302669/336fc838-7d2b-4199-a296-72420ea959b0">

<img width="485" alt="Screen Shot 2023-12-14 at 5 05 00 PM" src="https://github.com/ProBag/LLM-/assets/143302669/b460c9ec-6652-4538-a7f3-4741bc87de92">
Image credit: https://medium.com/@raghavaggarwal0089/bi-lstm-bc3d68da8bd0 

# BERT
BERT, or Bidirectional Encoder Representations from Transformers, is pre-trained to understand language and context and fine-tuned to achieve state-of-the-art results in various concepts of text classification. BERT is achieved by stacking encoders.

<img width="464" alt="Screen Shot 2023-12-14 at 5 05 45 PM" src="https://github.com/ProBag/LLM-/assets/143302669/300f99b9-3c76-4965-8efa-3e2fe510a3f1">
Image credit: https://machinelearningmastery.com/a-brief-introduction-to-bert/

# Model Evaluation 
<img width="641" alt="Screen Shot 2023-12-14 at 5 06 23 PM" src="https://github.com/ProBag/LLM-/assets/143302669/efc5d6ca-1af5-49ce-825d-f42341cc7437">
<img width="652" alt="Screen Shot 2023-12-14 at 5 06 35 PM" src="https://github.com/ProBag/LLM-/assets/143302669/57cb420e-477d-4151-b68c-35a3cec3b1c6">
<img width="285" alt="Screen Shot 2023-12-14 at 5 06 52 PM" src="https://github.com/ProBag/LLM-/assets/143302669/e18b779b-2e6c-47aa-baf0-9c497c9c7bf9">
<img width="243" alt="Screen Shot 2023-12-14 at 5 07 04 PM" src="https://github.com/ProBag/LLM-/assets/143302669/1acf9ff8-2e17-483e-909d-4b48c15cc4b5">
<img width="644" alt="Screen Shot 2023-12-14 at 5 07 21 PM" src="https://github.com/ProBag/LLM-/assets/143302669/73ca7570-1a02-4499-b961-eaa54fccd278">

# Future Results 
During the next chapter of this project, we will discuss TF-IDF vectorization methods in greater detail.







 




