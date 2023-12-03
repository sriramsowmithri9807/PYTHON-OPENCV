
                                            PROJECT APPROACH                        
OpenCV is a library of programming functions mainly aimed at real-time computer vision.

In this article, we will see how to get the objects of the same color in an image. We can select a color by slide bar which is created by the cv2 command cv2.createTrackbar.

Libraries needed:
OpenCV
Numpy
Approach:
First of all, we need to read the image which is in our local folder using cv2.imread( ). For filtering a specific color we need to convert image into HSV format which is hue, saturation, and value and mask the image using cv2.inRange( ) by providing lower and upper bounds of RGB values we wanted to filter which gives us a black and white image where the images with the color of our interests are in white and remaining are in black. we can get back the images with the specified color which we gave it by trackbar by doing cv2 bitwise_and operation.