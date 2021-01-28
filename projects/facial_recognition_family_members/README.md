# Face-Recognition-Against-My-Photo-Library
The iCloud photos from iOS or Mac OS provided a comprehensive way to tag faces. All the faces in the photo library will be identified and tagged accordingly based on the earlier user defined tags.

I am a photography enthusiast and I have started to taking photos from year 2004. As of today, it's over 200k shots and I've kept 40k of them. There are many desktop applications can do the job of face recognition, but it's going to be super fun if I can build the solution end to end, using deep learning.

## Environment Setup.
1. This project relies heavily on scikit-learn, tensorflow and keras packages. Details of the setup can be referred to the "requirements.txt" file.
2. Nvidia GPU for tensorflow is needed, if not, need to install tensorflow package, instead of tensorflow-GPU.
3. Command to be executed with conda installed.
	`conda create -n new_env python=3.5 --file requirements.txt`
4. The full python notebook is available [here](facial_recognition_family_members.ipynb)