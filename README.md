# Handwritten Line Text Recognition using Machine Learning with Tensorflow
HandWritingRecogniton is a ML based website that generates text data from the document and images.

### Description
Use Convolutional Recurrent Neural Network to recognize the Handwritten line text image without pre segmentation into words or characters. Use CTC loss Function to train.
More read this

* Project consists of Three steps:
  1. Multi-scale feature Extraction --> Convolutional Neural Network 7 Layers
  2. Sequence Labeling (BLSTM-CTC)  --> Recurrent Neural Network (2 layers of LSTM) with CTC 
  3. Transcription --> Decoding the output of the RNN (CTC decode)

## Other Files
Follow the drive link[here](https://drive.google.com/drive/folders/1TRhRAM4WHQ7qRZpyyo5CV0wami9xDoHE?usp=sharing) to check the video, ppt, and the trained model(after downloading the model save it in the model dir).

# Requirements
1. Tensorflow v2
2. Flask
3. Numpy
4. OpenCv 3
5. Spell Checker `autocorrect` >=0.3.0 ``pip install autocorrect``

#### Dataset Used
* IAM dataset download from [here](http://www.fki.inf.unibe.ch/databases/iam-handwriting-database)
* Only needed the lines images and lines.txt (ASCII).
* Place the downloaded files inside data directory  

Run in Web with Flask
```markdown
$ python upload.py
Validation character error rate of saved model: 8.654728%
Python: 3.6.4 
Tensorflow: 2.0
