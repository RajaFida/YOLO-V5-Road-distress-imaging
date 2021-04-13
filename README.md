# YOLO-V5-Road-distress-imaging
this repository represents the usage of modern computervision **YOLO V5** in automatic detection of road distresses 
 **All code and models are under active development, and are subject to modification or deletion without notice.**
## Requirements
Python 3.8 or later along with `torch>=1.7` and the requirements given in [requirements.txt](https://github.com/RajaFida/YOLO-V5-Road-distress-imaging/blob/main/requirements.txt)  To install run:
```bash
$ pip install -r requirements.txt
```

## Inference
To run inference on example images in `data/images`:
```bash
$ python detect.py --source data/images --weights best_potholes.pt --conf 0.25

Namespace(agnostic_nms=False, augment=False, classes=None, conf_thres=0.25, device='', exist_ok=False, img_size=640, iou_thres=0.45, name='exp', project='runs/detect', save_conf=False, save_txt=False, source='data/images/', update=False, view_img=False, weights=['yolov5s.pt'])
YOLOv5 v4.0-96-g83dc1b4 torch 1.7.0+cu101 CUDA:0 (Tesla V100-SXM2-16GB, 16160.5MB)

Fusing layers... 
Model Summary: 224 layers, 7266973 parameters, 0 gradients, 17.0 GFLOPS
image 1/2 /content/yolov5/data/images/bus.jpg: 640x480 4 persons, 1 bus, Done. (0.010s)
image 2/2 /content/yolov5/data/images/zidane.jpg: 384x640 2 persons, 1 tie, Done. (0.011s)
Results saved to runs/detect/exp2
Done. (0.103s)
```
