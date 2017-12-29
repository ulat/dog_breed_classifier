[//]: # (Image References)

[image1]: ./images/sample_dog_output.png "Sample Output"
[image2]: ./images/vgg16_model.png "VGG-16 Model Keras Layers"
[image3]: ./images/vgg16_model_draw.png "VGG16 Model Figure"


## Project Overview

This project from the AI Nanodegree builds a pipeline that can be used within a web or mobile app to process real-world, user-supplied images. Given an image of a dog, your algorithm will identify an estimate of the canine’s breed.  If supplied an image of a human, the code will identify the resembling dog breed.

![Sample Output][image1]

## Installation Instructions

To run the code on your local machine, please follow the instructions below.

  - __Clone the repository__ and navigate to the downloaded folder.

        git clone https://github.com/udacity/dog-project.git; cd dog-project

  - __Download the [dog dataset](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/dogImages.zip)__. Unzip the folder and place it in the repo, at location path/to/dog-project/dogImages.

  - __Download the [human dataset](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/lfw.zip)__. Unzip the folder and place it in the repo, at location path/to/dog-project/lfw. If you are using a Windows machine, you are encouraged to use [7zip](http://www.7-zip.org/) to extract the folder.

  - __Download the [VGG-16 bottleneck features](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/DogVGG16Data.npz)__ for the dog dataset. Place it in the repo, at location path/to/dog-project/bottleneck_features.

  - __Install the necessary Python packages__.

    - For Mac/OSX:

        conda env create -f requirements/aind-dog-mac.yml
        source activate aind-dog
        KERAS_BACKEND=tensorflow python -c "from keras import backend"

    - For Windows:

        conda env create -f requirements/aind-dog-windows.yml
        activate aind-dog
        set KERAS_BACKEND=tensorflow
        python -c "from keras import backend"

  - __Open the notebook__.
        jupyter notebook dog_app.ipynb
