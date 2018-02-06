# Semantic Segmentation
This project identifies areas of roadway present in provided images. The project was trained and tested using the [Kitti Road dataset](http://www.cvlibs.net/datasets/kitti/eval_road.php) and the pre-trained network weights from a modified, fully convolutional variant of the VGG16 model.  

### Prerequisites  
 - [Python 3](https://www.python.org/)  
 - [TensorFlow](https://www.tensorflow.org/)  
 - [NumPy](http://www.numpy.org/)  
 - [SciPy](https://www.scipy.org/)  

## Quick Start  
Run the following command to run the project:  
```  
python main.py  
```  

## Documentation  
This implementation of Semantic Segmentation uses pre-trained weights from a variant of the VGG16 deep neural network model where 1x1 convolutional layers are used in place of fully connected layers in the original model. These pre-trained weights are used to initialize a similarly structured classifier aimed at identifying road surfaces in images. The final result excludes most non-road surfaces and includes most road surfaces.
