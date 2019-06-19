<h1>Segmentation method for crop UAV images</h1>

Agriculture is a primary activity that supports human life, these is key in the sustainability and development of civilization in general, today facing major challenges. 

A critical and essential step to analyze plant images with computer vision is the plant segmentation, that is, separating the green plant material or region of interest from the background. 
This study proposes a segmentation method for crop UAV images. The dataset used will be images areas of drones in crops.

<b>Types of images</b>

![Fig001](https://user-images.githubusercontent.com/29265084/58557295-6bacc980-81f4-11e9-814c-0b1d5049fa7c.png)

![Fig002](https://user-images.githubusercontent.com/29265084/58557354-9434c380-81f4-11e9-99d4-0b90c4b9795f.png)

<h2>The method</h2>

The proposed method has four stages, the aim of each one is improve the image for next step, to get this aim the image is initially transformed to the color space YCrCb where the Cr channel is separated and used in next step. A feature network transforms a Cr image to  feature vector f based in backpropagation neural network. A squared window of 41 pixels is sliced over the image and extracted it histogram, after this normalize the f vector and used to score a PCA(Principal Component Analysis) previously computed, if the score value is in the interval for tree, the pixel is valuated to 1, else is 0 valuated. This steps is explained in more detail in next subsections.  


![Fig003](https://user-images.githubusercontent.com/29265084/59731927-8932e900-921e-11e9-8d79-85368d44d210.png)

<h2>Descriptor for Texture Classification</h2>

A novel neural network based image descriptor for texture classification is an interesting new texture descriptor generator for tree classification in UAV's images. For validation, the method uses three free texture datasets: UIUC, Outex and USPtex. The classification accuracies were calculated as 90.82%, 89.62% and 93.83% for these data sets respectively.The method is inspired by feed forward neural network and the main objective is to show feature extraction ability of the neural network. This descriptor consists of 3 x 3 overlapping blocks division, creating feature extraction network by using row and column pixels of the block, calculating feature value, normalization and histogram extraction. Firstly, image is divided into 3x3 size of overlapping blocks and pixels of each block are selected to create feed forward networks, Fig.~\ref{fig:Novel Network for texture clasification} shows a configuration for blocks and neural network.


![Fig004](https://user-images.githubusercontent.com/29265084/59731993-da42dd00-921e-11e9-841f-4aff4eb7a042.png)
