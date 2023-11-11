# News_Topic_Classification
This task aims to build a prediction model in classifying news topics or themes based on the initial content of the news. The dataset is taken from 5 different news media, namely Kompas, CNN, Detik.com, Tempo and Liputan6 by taking 3 labels, namely Entertainment, Sports and Politics.

Datasets are retrieved using data crawling using BeautifulSoup by reading html tags from each different news media. The total data taken is 450 data with each label having 150 data (balanced).

After that the dataset is cleaned from all noise, including
- url cleaning
- Tag or hashtag cleaning
- Changing newline to space
- Replacing double space into single space
- Discarding all non-alphabetic charac
- Stopword Re
- Stemmi

After cleaning the data, the data is represented using word embeddings, namely Word2Vec and also FastText with the skip-gram method. For details, please refer to the explanation.

Afterwards, the SVM and random forest models were run with both text representations and the result was that everything went well, where the best results were obtained from the SVM model with word2Vec embedding with an accuracy of 9%.

Translated with www.DeepL.com/Translator (free version)
