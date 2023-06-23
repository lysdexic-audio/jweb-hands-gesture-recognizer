# jweb-hands-gesture-recognizer

A self contained example demonstrating how to use MediaPipe Hand Gesture Recognizer with Max's `jweb` connected to either a live webcamera stream or using still images. 

This example does both handtracking and gesture recognition. If you only require handtracking try: [jweb-hands-landmarker](https://github.com/lysdexic-audio/jweb-hands-landmarker)

![Max example patcher](./jweb-hands-gesture-recognizer.gif)

## Features

The Gesture classification model bundle can recognize these common hand gestures:

```
0 - Unrecognized gesture, label: Unknown
1 - Closed fist, label: Closed_Fist
2 - Open palm, label: Open_Palm
3 - Pointing up, label: Pointing_Up
4 - Thumbs down, label: Thumb_Down
5 - Thumbs up, label: Thumb_Up
6 - Victory, label: Victory
7 - Love, label: ILoveYou
```

The hand landmark model bundle detects the keypoint localization of 21 hand-knuckle coordinates within the detected hand regions. The model was trained on approximately 30K real-world images, as well as several rendered synthetic hand models imposed over various backgrounds.

![Handlandmarks diagram](hand-landmarks.png)

## Resources

This example is inspired by [an example by Rob Ramirez](https://github.com/robtherich/jweb-mediapipe), which is in turn inspired by [MediaPipe in JavaScript](https://github.com/LintangWisesa/MediaPipe-in-JavaScript).
