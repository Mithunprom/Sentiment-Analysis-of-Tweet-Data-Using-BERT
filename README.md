<h1>Arthor:</h1>
<p1>Mithun Ghosh</p1>
<h1>Instruction for use: </h1>
<p1>Run the following <a href="nn.py">python file.</a> </p1>
<p2>The project description is described by <a href="SemEval2018-Task1-task-description.pdf">Saif <i>et al.</i>(2008)</a>. </p2>

# Sentiment-Analysis-of-Tweet-Data-Using-BERT
<p1>This project is about using the sentiment analysis of the tweet data by using the Bidirectional Encoder Representations from Transformers (BERT). BERT is a deeply bidirectional, unsupervised language representation, pre-trained using only a plain text corpus. Context-free models such as word2vec or GloVe generate a single word embedding representation for each word in the vocabulary, where BERT take into account the context for each occurrence of a given word.</p1>
<p2>Tweete sentiment, which includes an array of subtasks
on inferring the affectual state of a person from
their tweet. Only the English tweets are modeled in this project, although it can be easily extendes for other languages that described by <a href="SemEval2018-Task1-task-description.pdf">Saif <i>et al.</i>(2008)</a>. This method outperforms any other state of the art techniques for this datasets. However, stacking a multilayer BERT can furthur improve the performance, which will be considered for the future task. </p2>

##Steps to the modeling:
<ul>
  <li>The code can be run on Goggle Colab, where free memory and TPU can be used.
  The datasets include:<a href="2018-E-c-En-train.txt">train</a>, <a href="2018-E-c-En-dev.txt">validation</a> and <a href="2018-E-c-En-test.txt">test</a> data.
  Also, the BERT model of <a href="https://tfhub.dev/google/bert_uncased_L-12_H-768_A-12/1">large uncase</a> is run on Goggle Colab TPU mode.</li> 
<li> The datastes are tokenized and padded by bert hub model and ultimately converted into desired features for the bert model to be used. </li>
  <li> The number of layer in ther bert is fine tunned which preceded by a sigmoid layer (perhaps some more Relu layers in the middle) as the output layer. Overfitting is reduced by Early Stopping on the validation dataset. </li>
  <li> The best model is saved and later used to predict on the test dataset.</li>
  </ul>
