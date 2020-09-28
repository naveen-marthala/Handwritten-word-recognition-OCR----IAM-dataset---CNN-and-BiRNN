This project is about recognising handwritten words with CNN and Bi-directional LSTM, decoded with CTC.

## Dataset:
The IAM Handwriting contains:  
115,320 isolated and labeled words by 657 writers.

You can find the <a href=http://www.fki.inf.unibe.ch/databases/iam-handwriting-database>IAM words dataset</a> here.</br>

## Results:
<img src='sample predictions/sample predictions.jpg' alt=results><br>
Yes, the results are not very promising and out of all words in the holdout set, only about 58.4% have been identified perfectly; These can be fixed using any language model that can fix spelling mistakes.<br>
My machine consistenly crashed(16GB of RAM filled up completely) whenever I tried to import pre-trained language model(trained on 'Google Billion words' dataset) to fix such spelling mistakes. So, I uploaded the notebooks without spelling correction. Yes, I do have plans to fix this in the future.
<!--
and rest of the detections have artifacts either at beginning or end of the words. E.g. "It" has been identified as "SIt", with an extra "S" at the beginning. So, obviously this is still far from perfect on holdout set(validation set)  
-->

## Training:
Trained on GPU on Google Colab with <a href=https://www.tensorflow.org/api_docs/python/tf/keras>tensorflow.keras</a>

## References:
<ol>
<li>Pre-processing inspired from: <a href ="https://github.com/keras-team/keras/blob/1a3ee8441933fc007be6b2beb47af67998d50737/examples/image_ocr.py"> OCR example on keras github repo</a>.</li>
<li>CTC Loss function: <a href=https://towardsdatascience.com/intuitively-understanding-connectionist-temporal-classification-3797e43a86c>this article</a>.</li>
<li>Network architecture Inspired from:
  <ul>
    <li><a href=https://github.com/githubharald/SimpleHTR>SimpleHTR</a>,</li>
    <li><a href=TheAILearner/A-CRNN-model-for-Text-Recognition-in-Keras>A-CRNN-model-for-Text-Recognition-in-Keras</a>,</li>
    <li><a href=https://github.com/tuandoan998/HTR-for-IAM>HTR-for-IAM</a></li>
  </ul>
</ol>
