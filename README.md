# BMEN E4470 Final Project

Deep Learning for EEG Motor Imagery Classification

In this project, two deep learning models are implemented to predict the motor imagery (MI) state from EEG data obtained from the BCI Competition IV-2a dataset (http://www.bbci.de/competition/iv/). The first model is a multi-layer convolutional neural network feature fusion model (MCNN) which consists of four CNNs of varying depths and filter sizes. The output of the four CNNs are concatenated and passed into a multi-layer perceptron (MLP) model to output a prediction score [1]. The second model is known as the EEG-TCNet model which combines the EEGNet (compact convolutional neural network) with a temporal convolutional network (TCN) [2].

Training and evaluation of both models showed that the EEG-TCNet outperformed the MCNN with a 65.9% prediction accuracy for the former and 32.3% for the latter. Possible explanations for the low accuracy of MCNN include overfitting and a lack of pretraining needed to handle a small dataset. Additionally, the MCNN built in this project is a condensed version of that described in the original paper in order to handle memory-related issues in Google Colaboratory.

Sources:
[1] S. U. Amin, M. Alsulaiman, G. Muhammad, M. A. Mekhtiche, and M. Shamim Hossain, “Deep learning for EEG motor imagery classification based on multi-layer cnns feature fusion,” Future Generation Computer Systems, vol. 101, pp. 542–554, 2019.

[2] T. M. Ingolfsson, M. Hersche, X. Wang, N. Kobayashi, L. Cavigelli, and L. Benini, “EEG-TCNet: An accurate temporal convolutional network for embedded motor-imagery brain–machine interfaces,” 2020 IEEE International Conference on Systems, Man, and Cybernetics (SMC), 2020.
