#### Final Project for [Human Data Analytics course](http://www.dei.unipd.it/~rossi/), a.y. 2019/2020

#### University of Padua - Department of Mathematics

# Locomotion modes recognition on subsets of Opportunity dataset

*Alberto Bernardi* \
alberto.bernardi.6@studenti.unipd.it

*Stefano Della Morte* \
stefano.dellamorte@studenti.unipd.it


## Description
Human activity recognition (HAR), and in particular modes of locomotion recognition through 
wearable sensors, has been a widely faced task because of its broad applicability. 
A central aspect to be kept in mind is represented by the intrusiveness of the sensors, that should never affect the daily living of whatever kind of user.
As a consequence, it is of capital importance being able of selecting and placing the most limited number of sensors that are still representative of the whole dynamic. 
We particularly focused on this purpose, using the UCI Opportunity dataset and by comparing how this reduction affects different models.
We considered deep learning architectures, employing both 1-D and 2-D Convolutional Neural Networks and Recurrent Neural Networks variously combined. 
In addition, we distinguished two processing pipelines, willing to capture both the spatial and temporal correlations among the data.
The results suggest how a strong reduction of the sensors considered is possible at the cost of a tiny reduction of the performance.
This might be huge for any type of application, guaranteeing to the user a seamless experience, not conditioned nor disturbed by the on-body sensors.


## Instructions
The code is structured as follows:
* `Preprocessing.ipynb`: the preprocessing and segmentation stages. In its conclusion the preprocessed and segmented datasets (train-validation-test) must be pickled to a local or remote machine, since the pickled files are not included in this repository;
* `Models.ipynb`: models definition and a brief evaluation section. In addition, the user can also subset the dataset using a specific function (indeed the dataset is stored as a np.ndarray);
* `Comparison.ipynb`: compare several models performances with plots.

Futhermore, the user can find also:
* default pretrained models (addressed in the report) in `./models/`;
* exported plots of the default models in `./plots/`;
* scores tables for default models in `./scores`.

For obvious reasons, no dataset is included in the directory, but can be downloaded and exported after preprocessing and segmentation inside the `Preprocessing.ipynb` notebook.

Finally, the notebooks can be accessed also on Google Colab (barring authors decisions) at the following links:
* [Preprocessing](https://colab.research.google.com/drive/1iNZN0DZq9I8prnEf07IbGHEVx0bHHGwi?usp=sharing);
* [Models](https://colab.research.google.com/drive/11YslYdPONF6ajAnnB-actRCkZrFdelp_?usp=sharing);
* [Comparison](https://colab.research.google.com/drive/1iNZN0DZq9I8prnEf07IbGHEVx0bHHGwi?usp=sharing)
