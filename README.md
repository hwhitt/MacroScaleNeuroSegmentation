# MacroScaleNeuroSegmentation
### Machine Learning for Macro-scale Segmentation of Mouse Brain Neuro Scans

<p align="center"> 
<img src="/ResultImages/project_goal.png" width="420" > 
</p>


### Project Goals:    
Given a sub-patch of macro-scale neuro-images, the objective is to classify this small section of an image to a brain area -- hypothalamus (thalamus), striatum, or cortex.

The solution pipeline spanned data augmentation, feature extraction, dimensionality reduction, and classification. Data augmentation was leveraged to generate a dataset with 92,160 total images. Features evaluated included entropy, edge detection, object detection, shape indices, histogram of oriented gradients, and more. Two sets of features were evaluated, the second with more features than the first.   

Multiple dimensionality reduction approaches were iterated over including no reduction, Scaled PCA with 3 components, Scaled PCA with 5 components, Kernel PCA, and Gaussian Random Process. For each of these reductions, Logistic Regression, k-Nearest Neighbors, Decision trees, Linear SVMs, and Kernel SVMs were iterated over for classification.     
Transformations and classification followed a 70-30 train-test split procedure. 

#### Ultimately, the highest achieved accuracy was 97.8% using no dimensionality reduction and a kernel SVM as the classifier. Scores are reported as well as error analysis.

<p align="center"> 
<img src="/ResultImages/example_transforms.png" width="700" > 
</p>

Final Project for COE 3804, Machine Learning for Engineers   
