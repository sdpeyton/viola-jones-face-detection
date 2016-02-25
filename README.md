# viola-jones-face-detection

Authors: Chee Yi Ong, Stephen Peyton

This folder contains two subfolders: trainHaar and detectFaces. trainHaar consists of the 
training algorithm which trains classifiers using Haar-like features, while detectFaces 
uses the trained classifiers to detect faces.

The main functions for both parts of the face detection routine are named identically to
 the folder containing the code, i.e., trainHaar.m for the training part, and detectFaces.m 
 for the detection part.
 
 Instructions:
 1. Training: simply start the training by running the script trainHaar ('trainhaar' in 
 command window). Note that this takes approximately 21 hours on a 2.6GHz quad-core i7.
 2. Detection: detectFaces('image.jpg') or detectFaces('someDirectory/image.jpg').
 
 Assumptions for detection:
 1. Frontal-facing images ONLY.
 2. Background is not cluttered. Solid-colored background works the best.
 3. Tilting of the head is at a minimum.
 4. Image size is approximately 300x400 or similar. Individual features are a minimum of 
  19x19, because that is the smallest size of a single Haar feature or classifier.
