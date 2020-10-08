This project is about recognising handwritten words with CNN and Bi-directional LSTM, decoded with CTC.

## Dataset:
The IAM Handwriting contains:  
115,320 isolated and labeled words by 657 writers.

You can find the <a href=http://www.fki.inf.unibe.ch/databases/iam-handwriting-database>IAM words dataset</a> here. There's also a lines dataset available.</br>

## Results:

<h4>Test image following the predicted text are shown below:</h4>

<ol>

<div><li><a href=""><img src="https://raw.githubusercontent.com/naveen-9697/Handwritten-text-recognition-OCR----IAM-dataset---CNN-and-BiRNN/master/some%20images/g06-037k-01-02.png"/></a></a><h3>all</h3></div></li>

 <div><li><a href=""><img src="https://raw.githubusercontent.com/naveen-9697/Handwritten-text-recognition-OCR----IAM-dataset---CNN-and-BiRNN/master/some%20images/d03-112-01-03.png"/></a></a><h3>Kings</h3></div></li>
 
  <div><li><a href=""><img src="https://raw.githubusercontent.com/naveen-9697/Handwritten-text-recognition-OCR----IAM-dataset---CNN-and-BiRNN/master/some%20images/g07-038-01-02.png"/></a><h3>SGhigraphies</h3></div></li>
  
 <div><li><a href=""><img src="https://raw.githubusercontent.com/naveen-9697/Handwritten-text-recognition-OCR----IAM-dataset---CNN-and-BiRNN/master/some%20images/l04-098-00-06.png"/></a></a><h3>and</h3></div></li>

 <div><li><a href=""><img src="https://raw.githubusercontent.com/naveen-9697/Handwritten-text-recognition-OCR----IAM-dataset---CNN-and-BiRNN/master/some%20images/b05-098-03-06.png"/></a></a><h3>SI</h3></div></li>
 
  <div><li><a href=""><img src="https://raw.githubusercontent.com/naveen-9697/Handwritten-text-recognition-OCR----IAM-dataset---CNN-and-BiRNN/master/some%20images/a01-122-05-06.png"/></a></a><h3>SIt</h3></div></li>
  
 <div><li><a href=""><img src="https://raw.githubusercontent.com/naveen-9697/Handwritten-text-recognition-OCR----IAM-dataset---CNN-and-BiRNN/master/some%20images/a03-030-04-05.png"/></a></a><h3>the</h3></div></li>
 
 <div><li><a href=""><img src="https://raw.githubusercontent.com/naveen-9697/Handwritten-text-recognition-OCR----IAM-dataset---CNN-and-BiRNN/master/some%20images/e04-004-04-01.png"/></a></a><h3>show</h3></div></li>

 <div><li><a href=""><img src="https://raw.githubusercontent.com/naveen-9697/Handwritten-text-recognition-OCR----IAM-dataset---CNN-and-BiRNN/master/some%20images/k04-017-08-07.png"/></a></a><h3>Gcertain</h3></div></li>

</ol>


Yes, the results aren't very promising and only about 58.4% were identified correctly out of all words in the holdout set. And all such mistakes in spellings can be corrected using any language model.<br>
My colab session had crashed (12.72GB of RAM filling up completely) everytime I tried to import pre-trained language model(I was trying to use 'Google Billion words' dataset) to fix these spelling mistakes. For this reason, I have uploaded the jupyter notebooks without having corrected the spellings. And Yes, I do have plans to fix this in the future using cloud VMs.


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
