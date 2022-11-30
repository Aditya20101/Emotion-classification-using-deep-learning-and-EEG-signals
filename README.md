# Emotion_recognition
# Emotion classification using deep learning and EEG signals

Cross-wavelet spectrum images are used as dataset for emotion classification using SEED-1 dataset of EEG signals.
Matlab’s cross wavelet and wavelet coherence toolbox was used to generate cross-wavelet spectrum images.
For classification of cross-wavelet spectrum images, VGG19, VGG16 and RESNET50 pretrained models were used along with additional Flatten, Dense, Dropout and Batch-Normalization layers. Hence, this is a Convolutional Neural Networks based project. The study was done for two cases-(i) One additional dense layer; (ii) Two addtional dense layers on the pretrained models.

## Method - 1
Cross-wavelet spectrum of the original signal and it’s denoised version. The denoising was performed using wavelet denoising in Matlab. For this purpose, wden function of Matlab was used.  A total of 12741 images were generated out of 13950 images. 
 After 80-20 split, the dataset consisted of -
•	Training set – 10192 images
•	Test set – 2549 images

#### Classes - 3 : (Positive, Negative and Neutral)

Method - 1 : Dataset sample

<img width="536" alt="image" src="https://user-images.githubusercontent.com/75621797/185759736-520a8e6d-d918-44b5-9f30-22460571e3e3.png">

 ### Method -1 results
 
 <img width="450" alt="image" src="https://user-images.githubusercontent.com/75621797/204766254-13675229-cf6f-4b6f-97d9-d86adda93110.png">




## Method - 2
Cross-wavelet spectrum of the positive signal and negative signals with neutral EEG signal. A total of 6200 images were generated out of 13950 images. After 80-20 split, the dataset consisted of -
•	Training set – 4960 images
•	Test set – 1240 images
#### Classes - 2 : (Positive with neutral and Negative with neutral)

Method - 2 : Dataset sample

<img width="514" alt="image" src="https://user-images.githubusercontent.com/75621797/185759757-6810fc94-9bf5-48db-ad61-c8e8224881e8.png">

 ### Method -2 results

<img width="450" alt="image" src="https://user-images.githubusercontent.com/75621797/204766376-c73fd242-589d-4422-8927-399760908ef5.png">


 The EEG signal of subject-1, Video-2 (Neutral signal- label-0), channel-1 was taken as the reference for generating positive with neutral and negative with neutral cross-wavelet spectrum images. 






SEED Dataset link - https://bcmi.sjtu.edu.cn/home/seed/
