# MRNet-Segmentation

This project performs right ventricular (RV) segmentation in cardiac MRI using deep learning.  
It is part of the assignment for the UCD course: *AI for Medical Image Analysis*.

## Project Structure

| File / Folder | Description |
|---------------|-------------|
| `MRNetSegmentation.ipynb` | Main notebook for training and evaluation |
| `MRNetSegmentation.html` | Exported HTML version of the notebook |
| `plots/` | Contains visualization outputs (e.g., training curves, predictions) |
| `best_model.pth` | Best model (at epoch 25) |

---
## Task Overview
Due to size limitations, the dataset is stored externally.  

You can download the preprocessed dataset from:

**[Google Drive Dataset Link (MnM2)] https://drive.google.com/file/d/1fSSdYF7Vi8G_5Zk6yblHKu8Dfsg2EGIM/view?usp=drive_link**
> Place the extracted folder as `./data/` under your working directory.

---
## Trained Model Weights

You can download the best-performing model checkpoint here: 

**[best_model.pth (Google Drive)] https://drive.google.com/file/d/1lcSzt5U_toRsZdSBQjkYZjARnyIO6LE7/view?usp=drive_link**
> After downloading, place the file in the root folder or set its path in the notebook.

---
## Interactive Version of Notebook

An interactive version of the final segmentation notebook is also available: [MRNetSegmentation.html](./MRNetSegmentation.html)

It contains visualizations of training progress, model predictions, and performance evaluation.

---
## Visualizations

All training and prediction visualizations are saved in the `plots/` folder.

### Training Metrics
- `loss_dice_curves.png`: Training loss and Dice score across epochs

### Prediction Examples
- `epoch_1_prediction.png` to `epoch_30_prediction.png`: Sample predictions at different epochs
- `test_prediction_1.png` to `test_prediction_10.png`: Final predictions on test images

### Explainability (Grad-CAM)
- `gradcam_epoch1.png` to `gradcam_epoch30.png`: Grad-CAM visualizations for each epoch
- These attention maps highlight which regions the model focused on for segmentation.

> These visualizations help monitor learning progress and evaluate both prediction quality and model explainability.

---
## How to Run

Launch the notebook
- jupyter notebook MRNetSegmentation.ipynb
- You can run the notebook cell-by-cell to train the model, visualize predictions, and evaluate performance.

