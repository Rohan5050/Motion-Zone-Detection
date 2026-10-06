# Motion-Zone-Detection


 [!Watch Video](https://github.com/user-attachments/assets/6e4dd77f-2ec8-453e-9945-66c8f6d1cae3)


# Overview
Motion-Zone-Detection uses Background Subtraction and Yolo to detect and track moving objects in a user defined specific zone

Background subtraction is a common and widely used technique for generating a foreground mask (namely, a binary image containing the pixels belonging to moving objects in the scene) by using static cameras

How frame gets converted into foreground mask ?

-> Each pixel independently builds a memory of the colors it usually sees. When a new frame arrives, it immediately outputs white if the color is unfamiliar and black if it's familiar. Unfamiliar colors that persist get gradually absorbed into that memory, so a stationary object fades to black over many frames.

Document References

1. https://docs.opencv.org/5.0/tutorials/others/background_subtraction.html#how-to-use-background-subtraction-methods

2. https://docs.opencv.org/5.0/py_tutorials/py_imgproc/py_contours/py_contours_begin/py_contours_begin.html#contours-getting-started

3. https://medium.com/@itberrios6/introduction-to-motion-detection-part-3-025271f66ef9

4. https://docs.ultralytics.com/guides/trackzone

5. https://docs.ultralytics.com/datasets/detect/coco
