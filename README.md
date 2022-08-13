# Military Hand and Arm Signals Recognition System
- This Military hand and arm signals recognition system is made using `Roboflow`, `YoloV5`, and `PyTorch`. This system can be run on an Nvidia Jetson Nano or even your own personal computer. 
- For Nvidia Jetson Nano users, please refer to [Setting-Up-Jetson-Nano](https://github.com/a23f/Setting-Up-Jetson-Nano/) repository on how to set up the Jetson Nano before doing Inference for this system.
- For personal computer users, please refer to

## Running Inference on Nvidia Jetson Nano using YoloV5
1. Download the model (Military.pt) file from the repository
2. Move the model to the YoloV5 folder on the Jetson Nano
3. Open Terminal
4. Run the inference inside your conda environment using the following codes. (change 'myenv' to your environment name)
   - `conda activate myenv`
   - `cd yolov5`
   - `python3 detect.py --weights Military.pt --source 0 --device 0`

## Running Inference on personal computer using YoloV5
1. Download the model (Military.pt) file from the repository
2. Move the model to the YoloV5 folder on the personal computer
3. Open Anaconda Prompt
4. Run the inference inside your conda environment using the following codes. (change 'myenv' to your environment name)
   - `conda activate myenv`
   - `cd yolov5`
   - `python detect.py --weights Military.pt --source 0 --device 0`
