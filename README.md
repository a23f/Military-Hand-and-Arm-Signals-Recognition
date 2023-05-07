# Military Hand and Arm Signals Recognition System
- This Military hand and arm signals recognition system is made using `Roboflow`, `YoloV5`, and `PyTorch`. This system can be run on an Nvidia Jetson Nano or even your own personal computer. 
- For Nvidia Jetson Nano users, please refer to [Setting-Up-Jetson-Nano-For-YoloV5-Object-Detection](https://github.com/a23f/Setting-Up-Jetson-Nano-For-YoloV5-Object-Detection) repository on how to set up the Jetson Nano and the required packages installation before doing Inference for this system.
- For personal computer users, please refer to [Setting-Up-Windows-For-YOLOv5-Object-Detection](https://github.com/a23f/Setting-Up-Windows-For-YOLOv5-Object-Detection) repository on how to set up the Anaconda on Windows and the required packages installation before doing Inference for this system.

## Classes in the model
Dataset images were captured using a webcam and annotated using [Roboflow](https://roboflow.com/). There are a total of 10 classes in the model:
1. Freeze
2. Pistol
3. Trap
4. Cell Leader
5. Enemy
6. Gather
7. Gas
8. Hostage
9. Rifle
10. Sniper

<img src="https://github.com/a23f/Military-Hand-and-Arm-Signals-Recognition/blob/main/Classes/Freeze.jpg" width="250" height="305">    <img src="https://github.com/a23f/Military-Hand-and-Arm-Signals-Recognition/blob/main/Classes/Pistol.jpg" width="250" height="305">    <img src="https://github.com/a23f/Military-Hand-and-Arm-Signals-Recognition/blob/main/Classes/Trap.jpg" width="250" height="305">

<img src="https://github.com/a23f/Military-Hand-and-Arm-Signals-Recognition/blob/main/Classes/Cell_Leader.jpg" width="200" height="325">     <img src="https://github.com/a23f/Military-Hand-and-Arm-Signals-Recognition/blob/main/Classes/Enemy.jpg" width="200" height="325">     <img src="https://github.com/a23f/Military-Hand-and-Arm-Signals-Recognition/blob/main/Classes/Gather.jpg" width="200" height="325">    <img src="https://github.com/a23f/Military-Hand-and-Arm-Signals-Recognition/blob/main/Classes/Gas.jpg" width="200" height="325">

<img src="https://github.com/a23f/Military-Hand-and-Arm-Signals-Recognition/blob/main/Classes/Hostage.jpg" width="200" height="325">      <img src="https://github.com/a23f/Military-Hand-and-Arm-Signals-Recognition/blob/main/Classes/Rifle.jpg" width="200" height="325">     <img src="https://github.com/a23f/Military-Hand-and-Arm-Signals-Recognition/blob/main/Classes/Sniper.jpg" width="200" height="325">

## Running Inference on Nvidia Jetson Nano using:
### Webcam
1. Click this link to download the model file: [MilitarySignals.pt](https://github.com/a23f/Military-Hand-and-Arm-Signals-Recognition/raw/main/MilitarySignals.pt)
2. Move the model to the YoloV5 folder on the Jetson Nano
3. Open Terminal
4. Run the inference inside your conda environment using the following codes. (change 'myenv' to your environment name)
   - `conda activate myenv`
   - `cd yolov5`
   - `python3 detect.py --weights MilitarySignals.pt --source 0 --device 0`
5. Try imitating the 10 Military Hand and Arm Signal classes as shown above in front of your webcam.

### Image File
1. Click this link to download the model file: [MilitarySignals.pt](https://github.com/a23f/Military-Hand-and-Arm-Signals-Recognition/raw/main/MilitarySignals.pt)
2. Move the model to the YoloV5 folder on the Jetson Nano
3. Open Terminal
4. Run the inference inside your conda environment using the following codes. (change 'myenv' to your environment name)
   - `conda activate myenv`
   - `cd yolov5`
   - `python3 detect.py --weights MilitarySignals.pt --source 0 --device image.jpg`    (change 'image.jpg' to your image file name)

### Video File
1. Click this link to download the model file: [MilitarySignals.pt](https://github.com/a23f/Military-Hand-and-Arm-Signals-Recognition/raw/main/MilitarySignals.pt)
2. Move the model to the YoloV5 folder on the Jetson Nano
3. Open Terminal
4. Run the inference inside your conda environment using the following codes. (change 'myenv' to your environment name)
   - `conda activate myenv`
   - `cd yolov5`
   - `python3 detect.py --weights MilitarySignals.pt --source 0 --device video.mp4`    (change 'video.mp4' to your video file name)

## Running Inference on personal computer using:
### Webcam
1. Click this link to download the model file: [MilitarySignals.pt](https://github.com/a23f/Military-Hand-and-Arm-Signals-Recognition/raw/main/MilitarySignals.pt)
2. Move the model to the YoloV5 folder on the personal computer
3. Open Anaconda Prompt
4. Run the inference inside your conda environment using the following codes. (change 'myenv' to your environment name)
   - `conda activate myenv`
   - `cd yolov5`
   - `python detect.py --weights MilitarySignals.pt --source 0 --device 0`
5. Try imitating the 10 Military Hand and Arm Signal classes as shown above in front of your webcam.

### Image File
1. Click this link to download the model file: [MilitarySignals.pt](https://github.com/a23f/Military-Hand-and-Arm-Signals-Recognition/raw/main/MilitarySignals.pt)
2. Move the model to the YoloV5 folder on the personal computer
3. Open Anaconda Prompt
4. Run the inference inside your conda environment using the following codes. (change 'myenv' to your environment name)
   - `conda activate myenv`
   - `cd yolov5`
   - `python detect.py --weights MilitarySignals.pt --source 0 --device image.jpg`     (change 'image.jpg' to your image file name)

### Video File
1. Click this link to download the model file: [MilitarySignals.pt](https://github.com/a23f/Military-Hand-and-Arm-Signals-Recognition/raw/main/MilitarySignals.pt)
2. Move the model to the YoloV5 folder on the personal computer
3. Open Anaconda Prompt
4. Run the inference inside your conda environment using the following codes. (change 'myenv' to your environment name)
   - `conda activate myenv`
   - `cd yolov5`
   - `python detect.py --weights MilitarySignals.pt --source 0 --device video.mp4`     (change 'video.mp4' to your video file name)
