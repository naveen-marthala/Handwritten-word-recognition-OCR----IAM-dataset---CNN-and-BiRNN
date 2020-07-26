This project is about recognising handwritten words with CNN and Bi-directional LSTM, decoded with CTC.

## Dataset:
The IAM Handwriting contains:  
115,320 isolated and labeled words by 657 writers.

You can find the <a href=http://www.fki.inf.unibe.ch/databases/iam-handwriting-database>IAM words dataset</a> here.</br>

## Results:
<img src='sample predictions/sample prediction.jpg'

## Training:
Trained on GPU(Tesla P100-16GB) on Google Colab with <a href=https://www.tensorflow.org/api_docs/python/tf/keras>tensorflow>tensorflow.keras</a>

## References:
<ol>
  <li>CTC Loss function from <a href=https://towardsdatascience.com/intuitively-understanding-connectionist-temporal-classification-3797e43a86c>this article</a>.</li>
  <li>adapted from <a href=https://github.com/TheAILearner/A-CRNN-model-for-Text-Recognition-in-Keras>repo 1<a>,<a href=https://github.com/tuandoan998/HTR-for-IAM>repo 2</a> and <a href=https://github.com/githubharald/SimpleHTR>repo 3</a>.
</ol>
