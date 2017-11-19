## Udacity Deep Learning Project write_up

![ex_screenshot](./docs/misc/udacity_project01.jpg)
![ex_screenshot](./docs/misc/udacity_project02.jpg)
![ex_screenshot](./docs/misc/udacity_project03.jpg)
![ex_screenshot](./docs/misc/udacity_project04.jpg)

### Fully Convolutional Network
is useful for image classification. If I want to recognize an object I will use a fully connected layer with softmax activation. However, If I need to recognize the object and know where it is. Things change, I have to know not just shape, color but also spacial data.

### Batch Size
I've used default images which is about 4000(4131 by 'ls | wc -l'), so I set 42 batches and 100 epochs.

### 1x1 convolution
1x1 convolution can reduce/increase filters. It is to generate a deeper network without simply stacking more layers. And also It is inexpensive. Due to smaller kernel size(1x1), it causes less over-fitting

References: 
http://iamaaditya.github.io/2016/03/one-by-one-convolution/
https://www.facebook.com/groups/TensorFlowKR/permalink/447826408891756 (Korean)

### Further
I should've collected more datas to get more accurate model. If I have sufficient datas for train, validation. I believe that I would have models.

![ex_screenshot](./docs/misc/5_run6cam1_00064.jpeg)
![ex_screenshot](./docs/misc/5_run6_mask_00064.png)

by comparing these iamges. tensorflow(or keras) makes a model. due to the fact that all datas I have got is for human. It won't follow dogs, cats, but with correct datas It will