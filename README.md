# ExtractKeyFrame
It contains two algorithm extracting key frame. Before explaining them, I say something about comparing the similarity of tow images. In the next two algorithms, I use hash number of image to compare the similarity of two pictures. This algorithm is from [](https://blog.csdn.net/fengbingchun/article/details/42153261) . 

## Algorithm 1

It‘s a very simple algorithm to extract key frame.

* Step 1: Extract one frame from each 30 frames.
* Step 2: Compare the frame with the last frame. If they are similar, I discard it. Otherwise, I regard it as a keyframe.
* Step 3: Discard the frame that is nearly black.

**The result of the Algorithm 1:**

![](https://github.com/zjulzy/ExtractKeyFrame/blob/master/testcase/result1.png?raw=true)

## Algorithm 2

Algorithm 2 is a little advanced. I referenced an ancient paper(*Yueting Zhuang, Yong Rui, Thomas S. Huang,*
*Sharad  Mehrotra., Adaptive Key Frame Extraction Using Unsupervised Clustering, IEEE ICIP'98, Chicago, USA, 98.10.*</u> )   But the difference is I compare the similarity of two images by a different method mentioned above.

**The result of Algorithm 2:**

![](https://github.com/zjulzy/ExtractKeyFrame/blob/master/testcase/result2.png?raw=true)

**Last but not least, If you want to run the program in your computer, confirm you have the environment of OpenCV**