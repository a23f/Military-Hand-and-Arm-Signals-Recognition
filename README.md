# Military Hand and Arm Signals Recognition System
- This Military hand and arm signals recognition system is made using `Roboflow`, `YoloV5`, and `PyTorch`. This system can be run on an Nvidia Jetson Nano or even your own personal computer. 
- For Nvidia Jetson Nano users, please refer to [Setting-Up-Jetson-Nano](https://github.com/a23f/Setting-Up-Jetson-Nano/) repository on how to set up the Jetson Nano before doing Inference for this system.
- For personal computer users, please refer to

## Classes in the model
There are a total of 10 classes in the model.
1. Freeze
[cell_leader_i](https://user-images.githubusercontent.com/101104505/184507877-b746936a-537d-442d-b020-6b2c0f4801be.jpg)

## Running Inference on Nvidia Jetson Nano using Webcam
1. Click this link to download the model file: [MilitarySignals.pt](https://github.com/a23f/Military-Hand-and-Arm-Signals-Recognition/raw/main/MilitarySignals.pt)
2. Move the model to the YoloV5 folder on the Jetson Nano
3. Open Terminal
4. Run the inference inside your conda environment using the following codes. (change 'myenv' to your environment name)
   - `conda activate myenv`
   - `cd yolov5`
   - `python3 detect.py --weights MilitarySignals.pt --source 0 --device 0`

## Running Inference on personal computer using Webcam
1. Click this link to download the model file: [MilitarySignals.pt](https://github.com/a23f/Military-Hand-and-Arm-Signals-Recognition/raw/main/MilitarySignals.pt)
2. Move the model to the YoloV5 folder on the personal computer
3. Open Anaconda Prompt
4. Run the inference inside your conda environment using the following codes. (change 'myenv' to your environment name)
   - `conda activate myenv`
   - `cd yolov5`
   - `python detect.py --weights MilitarySignals.pt --source 0 --device 0`
