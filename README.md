## For Windows Installation 
* Download and Install cpp build tools https://visualstudio.microsoft.com/visual-cpp-build-tools/
* run buildtools exe file 
* Select Desktop Development With C++
* Check Mark MSVC and Windows 10 SDK Only
* And install it
```
pip install pycocotools
```

## Install Git 
* Download and Install Git <a href="https://git-scm.com/downloads"> Click Here</a>

## Clone Yolor
```
git clone https://github.com/Mubeen-Ahmad/yolor
cd yolor
```
## Install Requirments

```
pip install -r requirments.txt
```
## For Gpu 
Make Sure 

* NVIDIA Drivers (Updated to Latest)
* CUDA Toolkit 11.1

## Download Pretrained Weight

Download File and paste in the yolor Folder
<a href = "https://drive.google.com/file/d/1Tdn3yqpZ79X7R1Ql0zNlNScB1Dv9Fp76/view">Download</a>

## Execution

## On Images
```
python detect.py --source inference/images/horses.jpg --cfg cfg/yolor_p6.cfg --weights yolor_p6.pt --conf 0.25 --img-size 1280 --device 0

```
# Parameters
## --source Path (Images / Videos / Camera)
* e.g 
```
python detect.py --source inference/images/horses.jpg --cfg cfg/yolor_p6.cfg --weights yolor_p6.pt --conf 0.25 --img-size 1280 --device 0
```
```
python detect.py --source inference/myvideos.mp4 --cfg cfg/yolor_p6.cfg --weights yolor_p6.pt --conf 0.25 --img-size 1280 --device 0
```
* Here 0 is a Camera ID
```
python detect.py --source 0 --cfg cfg/yolor_p6.cfg --weights yolor_p6.pt --conf 0.25 --img-size 1280 --device 0

```
## --device Device ( GPU / CPU )
* e.g
* For GPU
 ```
 python detect.py --source 0 --cfg cfg/yolor_p6.cfg --weights yolor_p6.pt --conf 0.25 --img-size 1280 --device 0
 ```
* For CPU
 ```
 python detect.py --source 0 --cfg cfg/yolor_p6.cfg --weights yolor_p6.pt --conf 0.25 --img-size 1280 --device cpu
```
