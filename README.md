# Modeling Human Perceptual Inference with the Drift Diffusion Model and Neural Networks (NeuromatchProject)

## Abstract
Bayesian principles have been applied to model human perceptual estimation (Laquitaine et al.). Subjects were tested in a motion direction estimation task where motion evidence strength and priors were manipulated. The mean and variance of estimates agreed with a Bayesian model, but full estimate distributions were bimodal, violating Bayesian predictions. A Switching model that chooses between prior and evidence better fits the data. The results suggest that human perceptual inference follows Bayesian principles on average but uses a heuristic approximation that does not fully integrate priors and likelihoods. This shows optimal Bayesian computations may be approximated in the brain through simpler mechanisms.
The Drift Diffusion Model (DDM) is a mathematical framework used to model the decision-making processes in cognitive psychology and neuroscience. It provides a theoretical account of how humans and other organisms make simple perceptual decisions in a **Binary** scenario, where they should choose between two alternatives based on sensory evidence.
Now we are trying to fit the Drift Diffusion Model to behavioral data obtained from decision-making experiments to estimate parameters like the drift rate, decision threshold, and non-decisional components (e.g., motor response time) and finally model human decision-making in perceptual inference. As our main dataset and its experiment have conditions of DDM, which are fast, and uncertain, we only need to binarize the decisions here. Several important parameters like drift rate(v), threshold(a), bias(z), and non_dicision time(t) should be defined. Useful features like reaction_time, prior mean, and trial time exist in the dataset that can be helpful in our modeling process. We also modeled the human perceptual inference using deep neural networks for further experiments.

## Modeling the Laquitaine & Gardner database on human motion direction estimation errors

![Image](https://github.com/sajjadrezvani/NeuromatchProject/assets/100838219/7297ade6-d3cd-4570-95d3-891e8ff8a205)

![Image](https://github.com/sajjadrezvani/NeuromatchProject/assets/100838219/ff398a18-5d88-44c1-be2e-2ee0dd34142b)

![Image](https://github.com/sajjadrezvani/NeuromatchProject/assets/100838219/12e87e42-2eac-44a8-be80-30435866eba6)

![Image](https://github.com/sajjadrezvani/NeuromatchProject/assets/100838219/b7870918-c61a-49eb-889d-2b502aa44479)

## Dataset Overview

![Image](https://github.com/sajjadrezvani/NeuromatchProject/assets/100838219/a4fd5b6a-7433-4634-aa5c-e71bfc35615e)

## Modeling

### Results of the Logistic Regression Model for Predicting the Decision-Making Process between Prior and Sensory Evidence

![Image](https://github.com/sajjadrezvani/NeuromatchProject/assets/100838219/99d22f0c-51f1-416d-8863-c11ccb8cec94)

### Neural Network Model Architecture

![Image](https://github.com/sajjadrezvani/NeuromatchProject/assets/100838219/d1a3dbff-5b02-46e3-8d33-aa2446b3f155)

### Neural Network Model Learning Curve

![Image](https://github.com/sajjadrezvani/NeuromatchProject/assets/100838219/c4b967fe-4f0e-409e-9325-92a03e715194)

### Modeling the Reaction Time (RT) using the Drift Diffusion Model (DDM)

#### 0.06 motion coherence
  ![Image](https://github.com/sajjadrezvani/NeuromatchProject/assets/63340593/1f96a427-94e3-4fca-b18a-b8bfe0ba687b)

#### 0.24 motion coherence
  ![Image](https://github.com/sajjadrezvani/NeuromatchProject/assets/63340593/806bb50d-d7cf-43e1-856b-2123f04eab3f)


# Acknowledgements
We would like to express our gratitude to the contributors of the paper ["A Switching Observer for Human Perceptual"](https://github.com/sajjadrezvani/NeuromatchProject/blob/575a6231e687591b4ee58bd4b08ce8f1af0cda84/Related%20Works/A%20Switching%20Observer%20for%20Human%20Perceptual.pdf) 
for their valuable work and for making their datasets publicly available for research purposes. We acknowledge their efforts in collecting the data, which greatly contributed to the development of our model.

We also thank the organizers of the Neuromatch Academy for providing the opportunity to conduct this research. Their dedication to studying and working in the field of computational neuroscience has been a driving force behind our project.
