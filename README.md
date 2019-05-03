# Using BERT in Keras with tensorflow hub
Following on our [previous demo using ELMo embeddings in Keras with tensorflow hub](https://github.com/strongio/keras-elmo), we present a brief demonstration on how to integrate BERT from tensorflow hub into a custom Keras layer that can be directly integrated into a Keras or tensorflow model.

See the accompanying blog post with further description


https://towardsdatascience.com/bert-in-keras-with-tensorflow-hub-76bcbc9417b
https://colab.research.google.com/github/google-research/bert/blob/master/predicting_movie_reviews_with_bert_on_tf_hub.ipynb

## Dataset
First, Load the dataset, hosted by Stanford.

the IMDB Large Movie Review Dataset, is borrowed from [this Tensorflow tutorial](https://www.tensorflow.org/hub/tutorials/text_classification_with_tf_hub).

*** BERT.zip --> train_data.pickle & test_data.pickle

```python
# code to load dataset as dataframe
import pickle

# load
with open('train_data.pickle', 'rb') as f:
    train = pickle.load(f)
    
# load
with open('test_data.pickle', 'rb') as f:
    test = pickle.load(f)
```
