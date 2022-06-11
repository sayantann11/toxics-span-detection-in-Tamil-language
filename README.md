# toxics-span-detection-in-Tamil-language
Identification of offensive speech has become
an interesting and an important area of research
and has gained limelight in recent years. With
the development of several models, it has become way easier. Social media plays a crucial
role in identifying the offensive content. Identifying offensive spans is helpful in many ways.
In order to identify offensive spans from the
data set released as part of the shared task, the
Bidirectional Long Short-Term Memory (BiLSTM) model with different layers has been
done by us. This includes word embedding
with the help of Glove twitter data, extraction
of toxic comments from each text line and conversion of spans into sequences is done using
tweet tokenizer

# Methodology
After loading the data into the workspace, we have
applied various pre preprocessing techniques such
as tokenization and word embedding on the dataset.
Glove Twitter Data was used for word embedding.
While building the model, Bi directional Long
Short-term Memory was used along with Conditional random fields and for building our model,
the input dimensions are taken as number of words,
the output dimensions are embedding dimensions.
Also the embedding initializer is embedding matrix. The input length is the max length which has
the length of 100. We also took a dropout layer
with values 0.1. In model building (Bidirectional
LSTM) the value of the recurrent dropout is 0.1. In
time distributed function, a dense layer is layer is
taken with activation function ’relu’ and output is
generated with the help of the CRF model.
