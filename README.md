# Computer Control with Real-Time Imaging
 A basic study aimed at improving the computer usage comfort of individuals with physical disabilities. Libraries used in Python: OpenCV, MediaPipe, PyAutoGUI, cvzone.

 The project focuses on controlling the mouse using facial and eye movements, specifically for right-left clicking operations. To prevent uncontrolled clicks, the user must be at a certain distance from the screen. The mouse cursor movement is achieved by tracking the left pupil. When the user reaches a fixed distance, the distance between the lower edge of the left eye and the left corner of the lips is calculated at the moment of left eye blinking. If this distance is sufficiently short, it is interpreted as a left mouse click. To account for the possibility of both eyes partially closing at different ratios during blinking, right eye blinking is measured by the distance between the lower edge of the right eye and the midpoint of the right cheek. If this distance is sufficiently short, it is interpreted as a right mouse click.

 
