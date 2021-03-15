# Project - Udacity Data Scientist Nanodegree Capstone: Dog Breed Classifier

## Blog Post with more information:
https://sgdantas1.medium.com/udacity-capstone-project-dog-breed-detector-a93cf5d7112


## Project Overview
The goal of this project is to use Convolutional Neural Networks (CNNs) to build a image classifier pipeline. We started by very simple models, then we used transfer learning to leverage the pre-training from very deep networks.

Our classifier identifies the dog's breed of a dog image or, if it's a person, which breed resembles the picture. 

## About the data
The data was provided by Udacity, it consists of:
- 8351 dog pictures, divided into 133 breeds
- 13233 human pictures

### Motivation
In this project, Udacity in collaboration with Figure Eight provides a data engineering project. The goal was to analyze disaster data from Figure Eight to build a model for an API that classifies disaster messages and use Flask to visualize the data.

<a name="file_structure"></a>

### File Structure
    .
    ├── saved_models     
    │   ├── weights.best.from_scratch.hdf5  # trained model built from scratch
    │   └── weights.best.inception.hdf5     # trained model using inception weights
    │   └── weights.best.VGG16.hdf5         # trained model using VGG16 weights
    ├── haarcascades                   
    │   ├── haarcascade_frontalface_alt.xml # XML file for use with the OpenCV face detector class
    ├── images                              # images used to test the algorithm's predictions
    ├── dog_app.html                        # jupyter notebook saved in html format
    ├── dog_app.ipynb                       # jupyter notebook saved in ipynb format
    ├── extract_bottleneck_features.py      # python script with provided functions
    ├── LICENSE.txt                         # license text
    ├── CODEOWNERS                          # owners of the code
    └── README.md


<a name="instructions"></a>

### Instructions
1. Clone the repo
2. Download bottleneck_features files (see blog for more information)
3. Have fun



### Conclusions
- The goal was to have a model with accuracy greater than 60%, we managed to achieve 80%! This project was pretty fun and I believe learning about transfer learning is particularly important nowadays. This is the state-of-the-art approach for most computer vision and language models!

Of course, we can still improve our model. Here are some suggestions:
- Train the model with extra data, this can be done by getting more data or using data augmentation (rotation, zooming, etc)
- We could also train the model with some added noise in the images, this way the features extracted by the model should be more robust and less affected by the lighting of the image or similar factors
- We could also use more than one model for the final prediction, i.e., using an ensemble of models. This way, the final output would be the average output of each individual model. This way, we hope to avoid some biases that are developed when training each model.


<a name="acknowledgements"></a>

### Acknowledgements
- [Udacity](https://www.udacity.com/) for providing the data and guidelines to complete the project.

