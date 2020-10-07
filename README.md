This project is about recognising handwritten words with CNN and Bi-directional LSTM, decoded with CTC.

## Dataset:
The IAM Handwriting contains:  
115,320 isolated and labeled words by 657 writers.

You can find the <a href=http://www.fki.inf.unibe.ch/databases/iam-handwriting-database>IAM words dataset</a> here. There's also a lines dataset available.</br>

## Results:
<img src='sample predictions/sample predictions.jpg' alt=results><br>
Yes, the results aren't very promising and only about 58.4% were identified correctly out of all words in the holdout set. And all such mistakes in spellings can be corrected using any language model.<br>
My colab session had crashed (12.72GB of RAM filling up completely) everytime I tried to import pre-trained language model(I was trying to use 'Google Billion words' dataset) to fix these spelling mistakes. For this reason, I have uploaded the jupyter notebooks without having corrected the spellings. And Yes, I do have plans to fix this in the future using cloud VMs.
<!--
and rest of the detections have artifacts either at beginning or end of the words. E.g. "It" has been identified as "SIt", with an extra "S" at the beginning. So, obviously this is still far from perfect on holdout set(validation set)  
-->

## Training:
Trained on GPU on Google Colab with <a href=https://www.tensorflow.org/api_docs/python/tf/keras>tensorflow.keras</a> and took around 9 hours to complete.

## References and Thanks:
<ol>
<li>Image Pre-processing was partly inspired from: <a href ="https://github.com/keras-team/keras/blob/1a3ee8441933fc007be6b2beb47af67998d50737/examples/image_ocr.py"> OCR example on keras github repo</a>.</li>
<li>Custome CTC Loss function from <a href=https://towardsdatascience.com/intuitively-understanding-connectionist-temporal-classification-3797e43a86c>this article</a>.</li>
<li>Network architecture was inspired from following repositories:
  <ul>
    <li><a href=https://github.com/githubharald/SimpleHTR>SimpleHTR</a>,</li>
    <li><a href=https://github.com/TheAILearner/A-CRNN-model-for-Text-Recognition-in-Keras>A-CRNN-model-for-Text-Recognition-in-Keras</a>,</li>
    <li><a href=https://github.com/tuandoan998/HTR-for-IAM>HTR-for-IAM</a></li>
  </ul>
</ol>
