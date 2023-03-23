# L4_project - 2439753P
L4 Project at UofG - End to end speech emotion recognition model

Our CNN-LSTM model evaluated on the MSP-IMPROV dataset with 50.29% accuracy.


# Instructions 

The entirety of the code is done using Jupyter Notebook. You will need an environment that is capable of executing these files.
Suggestions: Google Colab/Anaconda
Each notebook is ran by executing the cells in order. 
Warning: Computationally expensive, especially the deep learning notebooks.

File explanation/order of running: Below we describe each notebook. They are listed in order which they should be ran in.

1) model_first.ipynb

This model consists of preprocessing and building the traditional model - it includes analyses of the datasets TESS and MSP-IMPROV, preprocessing them, 
extracting features and building traditional models with finetuning.

2)data generate.ipynb

Simple script which generates two numpy arrays in your local repository, called audios and labels (corresponding to the MSP-IMPROV data and their labels)
These are needed for training the Deep Learning models in the subsequent notebooks

3) CNN + ConvLSTM.ipynb

this notebook contains most of my training and fine-tuning process of the CNN-ConvLSTM network.
NOTE: not 100% cells included, some were reran accidentally, some were lost in the process. Most of the cells are included however.

4) eval base model .ipynb

this notebook includes the evaluation of the traditional model on the MSP-IMPROV dataset

5) Evaluation Model Final.ipynb

this notebook includes the evaluation of the end to end learning model on the MSP-IMPROV dataset


MISC folder: this folder contains multiple jupyter notebooks. These are attempts and experiments with different architectures from when I was learning about building models.
They include different inputs (raw audio, spectrograms, reduced spectrograms), and different architectures (LSTM only, CNN only, CNN-LSTM).

# Requirements:

Dataset is not included as it is too large for submission.
You need to download:
TESS dataset - https://www.kaggle.com/datasets/ejlok1/toronto-emotional-speech-set-tess
MSP-IMPROV dataset - this is not accessible publicly, need to gain access. Official page here: https://ecs.utdallas.edu/research/researchlabs/msp-lab/MSP-Improv.html

The downloaded folders need to be placed in the dataset folder. Apologies if tedious (althought shouldnt be, it is 7 folder moves).

Library downloading commands already included.
notebooks #3, #4, #5 are better ran on google colab than local environment.

