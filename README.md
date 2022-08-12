# Face-detection-Cascade-Classifier




In this practice, we aim to utilize the cascade classifier with the Haar feature to detect human faces. The well-known cascade classifier was proposed by Paul Viola and Michael Jones in 2001 [2]. The first step for implementing a cascade classifier is to gather the training samples that can be separated into two parts, positive images (which contain the human face(s)) and negative images (the target scenes without human faces or unrelated photos). Next, extract the Haar feature from the sample images with the technique of integral image (for reduction of the computation) [2]. However, the number of original Haar features is relatively large. With the help of the AdaBoost algorithm [2], one can select the highly correlated features to establish a strong classifier for human face detection. Since parts of the region of images are unrelated to the human faces, the author adopted the cascade classifier to drop the unwanted image in the early stage. Finally, we can use the trained cascade classifier to detect the human faces in the webcam frame.



在本項練習中，參考[1]，我們利用opencv 內建的 face cascade classifier 來判斷由視訊攝影機讀入的照片中是否有人臉






![image](https://user-images.githubusercontent.com/108604868/183235094-ec1f852c-4316-45ce-8ca0-868ce5d7720c.png)





https://user-images.githubusercontent.com/108604868/184277815-4c95d218-2102-4358-82d7-00dfac2697d6.mp4





# Reference
[1] https://www.youtube.com/watch?v=LopYA64KmdE&ab_channel=ProgrammingKnowledge  
[2] Rapid Object Detection using a Boosted Cascade of Simple Features
