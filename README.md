# Penalty Kick Analysis: Visual Recognition, Pose Estimation, and LSTM




The penalty kick is one of the most dramatic events that can occur in a soccer game. It can be the source of heartbreak or the source of glory for millions of fans. With an event that can be game defining, only around 17.5% of penalties are saved. Coaches have long made the hypothesis that the direction the kicker will shoot the penalty kick can be predicted based on their body movements prior to the shot. Here we test this hypothesis. Are we able to determine the direction of a penalty shot based on the kicker’s body movements before they make contact with the ball? This question is examined using three main concepts 1) object detection by means of YOLO v7, 2) pose estimation by means of YOLO Pose, and 3) categorical prediction through LSTM. By implementing this process on video data gathered from YouTube, we can extract pose data and track the kicker’s movements over a sequence of frames. This sequence of skeletal keypoint coordinates can then be input in the LSTM to train a model that predicts the final direction of the kick whether it is “Center”, “Left”, or “Right”. The predictions made by the model were then compared with a random generator intended to act as a goalkeeper randomly choosing a direction to dive. On average the random choosing goalkeeper had a predictive accuracy of 33.8% whereas the trained model had a predictive accuracy of 41.6%, displaying a 7.8% improvement in predictive accuracy.












