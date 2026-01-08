# YOLOv8 Electric Meter Number Detection

## 📦 Installation

### 1. Create Virtual Environment
```bash
python -m venv venv
```

### 2. Use Virtual Environment
```bash
.\venv\Scripts\activate
```

### 3. Install Dependencies
```bash
pip install -r requirements.txt
```

### 4. Training Model
```bash
python train_yolo.py
```

## Results: Step-by-Step Output
![Input Image](/images/00.jpg)

| Step | Description                                  | Image               |
| ---- | -------------------------------------------- | ------------------- |
| 1    | Convert image to grayscale                   | ![](/images/01.jpg) |
| 2    | Enhance contrast using CLAHE                 | ![](/images/02.jpg) |
| 3    | Apply Otsu's thresholding                    | ![](/images/03.jpg) |
| 4    | Use morphological open to remove small noise | ![](/images/04.jpg) |
| 5    | Filter contours by size and create mask      | ![](/images/05.jpg) |
| 6    | Apply mask to keep only valid digits         | ![](/images/06.jpg) |
| 7    | Invert colors (black digits on white bg)     | ![](/images/07.jpg) |
| 8    | Resize image to enlarge digits               | ![](/images/08.jpg) |
| 9    | Sharpen image to enhance edge clarity        | ![](/images/09.jpg) |

## Example
![Example](/images/20250617_02_01.png)
![Example](/images/20250617_02_02.png)
![Example](/images/20250617_02_03.png)
![Example](/images/20250617_02_04.png)
![Example](/images/20250617_02_05.png)
![Example](/images/20250617_02_06.png)
![Example](/images/20250617_02_07.png)
![Example](/images/20250617_02_08.png)
![Example](/images/20250617_02_09.png)
![Example](/images/20250617_02_10.png)