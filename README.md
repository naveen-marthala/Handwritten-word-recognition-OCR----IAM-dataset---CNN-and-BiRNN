This project is about recognising handwritten words with CNN and Bi-directional LSTM, decoded with CTC.

## Dataset:
The IAM Handwriting contains:  
115,320 isolated and labeled words by 657 writers.

You can find the <a href=http://www.fki.inf.unibe.ch/databases/iam-handwriting-database>IAM words dataset</a> here.</br>

## Results:
<img src='sample predictions/sample predictions.jpg' alt=results><br>
Yes, the results are not very promising and out of all words in the holdout set, only about 58.4% have been identified correctly; and rest of the detections have artifacts either at beginning or end of the words. E.g. "It" has been identified as "SIt", with an extra "S" at the beginning. So, obviously this is still far from perfect on holdout set and need to be tuned to fix such artifacts.

## Training:
Trained on GPU on Google Colab with <a href=https://www.tensorflow.org/api_docs/python/tf/keras>tensorflow.keras</a>

## References:
<ol>
  <li>CTC Loss function from <a href=https://towardsdatascience.com/intuitively-understanding-connectionist-temporal-classification-3797e43a86c>this article</a>.</li>
  <li>adapted from <a href=https://github.com/githubharald/SimpleHTR>SimpleHTR</a>.
</ol>
