This adds a new functionality to the code behind the [Switching Eds blog post](http://matthewearl.github.io/2015/07/28/switching-eds-with-python/).

While the post in the link shows the swapping of one face with another, this code makes you swap two faces.

To run the script you'll need to install dlib (http://dlib.net) including its
Python bindings, and OpenCV. You'll also need to obtain the trained model [from
sourceforge](http://sourceforge.net/projects/dclib/files/dlib/v18.10/shape_predictor_68_face_landmarks.dat.bz2).

Unzip with `bunzip2` and change `PREDICTOR_PATH` to refer to this file. The
script is run like so:

    ./faceswap.py <head image> <first face image> <second face image>

If successful, a file `output.jpg` will be produced with the facial features
from `<head image>` replaced with the facial features from `<face image>`.

