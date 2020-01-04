# PCA-for-CAT-Photos


In this question, you are expected to analyze cat images using PCA. You will use the dataset provided within the homework zip file as cats. The dataset is composed of 5000 images of cats. For this question, use of any library for PCA calculations is not allowed.
Flatten all images of size 64×64×3 to get 4096×3 matrix for each image. Note that all images are 3-channel RGB. Create a 3-D array, X, of size 5000 × 4096 × 3 by stacking flattened matrices of the images provided in the dataset. Slice X as Xi = X[:,:,i] where i corresponds to the first three index. thus obtaining each color channel matrix independently for all images. Reshape all Xi to obtain matrices, instead of 3D arrays.
Question 1.1 [10 pts] Apply PCA on Xi’s to obtain first 10 principal components for each Xi. Report proportion of variance explained (PVE) for each of the principal components. Discuss your results.

Question 1.2 [5 pts] Using the first 10 principal components found for each color channel, reshape each principal component to a 64 × 64 matrix. Stack corresponding principal components of each color channel to obtain 10 RGB images of size 64 × 64 × 3 and display all. Discuss your results.
Question 1.3 [10 pts] Describe how you can reconstruct an original cat image using the principal components you obtained in question 1.1. Use first k principal components to analyze and reconstruct the first image in the dataset where k ∈ {1, 50, 250, 500}.
