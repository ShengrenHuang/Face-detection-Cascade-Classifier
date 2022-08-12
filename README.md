# Face-detection-Cascade-Classifier




In this practice, we aim to utilize the cascade classifier with the Haar feature to detect human faces. The well-known cascade classifier was proposed by Paul Viola and Michael Jones in 2001 [1]. The first step for implementing a cascade classifier is to gather the training samples that can be separated into two parts, positive images (which contain the human face(s)) and negative images (the target scenes without human faces or unrelated photos). Next, extract the Haar feature from the sample images with the technique of integral image (for reduction of the computation) [1]. However, the number of original Haar features is relatively large. With the help of the AdaBoost algorithm [1], one can select the highly correlated features to establish a strong classifier for human face detection. Since parts of the region of images are unrelated to the human faces, the authors in [1] adopted the cascade classifier to drop the unwanted image in the early stage. Finally, we can use the trained cascade classifier to detect the human faces in the webcam frame. In this practice, by referring to [2], we employ the default cascade classifier provided by OpenCV to detect the human faces through the webcam frame. The result shows that football superstar Eden Hazard is caught correctly.





![image](https://user-images.githubusercontent.com/108604868/183235094-ec1f852c-4316-45ce-8ca0-868ce5d7720c.png)





https://user-images.githubusercontent.com/108604868/184277815-4c95d218-2102-4358-82d7-00dfac2697d6.mp4





# Reference
[1] Paul Viola and Michael Jones. Rapid Object Detection using a Boosted Cascade of Simple Features, 2001.  
[2] OpenCV Python Tutorial For Beginners 35 - Face Detection using Haar Cascade Classifiers:  
https://www.youtube.com/watch?v=LopYA64KmdE&ab_channel=ProgrammingKnowledge .
