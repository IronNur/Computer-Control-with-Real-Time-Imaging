# Computer Control with Real-Time Imaging
 A basic study aimed at improving the computer usage comfort of individuals with physical disabilities. Libraries used in Python: OpenCV, MediaPipe, PyAutoGUI, cvzone.

 The project focuses on controlling the mouse using facial and eye movements, specifically for right-left clicking operations. To prevent uncontrolled clicks, the user must be at a certain distance from the screen. The mouse cursor movement is achieved by tracking the left pupil. When the user reaches a fixed distance, the distance between the lower edge of the left eye and the left corner of the lips is calculated at the moment of left eye blinking. If this distance is sufficiently short, it is interpreted as a left mouse click. To account for the possibility of both eyes partially closing at different ratios during blinking, right eye blinking is measured by the distance between the lower edge of the right eye and the midpoint of the right cheek. If this distance is sufficiently short, it is interpreted as a right mouse click.

![](https://github.com/IronNur/Computer-Control-with-Real-Time-Imaging/blob/main/images%20(1).png)

Figure 1: Eye area

![](https://github.com/IronNur/Computer-Control-with-Real-Time-Imaging/blob/main/images%20(2).png)

Figure 2: Distance measurement

![](https://github.com/IronNur/Computer-Control-with-Real-Time-Imaging/blob/main/images%20(3).png)

Figure 3: Right eye control distance

![](https://github.com/IronNur/Computer-Control-with-Real-Time-Imaging/blob/main/images%20(4).png)

Figure 4: Right eye blinking distance measurement

![](https://github.com/IronNur/Computer-Control-with-Real-Time-Imaging/blob/main/images%20(5).png)

Figure 5: Left eye control distance

![](https://github.com/IronNur/Computer-Control-with-Real-Time-Imaging/blob/main/images%20(6).png)

Figure 6: Left eye blinking distance measurement

 To initiate clicks, the user is expected to be at a distance of 80-83 cm from the computer. When closer than 80 cm, a "MOVE BACK" warning is given with a red frame, and when farther than 83 cm, a "MOVE CLOSER" warning is given with a red frame. When the set optimum distance is reached, the user is notified with a green frame.

![](https://github.com/IronNur/Computer-Control-with-Real-Time-Imaging/blob/main/images%20(7).png)

Figure 7: Move back warning

![](https://github.com/IronNur/Computer-Control-with-Real-Time-Imaging/blob/main/images%20(9).png)

Figure 8: Move closer warning

![](https://github.com/IronNur/Computer-Control-with-Real-Time-Imaging/blob/main/images%20(8).png)

Figure 9: Optimum distance warning

 When the optimum distance is reached, during the right eye blink, the calculated distances are listed in fours and averaged. If the average is within a certain range, a right click is detected. The same calculation is done for the left eye, listed in threes, and detected accordingly.

![](https://github.com/IronNur/Computer-Control-with-Real-Time-Imaging/blob/main/images%20(10).png)

Figure 10: Right eye click count

![](https://github.com/IronNur/Computer-Control-with-Real-Time-Imaging/blob/main/images%20(11).png)

Figure 11: Left eye blink count
