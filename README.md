# Text Segmentation with TextTiling Algorithm and BERT

This project implements BERT encoding and TextTiling algorithm with LDA, for topic segmentation of textual data. It segments a document into coherent and non-overlapping
segments based on the depth scores calculated using the algorithm.


## Features

- Tokenization of sentences
- Calculation of coherence scores and depth scores
- Automatic determination of threshold for segmentation
- Segmenting the document into coherent segments
- Generating an output text file with segmented sentences

### LDA approach
-Tokenization, Dictionary, and Bag of Words of sentences to prepare data for LDA model
-LDA generate document-topic and topic-word distributions
-Coherence and Depth score are calculated by using shifted window on sentences
-High depth score and low Coherence score are indications for possible topic shift
-Select appropriate threshold to identify topics boundaries
-Generate a new segmented txt file

#### BERT approach
-Pre-trained and Fine-tuned BERT  MiniLM-L6-v2
-Shifted window on sentences
-Encode windows to a 384 dimensional dense vector
-Calculate Coherence score on the encoded vectors with similar approach
