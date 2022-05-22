# SRCNN
Image Super-Resolution Using Deep Convolutional Networks
<br />
Applying super resolution strategies to sattelite imagery
1. The SRCNN Network
In SRCNN, actually the network is not deep. There are only 3 parts, patch extraction and representation, non-linear mapping, and reconstruction as shown in the figure below:

![image](https://user-images.githubusercontent.com/106013751/169710536-07145630-b5a6-4864-a653-c80f797d2663.png)

2. Loss Function

![image](https://user-images.githubusercontent.com/106013751/169710551-d222c76a-7db6-4525-a664-ac8a3a1ed99b.png)

For super resolution, the loss function L is the average of mean square error (MSE) for the training samples (n), which is a kind of standard loss function.
Results: 

![](https://github.com/WarrenGreen/srcnn/blob/master/results/05953_combined.jpg)
![](https://github.com/WarrenGreen/srcnn/blob/master/results/05454_combined.jpg)
![](https://github.com/WarrenGreen/srcnn/blob/master/results/06006_combined.jpg)
