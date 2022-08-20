# Emotion_recognition
# Emotion classification using deep learning and EEG signals

Cross-wavelet spectrum images are used as dataset for emotion classification using SEED-1 dataset of EEG signals.
Matlab’s cross wavelet and wavelet coherence toolbox was used to generate cross-wavelet spectrum images.
For classification of cross-wavelet spectrum images, VGG19 pretrained model was used along with additional Flatten, Dense, Dropout and Batch-Normalization layers. Hence, this is a Convolutional Neural Networks based project.

## Method - 1
Cross-wavelet spectrum of the original signal and it’s denoised version. The denoising was performed using wavelet denoising in Matlab. For this purpose, wden function of Matlab was used.  A total of 12741 images were generated out of 13950 images. 
 After 80-20 split, the dataset consisted of -
•	Training set – 10192 images
•	Test set – 2549 images
#### Classes - 3 : (Positive, Negative and Neutral)


## Method - 2
Cross-wavelet spectrum of the positive signal and negative signals with neutral EEG signal. A total of 6200 images were generated out of 13950 images. After 80-20 split, the dataset consisted of -
•	Training set – 4960 images
•	Test set – 1240 images
#### Classes - 2 : (Positive with neutral and Negative with neutral)

 The EEG signal of subject-1, Video-2 (Neutral signal- label-0), channel-1 was taken as the reference for generating positive with neutral and negative with neutral cross-wavelet spectrum images. 



SEED Dataset link - https://bcmi.sjtu.edu.cn/home/seed/
