# SRCNN
Image Super-Resolution Using Deep Convolutional Networks
<br />
Applying super resolution strategies to sattelite imagery
1. The SRCNN Network
In SRCNN, actually the network is not deep. There are only 3 parts, patch extraction and representation, non-linear mapping, and reconstruction as shown in the figure below:

![image](https://user-images.githubusercontent.com/106013751/169710536-07145630-b5a6-4864-a653-c80f797d2663.png)

2. Loss Function

![image](https://user-images.githubusercontent.com/106013751/169710551-d222c76a-7db6-4525-a664-ac8a3a1ed99b.png)

3. Relationship with Sparse Coding

![image](https://user-images.githubusercontent.com/106013751/169710582-97855376-48d4-41f4-a9ac-91c03e026064.png)

For Sparse Coding (SC), in the view of convolution, the input image is conv by f1 and project to onto a n1-dimensional dictionary. n1=n2 usually is the case of SC. Then mapping of n1 to n2 is done with the same dimensionality without reduction. It is just like a mapping of low-resolution vector to high-resolution vector. Then each patch is reconstructed by f3. And overlapping patches are averaged instead of adding together with different weights by convolution.
For super resolution, the loss function L is the average of mean square error (MSE) for the training samples (n), which is a kind of standard loss function.

Results: 

![](https://github.com/WarrenGreen/srcnn/blob/master/results/05953_combined.jpg)
![](https://github.com/WarrenGreen/srcnn/blob/master/results/05454_combined.jpg)
![](https://github.com/WarrenGreen/srcnn/blob/master/results/06006_combined.jpg)
