## Traditional Decor Patterns  

More information and complete notebook 
[![](https://mateuszgrzyb.pl/wp-content/uploads/2017/07/kaggle-logo-transparent-300.png)](https://www.kaggle.com/olgabelitskaya/traditional-decor-patterns)  

#### Content

The main dataset (decor.zip) is 485 color images (150x150x3) of traditional decor patterns and the file with labels decor.csv. Photo files are in the .png format and the labels are integers and values.

The file DecorColorImages.h5 consists of preprocessing images of this set: image tensors and targets (labels).

**I encourage you to use kaggle kernel, You can find it here: [Kaggle](https://www.kaggle.com/rafalb/transfer-learning-and-image-preprocessing-94)**  

#### If you want to use this script for Your own follow instruction :   

**In order to work properly, you should have**  

| Plugin | README |
| ------ | ------ |
| NumPy | [Getting NumPy](http://www.numpy.org/) |
| Pandas | [Pandas Library](https://pandas.pydata.org/) |
| SciKit-learn | [http://scikit-learn.org/stable/install.html](http://scikit-learn.org/) |
| TensorFlow | [Installing TensorFlow ](https://www.tensorflow.org/install/) |
| Keras | [Installation](https://keras.io/#installation) |
| H5py | [Installation](http://docs.h5py.org/en/latest/build.html)|
If You want to use virtual machine for first time check this : [Environment](https://github.com/dataworkshop/course_env)  


* Download data : https://www.kaggle.com/olgabelitskaya/traditional-decor-patterns/data  
  
* Clone or download github folder with jupyter notebook and pretrained weights.
  
* Create new folder 
> 'input/traditional-decor-patterns'   and unzip kaggle dataset there.  
  
* Go to **Create predict models** in jupyter notebook and click on *Xception model with frozen all layers*.  
  
* Change weights in baseModel  
``` python
baseModel = Xception(weights='imagenet', 
                        include_top=False,
                       input_shape = (197, 197, 3))
```

* If You want to test Model with existing images create folder  and unzip images
> '../input/traditional-decor-patterns/decor'   


  
