# Sign-to-speech-Language
Here is a GitHub README file for the "Sign2Speech" project based on the content from your project report:

---

# Sign2Speech

Sign2Speech is a deep learning-based project aimed at bridging the communication gap between the hearing-impaired community and the general public by translating American Sign Language (ASL) gestures into spoken English.


## Introduction

Effective communication is vital for social integration and personal development. However, individuals with hearing impairments face challenges in using traditional spoken language. Sign2Speech leverages deep learning to facilitate communication between the hearing-impaired community and the general public by converting ASL hand signs into spoken English.

## Data Description

The dataset consists of images of ASL alphabets, each representing a different class. Originally comprising 87,000 images of size 200x200 pixels, the dataset was reduced for computational efficiency, using 100 images per alphabet for training.

## Data Visualization

The dataset was processed using NumPy arrays and organized into a Pandas DataFrame for clarity and efficiency in data handling. A total of 2,730 images were used in the project.

## Model Architecture

Sign2Speech utilizes a Convolutional Neural Network (CNN) for feature extraction and a recurrent neural network for sequence modeling. Key components include:

- **Input Layer**: Accepts 200x200 RGB images.
- **Convolutional Layers**: Extracts low-level features with filters and applies Rectified Linear Unit (ReLU) activation and max-pooling.
- **Dense Layers**: Identifies complex patterns with fully connected layers, leading to class probabilities.
- **Output Layer**: Generates a probability distribution over 27 classes, corresponding to ASL alphabets and space.

## Training and Evaluation

The model was trained over 5 epochs with a batch size of 32. The training process achieved approximately 97.27% accuracy on the test data.

## Discussion

The Sign2Speech project demonstrated high accuracy in recognizing ASL gestures. However, it currently cannot operate in real-time using webcam inputs. Enhancing real-time capability would significantly increase its practical applicability.

## Future Work

Future improvements include:
- Expanding the dataset with more diverse images.
- Incorporating data augmentation, transfer learning, and attention mechanisms.
- Optimizing for real-time performance with hardware accelerators.


