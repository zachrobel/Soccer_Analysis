Soccer Video Analysis Program

Overview

This program is designed to analyze soccer videos by detecting and tracking players and the ball, assigning teams to players, and visualizing team ball control statistics. It utilizes computer vision techniques and machine learning algorithms to perform various tasks such as object detection, tracking, and clustering.

Features

Player and Ball Detection: The program uses the YOLOv5 object detection model to detect players, referees, and the ball in soccer video frames. It utilizes the Ultralytics library for seamless integration with the YOLOv5 model.

Object Tracking: A custom tracker class is implemented to track the detected players, referees, and the ball across video frames. The tracker utilizes the Supervision library for efficient object tracking.

Team Assignment: The program assigns teams to players based on the color similarity between player jerseys and dominant team colors identified using K-means clustering.

Visualization: The program visualizes team ball control statistics by overlaying semi-transparent rectangles on video frames, indicating which team has control of the ball at each frame.

Usage

Prepare your soccer video file (e.g., soccer.mp4) and place it in the project directory.

Run the main() function in the soccer_analysis.py file:

Copy code
python soccer_analysis.py
The program will process the video frames, perform object detection and tracking, assign teams to players, and visualize team ball control statistics.

The annotated video with visualizations will be saved as output.avi in the project directory.
