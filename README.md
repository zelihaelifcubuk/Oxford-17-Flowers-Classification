# Oxford 17 Category Flowers Dataset - CNN (ResNet based)

[Click for the original dataset](https://www.robots.ox.ac.uk/~vgg/data/flowers/17/)
<br>
<br>
### Libraries 
#### 1.Numpy <br> 2.Matplotlib <br> 3.Seaborn <br> 4.OS <br> 5.PIL <br> 6.Scikit-learn <br> 7.Tensorflow <br> 8.Keras
<br>

In this project, the Oxford 17 Flowers dataset, which is a reduced version of the Oxford 102 Flowers dataset, is used. The dataset is divided for each class: train, validation and test. There are 50 images from each class in the Train dataset, and 15 images from each class in the Validation and Test datasets. Apart from this dataset, a "new test data" folder is created using five images for each class in order to test the model on images that does not see during training.

Images are loaded manually using a user-defined function, not using ImageDataGenerator. Additionally, the images are resized to 224x224. LabelEncoder and OneHotEncoding operations are performed on the class label. ResNet50 model is used and features learned on the ImageNet dataset are included in the project. Accuracy, confusion matrix and classification report are used as performance evaluation metrics.

This dataset is loaded to test the model with new test data. Each time the program is run, it randomly selects one of the 17 classes and randomly selects one of the 5 images in this class. It then tests this image which is chosed on the model. It prints the information on which class it guesses and in what percentage, the actual class information and the image it chooses on the screen. After this process, it displays the graph of the ratio predicted by this selected image for each class.

