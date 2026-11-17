# Pretrained Models for Grain Size Measurements

Model weights for [AI4GSD](https://github.com/pnnl/AI4GSD) and [YOLOv5-GSD](https://github.com/fluids/yolov5-GSD), stored using Git LFS.

## Models

| Model path | Purpose |
|---|---|
| `AI4GSD/anthroai.179.26.51.640.yolo11m.20250906.pt` | Non-sediment detection |
| `AI4GSD/capai.80.11.26.1280.yolo11m.20250825.pt` | Pixel-size estimation |
| `AI4GSD/rockai.47.7.0.1280.yolo11m.20250322.pt` | Sediment grain detection |
| `YOLOv5-GSD/yolo_v5_best.pt` | YOLOv5 grain detection |

## Download All Models

Install [Git LFS](https://git-lfs.com/), then run in a terminal:

```bash
git lfs install
git clone https://github.com/fluids/models.git
```

## Download a Specific Model with Python

Choose a model path from the table. The file will be saved in your current folder.

```python
from urllib.request import urlretrieve
model = "YOLOv5-GSD/yolo_v5_best.pt"
url = f"https://media.githubusercontent.com/media/fluids/models/main/{model}"
urlretrieve(url, model.split("/")[-1])
```

## Usage and Attribution

See each model’s source project for usage instructions, citations, and license terms.