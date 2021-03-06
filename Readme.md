## Speech Emotion Recognition
This repository contains our work on Speech emotion recognition using emodb dataset. This dataset is available here [Emo-db](http://www.emodb.bilderbar.info/download/)

### Prerequisites
Linux (preferable Ubuntu LTS). Python2.x 

### Installing dependencies 
Dependencies are listed below and in the `requirements.txt` file.

* h5py
* Keras
* scipy
* sklearn
* speechpy
* tensorflow
* tqdm

Install one of python package managers in your distro. If you install pip, then you can install the dependencies by running 
`pip2 install -r requirements.txt` 

If you prefer to accelerate keras training on GPU's you can install `tensorflow-gpu` by 
`pip2 install tensorflow-gpu`

### Directory Structure
- `speechemotionrecognition` - Package folder which contains all the code files corresponding to package
- `dataset` - Contains the speech files in wav formatted seperated into 7 folders which are the corresponding labels of those files
- `models` - Contains the saved models which obtained best accuracy on test data.
- `example.py` - Contains examples on how to use the package

### Details of the package
- `utilities.py` - Contains code to read the files, extract the features and create test and train data
- `mlmodel.py` - Code to train non DL models. We have three models
	- `1 - SVM`
	- `2 - Random Forest`
	- `3 - Neural Network`
- `dnn.py` - Code to train Deep learning Models. Supports two models given below
    - `1 - CNN`
    - `2 - LSTM`

### Using the package
Look at `example.py` for sample usage.

### Contributing to the repository.
* If you find any problem with the code, please feel free to open an issue.
* Found something you can improve, please send me a pull request with your changes.
I will be more than happy to review and approve them.

### Contacting me
You can send an email to [harry7.opensource@gmail.com](mailto:harry7.opensource@gmail.com)

**Note**: If you find this code useful, please leave a star :)
