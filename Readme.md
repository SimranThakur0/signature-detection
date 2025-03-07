# Signature Detection using YOLOv8 

## Overview
This project trains a YOLOv8 model to detect signatures in images. The dataset was annotated in the YOLO format, and data augmentation was performed to improve accuracy. The trained model is evaluated on test data and deployed using Flask for local inference.

## Project Structure
```
.
├── annotateddata/
│   ├── train/
│   │   ├── images/
│   │   ├── labels/
│   ├── valid/
│   │   ├── images/
│   │   ├── labels/
│   ├── test/
│   │   ├── images/
│   │   ├── labels/
├── data/
├── model/
├── notebooks/
│   ├── train.ipynb
├── app.py
├── requirements.txt
├── setup.sh
├── Readme.md
```

## Installation
1. Clone the repository:
   ```bash
   git clone <repo_link>
   cd <repo_folder>
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the setup script (optional):
   ```bash
   chmod +x setup.sh
   ./setup.sh
   ```

## Training the Model
- Open `notebooks/train.ipynb` and run the training script.
- The dataset is already structured in YOLO format.
- Augmentations were applied to improve model generalization.

## Evaluation
Once training is complete, the model is evaluated on the test dataset.

### Evaluation Result:
![Evaluation Screenshot](screenshot/1.jpeg)

## Notes
- The dataset contains a limited number of images, so augmentation was crucial.
