# ML4HEP Tutorial

Landing page for University of Manchester Machine Learning for High-Energy Physics tutorial, part of a series for the RAEng Google DeepMind ResearchReady programme.

The session motivates the use of machine learning in high-energy physics research, particularly in the context of the Large Hadron Collider.
Several examples of various machine learning technologies, applied to particle physics research, are given.

A set of hands-on exericses are provided.
The main exercises use the [JetClass](https://zenodo.org/records/6619768) dataset, focusing on the classificaton of jet classes using DNNs on high-level jet features and transformers on low-level jet constituents.  See below
A set of introductory exercises aimed at those with less ML (and specifically PyTorch) experience can be found at [Intro2DNN4Physics](https://github.com/els285/Intro2NN4Physics/tree/main/Exercises).


## Main Exercises
Two datasets are available:
* High-level: Skimmed JetClass dataset (.h5 format) with high-level jet features (kinematics and Nconstituents) available [here](https://cernbox.cern.ch/s/HAsUVTx60u7L7TY/).
* Low-level: Skimmed JetClass dataset (.h5 format) with low-level constituent kinematics available [here](https://cernbox.cern.ch/s/4rtGlo1RlFvUNwz).

Each dataset contains a `signal` and a `background` class. The intended goal is to train a DNN on the high-level jet features, and then show how a transformer trained on the low-level features can out-perform the simpler DNN.

Walk-through iPython notebooks are made available:
* [JetClassificationWithDNN](https://github.com/els285/RAEngHEPTutorial/blob/main/JetClassificationWithDNN_public.ipynb). Link to Colab [here](https://colab.research.google.com/drive/1Oq1hIkK740ljFWtiUvHb407FawQwvNYp?usp=sharing).
* [JetConstituentTransformer](https://github.com/els285/RAEngHEPTutorial/blob/main/JetConstituentTransformer_public.ipynb). Link to Colab [here](https://colab.research.google.com/drive/14eGFIv7xFL_jwJkyaSD3WI4sTl3-0OA8?usp=sharing).

It's recommended that you download these and then upload to your own Colab space. Alternatively you can work on your own machine. Or on CSF, but I am not sure how to run an iPython notebook on a GPU instance on CSF - maybe you know.
