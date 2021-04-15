# YOLO-V5-Road-distress-imaging
this repository represents the usage of modern computervision **YOLO V5** in automatic detection of road distresses 
 **All code and models are under active development, and are subject to modification or deletion without notice.**
## Requirements
Python 3.8 or later along with `torch>=1.7` and the requirements given in [requirements.txt](https://github.com/RajaFida/YOLO-V5-Road-distress-imaging/blob/main/requirements.txt)  To install run:
```bash
$ conda install -c conda-forge pycocotools
$ pip install -r requirements.txt
```

## Inference for Potholes
To run inference on example images in `data/images`:
```bash
$ python detect.py --source data/images --weights best_potholes.pt --conf 0.5 --img 416
```
## Inference for Cracks
To run inference on example images in `data/images`:
```bash
$ python detect.py --source data/images --weights last_cracks.pt --conf 0.5 --img 416
```


### Results when running

```bash
/content/YOLO-V5-Road-distress-imaging
Namespace(agnostic_nms=False, augment=False, classes=None, conf_thres=0.5, device='', exist_ok=False, img_size=640, iou_thres=0.45, name='exp', project='runs/detect', save_conf=False, save_txt=False, source='data/images', update=False, view_img=False, weights=['last_cracks.pt'])
YOLOv5 🚀 b8e0280 torch 1.8.1+cu101 CPU

Fusing layers... 
Model Summary: 232 layers, 7246518 parameters, 0 gradients, 16.8 GFLOPS
image 1/16 /content/YOLO-V5-Road-distress-imaging/data/images/2891--142-_jpg.rf.9fe7d5ba0407d4789dc84f6f9129b232.jpg: 640x640 6 0s, Done. (0.455s)
image 2/16 /content/YOLO-V5-Road-distress-imaging/data/images/2893--8-_jpg.rf.f054793b0be95746ed1272235b3795d9.jpg: 640x640 1 0, Done. (0.444s)
image 3/16 /content/YOLO-V5-Road-distress-imaging/data/images/2897--116-_jpg.rf.6685af4d47a45d1b22a7f3262e0dd69e.jpg: 640x640 8 0s, Done. (0.427s)
image 4/16 /content/YOLO-V5-Road-distress-imaging/data/images/2897--156-_jpg.rf.c2bb966aa10f1fd6bf0348b49f7482b7.jpg: 640x640 18 0s, Done. (0.423s)
image 5/16 /content/YOLO-V5-Road-distress-imaging/data/images/2897--161-_jpg.rf.1e657b275b587bd0b945148abbf293d2.jpg: 640x640 7 0s, Done. (0.434s)
image 6/16 /content/YOLO-V5-Road-distress-imaging/data/images/2897--198-_jpg.rf.8c0ddc531d83d21dd2e97f5982ee33d7.jpg: 640x640 2 0s, Done. (0.431s)
image 7/16 /content/YOLO-V5-Road-distress-imaging/data/images/2897--228-_jpg.rf.13501ea2dafac6813a5edcfa0d8f7d25.jpg: 640x640 1 0, Done. (0.431s)
image 8/16 /content/YOLO-V5-Road-distress-imaging/data/images/2897--245-_jpg.rf.3d35d24738adfb6235acbe6b5fe7af07.jpg: 640x640 Done. (0.423s)
image 9/16 /content/YOLO-V5-Road-distress-imaging/data/images/2897--283-_jpg.rf.740b09e87e932671df487679ec18855b.jpg: 640x640 3 0s, Done. (0.431s)
image 10/16 /content/YOLO-V5-Road-distress-imaging/data/images/2897--294-_jpg.rf.de3da74e312a5b01bcfc89e5aaebb5a1.jpg: 640x640 6 0s, Done. (0.418s)
image 11/16 /content/YOLO-V5-Road-distress-imaging/data/images/2897--310-_jpg.rf.ee5f109e825244f9d1eb1220530de407.jpg: 640x640 9 0s, Done. (0.424s)
image 12/16 /content/YOLO-V5-Road-distress-imaging/data/images/2897--319-_jpg.rf.edbfd6d45ec4495c98f1d174d6c932f1.jpg: 640x640 Done. (0.438s)
image 13/16 /content/YOLO-V5-Road-distress-imaging/data/images/2897--339-_jpg.rf.2a55ee2a09496c777804ff33e41770b7.jpg: 640x640 3 0s, Done. (0.446s)
image 14/16 /content/YOLO-V5-Road-distress-imaging/data/images/2897--342-_jpg.rf.22fc0ba1b9144e58216967937887f226.jpg: 640x640 1 0, Done. (0.446s)
image 15/16 /content/YOLO-V5-Road-distress-imaging/data/images/2897--347-_jpg.rf.4b007991afa6ff07d09191fb73eb5397.jpg: 640x640 4 0s, Done. (0.426s)
image 16/16 /content/YOLO-V5-Road-distress-imaging/data/images/2897--94-_jpg.rf.5e5be35bd1b44b7743bf342e03829016.jpg: 640x640 12 0s, Done. (0.428s)
Results saved to runs/detect/exp2
Done. (7.128s)
```
