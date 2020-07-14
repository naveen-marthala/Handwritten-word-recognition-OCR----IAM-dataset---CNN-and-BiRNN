This project is about recognising handwritten words with CNN and Bi-directional LSTM, decoded with CTC.

## Dataset:

The IAM Handwriting contains:  
115,320 isolated and labeled words by 657 writers.

link to <a href=http://www.fki.inf.unibe.ch/databases/iam-handwriting-database>IAM words dataset</a>. 

## Results:
<table style="width:100%">
  <tr>
    <th>Character-Error-Rate</th>
    <td>  %</td>
  </tr>
  <tr>
    <th>Word-Error-Rate</th>
    <td>  %</td>
  </tr>
</table>

## Training:
Trained on GPU(Tesla P100-16GB) on Google Colab.
Training the final model took close to 4 hours with <a href=https://www.tensorflow.org/api_docs/python/tf/keras>tensorflow.keras</a>

## Usage:
-- <i>pending and will be filled</i> --

## References:
<ol>
  <li>Architecture inspired from <a href=https://arxiv.org/pdf/1507.05717.pdf>this paper</a>.</li>
  <li>CTC Loss function from <a href=https://towardsdatascience.com/intuitively-understanding-connectionist-temporal-classification-3797e43a86c>this article</a>.</li>
</ol>
