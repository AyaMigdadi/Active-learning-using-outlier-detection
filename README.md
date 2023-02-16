# Active-learning-using-outlier-detection
### An Active Learning Framework with A Novel Query Strategy Based on Outlier Detection
Most of the existing deep learning algorithms acquire competitive results based on the presumption that the pre-labeled dataset is generally quite abundant and can be fed to the training all at once. However, such presumptions are not confirmed with real-world scenarios as many applications do not guarantee the abundance of labeled data. Blindly pursuing to direct the manpower to annotate the available unlabeled data is an unfeasible and unwise solution causing an actual hurdle. The most compelling option to mitigate this drawback entails shedding some light on an approach capable to employ such infrequent data professionally as well as preserving and achieving impressive results, which can be found in Active learning (AL) techniques. The goal of Active learning is to generate an algorithm that efficiently selects maximally-informative samples to be labeled by an oracle. Such samples guarantee to preserve the performance of the model as if it was trained using a larger (complete) training dataset. This research proposes a novel Active Learning framework. The proposed Active Learning framework reduces the amount of data required for training an image classification model. The proposed AL pipeline consists of an AL query strategy and baseline deep learning classifier. The query strategy selects the most informative data points from a pool of unlabeled data. These points train the baseline classifier, which learns to classify new points. The novelty in this work falls into three folds. The first fold stands for selecting the initial training data of the baseline classifier that preserve the distribution of the original unlabeled data. In the second fold, the outlier detection (OD) functions are appointed as acquisition functions. To the best of our knowledge this is the first work that used OD as a query strategy in AL. The last fold seeks to give the DL classifier more robustness and effectiveness by combining it with Incremental Learning, which continuously updates the classifier to makes it adaptive to newly coming samples in each iteration. We tested our AL approach using Convolutional Neural Network (CNN), ResNet18, and LeNet5 with two dataset sets (MNIST and FashionMNIST). The experimental results show that the proposed framework outperforms other AL approaches. 









This project contains 4 main folders 
•	1MNIST 
•	2FASHION
•	Comparing
•	Visualization (Core_set and Outliers)



(1Mnist & 1Fashoin) folders contain 3 subfolders:
CNN
LeNet
ResNet 
Each subfolder contains the code to run (the proposed AL framework) based on the specific architecture (CNN, LeNet, or ResNet). Moreover, it contains the code of applying the specific architecture over the all set used (MNIST or FASHOINMNIST)


Comparing folder contains the code to compare the implementation of the proposed AL by using different classifiers (CNN, LeNet, or ResNet)


The visualization (Core_set and Outliers) folder contains the code for visualization of the embedding distribution of initial selected data, The embedding distribution of core-subset, and The embedding distribution of outlier points. 
