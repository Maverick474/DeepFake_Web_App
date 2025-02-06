# Abstract

Deepfakes are synthetic media created using deep learning techniques, such as Generative Adversarial Networks (GANs), to produce realistic but fake images, videos, or audio. While they have legitimate uses in entertainment and education, they also pose risks like misinformation and fraud. Your project, Deepfake Detection Using various deep learning methods, aims to combat this by analyzing multiple data modalities (e.g., visual, audio) to identify inconsistencies and detect deepfakes more accurately. Our method is capable of automatically detecting the replacement and reenactment deep fakes. Our system uses a Res-Next Convolution neural network to extract the frame- level features and these features and further used to train the Long-Short-Term Memory (LSTM) based Recurrent Neural Network (RNN) to classify whether the video is subject to any kind of manipulation or not, i.e. whether the video is deep fake or real video. To emulate the real time scenarios and make the model perform better on real time data and particle swarm optimization (PSO) to boost the accuracy level through hyper parameters, we evaluate our method on large amount of balanced and mixed data-set prepared by mixing the various available data-set like Face-Forensic++, Deepfake detection challenge, and Celeb-DF.

# How to Run

1. Open Terminal or Command prompt from the location where you want to set the project. Recommended is to download and install git bash for terminal
2. Now run the following command,
> git clone https://github.com/Maverick474/DeepFake_Web_App.git

It only works if Git installed in your system, else download zip file manually from GitHub and extract it into desired location.

3. Now run,

Creating Virtual evnironment is Optional but recommended (must use git bash for activation)
> python -m venv venv
> 
> source venv/Scripts/activate

Following command will install all project required libraries
> pip install -r requirements.txt

4. Create uploaded_videos in the root folder

5. Download the .pt model: https://drive.google.com/drive/folders/1Q3cbRO13lh3RGyZVCxnN_4jslEEBqHaW?usp=sharing

6. Create folder models in the root folder and place .pt model in it

7. Now run server,
> python manage.py runserver

5. Now local server is ready. Open any browser and visit http://127.0.0.1:8000/
