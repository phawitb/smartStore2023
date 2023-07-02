# smartStore2023

###### 1.conda create --name yolov8 python=3.9
2.pip install notebook
3.python -m ipykernel install --user --name=yolov8  

4.install pytorch GPU >> https://pytorch.org/get-started/locally/
	- check cuda version! and install >> nvidia-smi
	- check complete install >> import torch
				    torch.__version__
				    torch.cuda.is_available()

5.pip install ultralytics >> https://github.com/ultralytics/ultralytics

6.resize images raw >> resize_img_floder.ipynb

7.make label >> https://www.makesense.ai/
8.split data >> split_imgs.ipynb

9.train >> yolo task=detect mode=train model=yolov8m.pt data=custom.yaml epochs=3 imgsz=640 batch=2 workers=0
10.transfer weights >> yolo task=detect mode=train model=yolov8m.pt pretrained=best.pt data=custom.yaml epochs=3 imgsz=640 batch=2 workers=0

11.predict >> Predict_img_floder_vdo.ipynb
