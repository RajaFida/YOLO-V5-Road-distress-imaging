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
$ python detect.py --source data/images --weights best_potholes.pt --img 416 --conf 0.5

Namespace(agnostic_nms=False, augment=False, classes=None, conf_thres=0.5, device='', exist_ok=False, img_size=640, iou_thres=0.45, name='exp', project='runs/detect', save_conf=False, save_txt=False, source='data/images', update=False, view_img=False, weights=['best_potholes.pt'])
YOLOv5 🚀 423b3eb torch 1.8.1+cu101 CPU

Fusing layers... 
Model Summary: 232 layers, 7246518 parameters, 0 gradients, 16.8 GFLOPS
image 1/2 /content/YOLO-V5-Road-distress-imaging/data/images/2897--319-_jpg.rf.edbfd6d45ec4495c98f1d174d6c932f1.jpg: 640x640 3 0s, Done. (0.801s)
image 2/2 /content/YOLO-V5-Road-distress-imaging/data/images/2897--339-_jpg.rf.2a55ee2a09496c777804ff33e41770b7.jpg: 640x640 4 0s, Done. (0.675s)
Results saved to runs/detect/exp
Done. (1.653s)
```
