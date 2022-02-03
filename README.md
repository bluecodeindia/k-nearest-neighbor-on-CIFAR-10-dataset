# k-nearest-neighbor-on-CIFAR-10-dataset

1. Download the data CIFAR-10 dataset and extract in the data folder.

2. The CIFAR-10 dataset has 50,000 images for the training and 10,000 images for the test.

3. Each image size is 32 x 32 pixels.

4. First you need to create a python dictionary and set the following parametrs:
  - num_folds: number of k in k-cross validation.
  - k_choices: number of k for the nearest neighbour.
  - data_dir: set the path of your CIFAR-10 dataset.
  
5. Create the object of the class and provide the dictionary to initialize.
  > classifier = KNearestNeighbor(dictionary)
  >
6. The following line will automatically load the data from the path provided by you.
  > classifier.loadData()
  
7. The following line will show you the sample images.
  > classifier.visualize()
  
8. Now you need to check the results of the k-fold cross validation.
  > classifier.crossValidation()
    
9. The following could be used for the testing of the model by providing number of k for nearest neighbour.
  > classifier.fit(k)
