# Video-Reverser-Application-Using-Python-Flask
Overview
The Reverse Video App allows users to upload a video, which is then processed to create a reversed version of the video. The application utilizes a Flask backend with Python for video processing, and a responsive frontend built with HTML, CSS, and JavaScript.

Technologies Used

Frontend:
HTML
CSS
JavaScript

Backend:
Flask (Python)
Video Processing:
OpenCV for video frame manipulation
MoviePy for audio handling and video writing
Other Libraries:
NumPy for numerical operations

Video Processing:

Upon submission, the video file is sent to the backend where it is temporarily saved.
The reverse_video function is invoked, which performs the following:
Extracts audio from the uploaded video (if present).
Reads and reverses the video frames using OpenCV.
Reverses the extracted audio using the scipy.io.wavfile library, if applicable.
Combines the reversed video and audio using MoviePy and saves the final output.

Result Display:
The reversed video is then sent back to the frontend, where it is displayed in a video player for the user to watch.
