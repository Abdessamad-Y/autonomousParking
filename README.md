# Autonomous car parking while using AI agent from Unity

### the goal of this project is to stimulate real life autonomous parking with unity


## Installation
### 1) First clone the repository somewhere you like

### 2) Install Unity Hub
You can download Unity Hub from here: **[https://unity3d.com/get-unity/download](https://unity3d.com/get-unity/download)**
With Unity Hub you can easily manage Unity  installations and projects.

### 3) Install Unity
Load the Unity project and use the error message it gives regarding the version, to install the version of Unity the project was made in.
**![](https://lh5.googleusercontent.com/blqH-PccoH1khIPceOxbqgUS7LV2wxi8isphmjrslcVU76yY6FYkOOmTfYO4qwZoE9orvH5bxIdLIZ5INGW6p1DpA5BxnN5IBXfKdUwXZNUPJuRT8e3IlyMqCYaRMw)**
*The version in the picture is different from the actual project version*

### 4) Install the ML-Agents package in Unity
It could be that Unity already did this by looking at the manifest.json file. You can check this by going to *Window -> Package Manager*. Select *Packages: In Project* and ML-Agents 2.0.1 should be in there. If not, you can install this by selecting *Packages: Unity Registry* and searching for the ML-Agents package.



**![](https://lh3.googleusercontent.com/mSr30SKamTx5wViKCRiJB9w6lIcKu-JTIjOpUTYWQn_jMDHR_GeypubYaOQfNNhgHjBHQ7Bjf7LeI_MYtGfxfWRIaEcWIoP71blnO1ZoJZAvwdN_rGPoktHqJ6U9wg)**



### 5) Install Python with ML-Agents / PyTorch
I'll use Anaconda here.

    conda create -n <venv name> python=3.8
    conda activate <venv name>
    pip install mlagents

check the unity mlagents documentattion in this link :
**[https://github.com/Unity-Technologies/ml-agents](https://github.com/Unity-Technologies/ml-agents)**
(Highly recommended)

This can be different for your system depending on which platform you are, use the PyTorch website to create the install command for you. In my case (Windows/Nvidia) this was: 

    conda install pytorch torchvision torchaudio cudatoolkit=10.2 -c pytorch

Verify the installation by trying the command:

    mlagents-learn

you must see the unity logo if not reinstall

**![](https://lh4.googleusercontent.com/Su_6IuXyVYrsI1Tk-t7-yVqJy83CxQUsUUt-Md6_JwfHzz898GUUb8wb0V3_E4354Qbn5ay2FcsVcgHqsg2aEsKrL_Q8VsL3Cz1gNV2mtCBQc2agwAmAf--Exf7-Hg)**


## the rewards parameters can be found on the file CarAgent.cs (this is the hardest parameter to play with )

## for the hyperparameter and the model settings chack trainer_settings.yaml




The project was inspired from Thomas Van Iseghem 