# DeepLearningInVision_InfraredPics

Here I summarize the learnings from Lars Hubacher and his team on the use of deep learning on the binary classification problem defined [here](https://zenodo.org/record/5783947#.YhNy1y8w30o).

# Summary #
| Model | Implementation | Notes |
| ----- | -------------- | ----- |
| Classical (LeNet-5) | [Keras_Tuner.ipynb](ConvNet_from_Scratch/ConvNet_from_Scratch/Keras_Tuner.ipynb) | Models with different number of neurons and depth |
| Classical (LeNet-5) | [Sandro_Deep_Learning.ipynb](ConvNet_from_Scratch/ConvNet_from_Scratch/Sandro_Deep_Learning.ipynb) | Models with different number of neurons and dropout settings, testing different train/test splits |
| Feedforward | [NN.ipynb](NN/NN.ipynb) | Feedforward NNs can learn if trained enough |
| All of those under `keras.applications` | [#1_benchmarking_kerasmodels.ipynb](Pretrained_CNN's/#1_benchmarking_kerasmodels.ipynb) | 27 models, reaching ~0.90 accuracy |
| All of those under `keras.applications` retraining one of the FC layers | (See presentation) | 27 models, reaching ~0.92 accuracy |
| mobilenetV2 | [#2_mobilenetV2.ipynb](Pretrained_CNN's/#2_mobilenetV2.ipynb) | Not clear if it worked out |
| ResNet50 | [#3_ResNet50.ipynb](Pretrained_CNN's/#3_ResNet50.ipynb) | Not clear if it worked out |

# Tools # 
* [TensorFlow](https://www.tensorflow.org)
* [KerasTuner](https://keras.io/keras_tuner/) 
* [TensorBoard](https://www.tensorflow.org/tensorboard)
* python standard library
* [pandas](https://pandas.pydata.org)
