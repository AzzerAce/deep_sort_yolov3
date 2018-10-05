
# Introduction
  Thanks for these projects, this work now is support tiny_yolo v3 but only for test, if you want to train you can either train a model in darknet or in the second following works. It also can tracks many objects in coco classes, so please note to modify the classes in yolo.py. besides, you also can use camera for testing.

  https://github.com/nwojke/deep_sort
  
  https://github.com/qqwweee/keras-yolo3
  
  https://github.com/Qidian213/deep_sort_yolov3

# Quick Start

  1. Download YOLOv3 or tiny_yolov3 weights from [YOLO website](http://pjreddie.com/darknet/yolo/).Then convert the Darknet YOLO model to a Keras model. Or use what i had converted https://drive.google.com/file/d/1uvXFacPnrSMw6ldWTyLLjGLETlEsUvcE/view?usp=sharing (yolo.h5 model file with tf-1.4.0) , put it into model_data folder
  
  2. Run YOLO_DEEP_SORT with cmd :
   ```
   python my_demo.py <path/to/input_video> <path/to/output_video> <path/to/output_txt>
   ```
   (default input_video is webcam feed, default output_video is ./output.avi, default output_txt is ./detection.txt)

# Dependencies

  The code is compatible with Python 2.7 and 3. The following dependencies are needed to run the tracker:

    NumPy
    sklean
    OpenCV

  Additionally, feature generation requires TensorFlow-1.4.0.

# Note 

  Model file model_data/mars-small128.pb need by deep_sort had convert to tensorflow-1.4.0
 
# Test only

  Speed : when only run yolo detection about 11-13 fps  , after add deep_sort about 11.5 fps (GTX1060 6G)
 
  Test input video : ./test_video.avi
  
  Test result video : ./test_output.avi
  
  Test output txt : ./test_detection.txt
 

