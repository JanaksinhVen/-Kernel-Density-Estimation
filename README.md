# Kernel-Density-Estimation
The question answer format repository for use of Kernel Density Estimation for Bounding Box problem

## Task-1 :
Implement Kernel Density Estimation (KDE). Your KDE should include the
following functions
* allows selection from the following kernels: box, gaussian, triangular
* fit data
* select appropriate bandwidth using the pseudo-likelihood method
* evaluate the density given an input x
* visualize the data and the estimated pdf. For this you can assume that
the function will be used only when input dataset is 1-D or 2-D.
The KDE should support n-dimensional input, so don’t write your code assuming 1-D data.
## Task-2 :
The task was to determine the optimal horizontal and vertical Euclidean distance thresholds between
bounding boxes containing words on a document page. The objective of this
task is to establish connections between boxes within a paragraph while ensuring that boxes across paragraphs and columns remain unconnected. Attached
are illustrative examples showcasing the desired box connections and a sample
visualization of the expected output [ATTACHMENT](https://iiitaphyd-my.sharepoint.com/:f:/g/personal/nitin_shrinivas_students_iiit_ac_in/EjVu2YV5MKVAnYPhu_Ua1GoBI9R4a4x3j_LMEUZq2ATXmw?e=Gh0azK).  
You have also been given the following scripts -
* Script to visualize the enclosing boxes.
* Script to visualize the connecting boxes. The input for this script is a data
frame object with the following attributes.
* – ID: The ID number of the word which is in int datatype.
* – Top-Left, Bottom-Right, Top edge center, Bottom edge center, Right
edge center, Left edge center: A list containing the x and y coordinates of the respective coordinates as understood by their attribute
names.
* – Top box, Bottom box, Right box, Left Box - A list containing the distance and id of the nearest neighbor in the Top, Bottom, Right, and
Left directions respectively. HINT - To remove the connection
make sure that the list is [-1, 0].

Using the KDE implemented in the previous task, estimate the appropriate
horizontal and vertical thresholds to apply to the distances between the boxes,
such that boxes within the same paragraphs are connected and there are no
connections to boxes in other paragraphs.  

For any 4 images of your choice from the dataset, experiment with different
bandwidths . Visualize the density estimated and thresholded document for
each of the hyperparameter settings per image.  

Note: If you have 4 hyperparameter configurations, you should have 12 figures
for each (2 density estimation curves (horizontal and vertical distances) along
with the final output image) for each hyperparameter setting  

Visualize and compare the generated output for the following images given by
your KDE with the best hyperparameter configuration with the output obtained
from your solution. The images are listed below :
* 29.jpg
* 68.jpg
* 145.jpg
* 201.jpg
* 232.jpg
* 250.jpg
Note : You should visualize the output images side by side for each
test image
