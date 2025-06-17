# YOLOv8 Electric Meter Number Detection

## 📦 Installation

Install all required dependencies using:

```bash
pip install -r requirements.txt
```

Run training using:

```bash
python train_yolo.py
```


# Results: Step-by-Step Output
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
