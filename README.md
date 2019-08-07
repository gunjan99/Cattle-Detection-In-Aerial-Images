# Cattle-Detection-In-Aerial-Images
This was my CSIR-CEERI project for the period of 2 months from May 20, 2019 to July 13, 2019. For this project I created dataset of my own using the videos obtained online(around 1500 images were annotated manually and trained upon). Since not much data was available so testing was done using random images picked from google images.For this project I used fizyr's implementation of retinanet. In this implementation I made two changes: 1) Added a new anchor size of 32 as aerial images are smaller in size 2) skip_mismatch parameter was set to true
This is the link to the dataset I created by extracting frames from videos and annotating them manually using labelImg tool.
https://drive.google.com/open?id=1Me12L7_ZLFKEOLd4_MbF6phipwYemmyK<br/>
The link to weights obtained after training Retinanet architecture for 50 epochs is : https://drive.google.com/open?id=1DTjKc6ZAQhJn1q6gX_mpzn9T1xXQ_PeP<br/>
Parameters for training were:<br/>
1)epochs:50<br/>
2)batch size = 1<br/>
3)steps in each epoch = 1300<br/>
Results are shown using images having the name starting with 'result' in this repo.<br/>
Images having name starting with 'EarlyResult' show the results obtained from the weights of ImageNet(which had a class 'Cow').
