# Face-Detection
This line sets the video source to the default webcam, which OpenCV can easily capture.

NOTE: You can also provide a filename here, and Python will read in the video file. However, you need to have ffmpeg installed for that since OpenCV itself cannot decode compressed video. Ffmpeg acts as the front end for OpenCV, and, ideally, it should be compiled directly into OpenCV. This is not easy to do, especially on Windows.
Here, we capture the video. The read() function reads one frame from the video source, which in this example is the webcam. This returns:

The actual video frame read (one frame on each loop)
A return code
The return code tells us if we have run out of frames, which will happen if we are reading from a file. This doesn’t matter when reading from the webcam, since we can record forever, so we will ignore it.
