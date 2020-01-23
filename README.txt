This file contains some notes for the code to do the basic video analysis

1. [framewok.png] is a brief introduction of the current framework.

2. [video2image.ipynb] contains the code to read video and store the frames. The reason we include this step in our current framework is because we can check the specific image if we find some ‘interesting’ results from certain algorithms. One direct drawback of this is it will need some space to store all the frames especially when we have a long video. One way to reduce the required space is to decrease the image quality (parameter `img_quality` in function `video_to_image2`).

3. [laptimes.ipynb] contains the code to compute image similarity and estimate laptimes. Some steps are splited into different parts to expedite the computation.

4. [detection.ipynb] contains the code to detect objects directly from the video and do some basic analysis frame by frame. Some examples are included in the notebook.

5. [objects.npy] contains some information of the detected objects from an example video. It is used in one of the example in the [detection.ipynb]. It could take some times to obtain such information from a given video. One could refer to the codes that are commented out in [detection.ipynb] to parallelize the procedure.

6. We use some pre-trained network model to do the object detection, which could be found in (https://github.com/OlafenwaMoses/ImageAI/blob/master/imageai/Detection/README.md)





For any questions, please contact Cong Mu (cmu2@jhu.edu)