# MRNet-Segmentation

This project performs multi-class cardiac MRI segmentation (Left Ventricle, Myocardium, Right Ventricle) using deep learning.  
It is part of the assignment for the UCD course: *AI for Medical Image Analysis*.

## Project Structure

| File / Folder | Description |
|---------------|-------------|
| `MRNetSegmentation_UNet.ipynb` | Main notebook for U-Net training, explainability (Grad-CAM), and evaluation |
| `MRNetSegmentation_UNet.pdf` | Exported PDF version of the notebook |
| `epoch_prediction/` | Sample predictions at different training epochs |
| `gradcam_epoch/` | Grad-CAM visualizations for each epoch and class |
| `test_prediction/` | Final predictions on unseen test images |
| `loss_dice_curves.png` | Training loss, Dice score, and IoU curves for U-Net |
| `training_curves.png` | Combined training metrics plot for U-Net |
| `README.md` | Project documentation |

---
## Task Overview
Due to size limitations, the dataset is stored externally.  

You can download the preprocessed dataset from:

**[Google Drive Dataset Link (MnM2)] https://drive.google.com/file/d/1fSSdYF7Vi8G_5Zk6yblHKu8Dfsg2EGIM/view?usp=sharing**
> Place the extracted folder as `./data/` under your working directory.

---
## Trained Model Weights

You can download the best-performing model checkpoint here: 

**[best_model.pth (Google Drive)] https://drive.google.com/file/d/15sgA1RibdAWwBy97q5d-QXSdMhyyyFsn/view?usp=sharing**
> After downloading, place the file in the root folder or set its path in the notebook.

---
## Interactive Version of Notebook

An interactive version of the final segmentation notebook is also available: [MRNetSegmentation_UNet.pdf](./MRNetSegmentation_UNet.pdf)

It contains visualizations of training progress, model predictions, and performance evaluation.

---

## Visualizations

All outputs are saved in the corresponding folders or as standalone image files.

### Training Metrics
- `loss_dice_curves.png` — Loss, Dice score, and IoU trends over epochs
- `training_curves.png` — Combined training metrics for U-Net

### Prediction Examples
- `epoch_prediction/` — Predictions at various training epochs
- `test_prediction/` — Final predictions on unseen test images

### Explainability (Grad-CAM)
- `gradcam_epoch/` — Grad-CAM visualizations for each epoch and target class  
  These highlight which regions the model focused on for each cardiac structure.

---
## How to Run

Launch the notebook
- jupyter notebook MRNetSegmentation.ipynb
- You can run the notebook cell-by-cell to train the model, visualize predictions, and evaluate performance.

