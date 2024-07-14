# Tutorial for FTC OpenCV and VisionPortal

This is a tutorial for working with your camera, from the first steps of setting it up all the way up to recognizing game pieces and AprilTags.

# Setting up the camera
You can Learn how to learn how to connect your camera to the Control Hub and how to look at what it sees here:
- [Setting up Camera](https://ftc-tech-toolbox.vercel.app/docs/Computer%20Vision/a)

Guide for how to configure the camera and how to open the Camera Stream (don't use the sample OpMode):
- [Configuring an External Webcam](https://ftc-docs.firstinspires.org/en/latest/hardware_and_software_configuration/configuring/configuring_external_webcam/configuring-external-webcam.html)

Additionally, In the next page (which has its link right after this) you have an explanation of OpenCV's basics and 3 classes that I recommend to copy to your project so you can look at what your camera sees (make sure to copy them into 3 different classes):
- [Intro to OpenCV](https://ftc-tech-toolbox.vercel.app/docs/Computer%20Vision/b)

# Expanding on OpenCV (Optional)
If you want to learn more about how the computer vision works and want to expand your knowledge about it you can read about OpenCV on the official FTC OpenCV github project: 
- [FTC OpenCV Github](https://github.com/OpenFTC/EasyOpenCV)

# VisionPortal
Vision Portal is an expansion of OpenCV that makes the work with so much more comfortable and fun to look at with a lot of new features that are easy to work with.
Luckily for us, our good friend Tech Toolbox has us covered with a quick explanation of Vision Portal's addition s and some good sample classes for the basics of VisionPortal: 
- [Intro to VisionPortal](https://ftc-tech-toolbox.vercel.app/docs/Computer%20Vision/ea)

- [VisionProcessor](https://ftc-tech-toolbox.vercel.app/docs/Computer%20Vision/eb)

- [VisionProcessor OpMode](https://ftc-tech-toolbox.vercel.app/docs/Computer%20Vision/ec)

# VisionPortal Thresholding
In this section we are going to look at a great usage of VisionPortal's functions in a code that could be in a team's project for doing the computer vision in the Autonomous period:
- [VisionPortal Thresholding](https://ftc-tech-toolbox.vercel.app/docs/Computer%20Vision/ed)

The general idea is to look at the 3 places that the prop could be in (in this code they look in the left and center, and if the prop is in neither of them it must be in the right) for the color red, and the place that has a higher red amount than a threshold that we placed would be where the red prop is located. For further explanations about the code you can more about it in its page.
### How to try the code for yourselves
if you'd like to try the code for yourselves you need to make a few changes after copying the code to your project:
- Use the OpMode from the bottom of the previous page (it's the only one to include every part of the OpMode's code)
- Change the rectangle's coordinates to be for your use (the first point is the top left and the second is the bottom right of your rectangle).
If you want an easy way to see the rectangle (the 'rect' object is not visable in the camera stream), you can use the function 'Imgproc.rectangle()' to see the rectangles in your camera stream and thus make it easier to change them.
- (Optional) You can make the output of the code an enum instead of a string if you want am easy usage of the output, especially if you are going to use it in other classes for the autonomus or other usages.
# AprilTags
AprilTags are images that are similar to QR codes that are scattered across the field and could be very helpful for some tasks such as automatic straightening and letting the robot know exactly where it is in the field when in the auto period.
There is a lot of resources about AprilTags here and in the sample codes of the SDK (in the FtcRobotController): 
- [AprilTag Programming](https://ftc-docs.firstinspires.org/en/latest/programming_resources/index.html#apriltag-programming)
