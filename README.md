# Automatic Image Labelling

The steps of this process are mentioed below:

1. It uses ResNet50 network pre-trained on ImageNet dataset. 
After discarding the final prediction layer, the activations of the penultimate layer can be used as features to represent the images.

2. The next challenge is to automate the process of deciding the number of classes in the dataset. 
This method uses K-means clustering to to cluster out the datasets belonging to different classes. 
The elbow rule can be used to find the most optimal value for the number of clusters. 

3. After deciding the number of clusters, K-means can be used to divide the datasets into different
classes. The datasets are then saved in different folders depending on the class labels.
