# Entity-Oriented-Polarity-Detection-from-Document

In this project, we aim to address the problem of determining entity-oriented polarity in business news documents.
We attempt to classify the polarity of the sentiment expressed toward a given mention of a company in a news article. 
Here the polarity of the named entity which is the company or organization mentioned in the news can be classified into positive, negative, or neutral. 
In this work, we present a BERT-based NLI (Natural Language Inference) model to classify polarity of entity mentioned in text.
Our model gives a benchmark test accuracy of 0.9646 and a F1 score of 0.9258 in predicting if the given hypothesis for the NLI task contradicts, entails or is neutral to the corresponding premise.

## 1.1 Problem Statement
In this project we classify the polarity of the entity in a news article. 
For this task, we use a dataset of over 17,000 manually labeled documents, containing 20,000 different entity-premise pairs. 
The polarity of the entity in each premise is classified as positive, negative, or neutral.
The steps of the task were to preprocess the dataset, append a hypothesis at the end of each premise in the dataset, and then predict if the given hypothesis contradicts, entails or is neutral to the corresponding premise.

## 1.2 Dataset

The data is organized as a list of documents. Each document is a dictionary that has the following fields:

• url: the document source

• content: the document text

• headline: the headline position in the text

• docnoId: unique identifier of the document

• entities: a list of annotated company names

“entities” is a list that has the following fields:

• entityId: the entity identifier in this document; entities from different documents may have the same id

• name: company name

• offsets: the entity positions in the text

• polarity: manually annotated polarity

## 1.3 Links to dataset :

• Original dataset : https://drive.google.com/file/d/1W9cBf33LEX_9MqzaWcpW3QdkmQtMHuv2/view?usp=sharing

• Processed dataset : https://drive.google.com/file/d/1a1NfFAnpQYTgzW-TRpnpddUjoL02vLJR/view?usp=sharing

• Train set : https://drive.google.com/file/d/12UB8Ok3tA9Yh6i3uSys3kTqB0hcq2UIN/view?usp=sharing

• Dev set : https://drive.google.com/file/d/15VSLEBEcMFzuaPi46SP9HWEJySzJ3guT/view?usp=share_link

• Test set : https://drive.google.com/file/d/1PiZka4TJQ__3AGPCHfchPkTT4SfuDAS0/view?usp=sharing

• Model : https://drive.google.com/file/d/12bkyIBwyNJWfY3hfi-9KBqwWwA2BCwZI/view?usp=sharing
