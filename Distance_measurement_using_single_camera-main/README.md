# Distance measurement using single:one:camera :camera:

If you want to estimate distance of objects with your simple webcam, then this algorithm(*Triangle similarity*) would be helpful for you to find Distance *from object to camera*, I have provide to two examples, one is simple **face detection and distance Estimation**, other is **Yolo4 object detection and distance Estimation**


## install Opencv-python

- Windows

  pip install opencv-python

- _install Opencv-python on Linux or Mac_

  pip3 install opencv-python

## Run the code

- windows: :point_down:

  python distance.py

  ------ OR ---------

  python Updated_distance.py

- linux or Mac :point_down:

  python3 distance.py

  ------ OR ---------

  python3 Updated_distance.py

### :bulb:_Focal Length Finder Function Description_ :bulb:

```python
# focal length finder function
def focal_length(measured_distance, real_width, width_in_rf_image):

    focal_length_value = (width_in_rf_image * measured_distance) / real_width
    #return focal length.
    return focal_length_value

```

The Focal Length finder Function has three Arguments:

`measured_distance` is the distance which we have measured while capturing the reference image:straight*ruler:. \*\*\_From object to Camera*\*\* which is `Known_distance = 72.2 #centimeter`

`real_width` It's measured as the width of the object in the real world, here I measured the width of the face in real-world which was `Known_width =14.3 # centimetre`

`width_in_rf_image` is the width of the object in the image/frame it will be in **pixels**

### :bulb:_Distance Finder Function Description_ :bulb:

```python
# Distance estimation function

def distance_finder(focal_length, real_face_width, face_width_in_frame):

    distance = (real_face_width * focal_length)/face_width_in_frame
    return distance

```

This Function takes three Arguments,

` Focal_Length` is the focal length, out of the **FocalLength** finder function.

`real_face_width` measures the width of an object in the real world, here I measured the width of a face in real-world which was `Known_width =14.3 #centimeter`

`face_width_in_frame` is the width of the face in the frame, the unit will be pixels here.



You can create the following Robot with Raspberry That would be easy then, using Arduino Stuff, Raspberry 🍓 Pi will make it a system on Robot 🤖