# face segmentation using dlib and opencv

This script is based on https://github.com/matthewearl/faceswap

This script detects and segments faces in the input image. 

### 1. install dlib and opencv
To run the script you'll need to install dlib (http://dlib.net) including its
Python bindings, and OpenCV.

You can install dlib and opencv by:
```cmd
pip install dlib
pip install opencv-python
```

### 2. download dlib face landmarks model
You'll also need to obtain the trained model [from
dlib](http://dlib.net/files/shape_predictor_68_face_landmarks.dat.bz2).

Unzip with `bunzip2` and change `PREDICTOR_PATH` to refer to this file. 

On Linux, you can download and unzip by running this script: [./download.sh](./download.sh)

### 3. run the script
The script is run like so:

    ./faceseg.py <image> [<output image>]

If successful, a file `output.jpg` will be produced with only segmented face regions in the input image.
