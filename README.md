# Flower Classification with Deep Learning (ANN, CNN, VGG16, RNN)

Semester project, Deep Learning course (8th semester), BS Software Engineering,
University of Sialkot. The report is an unpublished research paper:
"An Intelligent Deep Learning Framework for Flower Classification and Medicinal
Knowledge Mapping" (included in this repository as a PDF).

## What this project does
Compares four neural network architectures for multi-class flower image
classification on the same dataset and preprocessing:
- ANN (fully connected baseline)
- CNN (AlexNet-style)
- VGG16 (transfer learning, ImageNet weights, fine-tuned)
- RNN (images reshaped into sequences)

## Dataset
Public Kaggle flower dataset with 14 classes: [Kaggle dataset link].
13,618 training images and 98 validation images. The dataset is not copied
into this repository.

## Results (validation)
| Model | Train accuracy | Validation accuracy | Validation loss |
|-------|----------------|---------------------|-----------------|
| ANN | 45% | 47% | 1.3 |
| CNN (AlexNet-style) | 70% | 67% | 1.2 |
| VGG16 (transfer learning) | 98% | 97% | 0.07 |
| RNN | 45% | 43% | 1.75 |

VGG16 performed best. Note: the validation set is small (98 images), so the
accuracy figures are indicative only.

## Repository contents
- One notebook per model (ANN, CNN, VGG16, RNN)
- A notebook that combines the results into comparison graphs
- The paper (PDF)

## Tools
Python, TensorFlow, Keras, Google Colab.

## Limitations and future work
The medicinal knowledge mapping described in the title (linking each predicted
flower to nutritional and medicinal information) is proposed as future work and
is not implemented here. Other ideas: newer architectures (EfficientNet,
DenseNet, Vision Transformers), a larger validation set, and a mobile or web
application.

Paper (PDF): [Flower Classification with Deep Learning]
(https://github.com/MansoorMaqsood/flower-classification-dl/raw/main/Flower%20Classification%20with%20Deep%20Learning.pdf)

## Author
Mansoor Maqsood, University of Sialkot
