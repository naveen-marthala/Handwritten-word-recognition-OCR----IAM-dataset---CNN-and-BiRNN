<ol>
<li>include an unknown token.</li>
<li>why was a custom loss function chosen, instead of something like cross entropy averaged over time?</li>
<li>decision between LSTMs and GRUs. and why only 2 of them were used?</li>
<li>what was the sequence length for LSTMs; and what was done for sequences that weren't lengthy enough and how the padding was handled.</li>
<li>change the network layout to use encoder-to-decoder version of many-to-many RNN, instead of plain many-to-many RNN.</li>
<li>do not use custome loss layer and complicate things, use the one built in tensorflow 2</li>
add a very detailed readme file, with links to
<li>description of the data and where to find it?</li>
<li>how the data was pre-processed and why seperate split (text) files were created?</li>
<li>decisions behind the architecture and loss function? how and where this was trained? (also include/point to the image of architecture)</li>
<li>Then finally include a language model to correct spelling mistakes in inferred words?</li>
<li>how this can be resued? (include functions to pre-process an image for inference and for inference from command line)</li>
<li>include all that didn't work or wasn't working in a seperate branch. e.g. optimised to different loss function and another RNN type(only include GRU or LSTM in master branch)</li>
<li>also include the picture of the architecture</li>
<li>include re-usable code and requirements.txt file</li>
  <li>changed readme.md</li>
</ol>
