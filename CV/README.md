# Computer Vision Folder Notes

This folder contains my computer vision practice work across image classification, object detection, OCR, and segmentation.

## Folder Structure

```text
CV/
|- README.md
|- image_classification/
|  |- satellite-img-cls.ipynb
|  \- models/
|     |- resnet50_eurosat_best(3).pth
|     |- vit_eurosat_best.pth
|     \- vit_partial_best.pth
|- object_detection/
|  |- chess.ipynb
|  \- chess_pieces/
|     |- chess_yolo11/
|     |  |- args.yaml
|     |  |- results.csv
|     |  |- results.png
|     |  |- labels.jpg
|     |  |- train_batch*.jpg
|     |  |- val_batch*_pred.jpg
|     |  |- val_batch*_labels.jpg
|     |  \- weights/
|     |     |- best.pt
|     |     \- last.pt
|     |- chess_yolo112/
|     |  |- args.yaml
|     |  |- results.csv
|     |  |- results.png
|     |  |- labels.jpg
|     |  |- train_batch*.jpg
|     |  |- val_batch*_pred.jpg
|     |  |- val_batch*_labels.jpg
|     |  \- weights/
|     |     |- best.pt
|     |     \- last.pt
|     |- val/
|     |- val2/
|     |- val3/
|     |- val4/
|     |- val5/
|     \- val6/
|  \- building_detect/
|     |- building-defect (1).ipynb
|     \- runs/
|        \- detect/
|           |- train/
|           |  |- args.yaml
|           |  |- results.csv
|           |  |- results.png
|           |  |- labels.jpg
|           |  |- train_batch*.jpg
|           |  |- val_batch*_pred.jpg
|           |  |- val_batch*_labels.jpg
|           |  \- weights/
|           |     |- best.pt
|           |     \- last.pt
|           \- val/
|              |- Box*.png
|              |- confusion_matrix*.png
|              |- val_batch*_pred.jpg
|              \- val_batch*_labels.jpg
|- OCR/
|  |- handwriting/
|  |  |- exp.ipynb
|  |  |- test.jpeg
|  |  |- testt.jpeg
|  |  |- Grayscale_Image.jpeg
|  |  |- binary_image.jpeg
|  |  |- Inverted_Image.jpeg
|  |  |- noise_removed_image.jpeg
|  |  |- no_noise.jpeg
|  |  |- no_borders.jpeg
|  |  |- thickened.jpeg
|  |  |- thinned.jpeg
|  |  \- corrected_output.jpg
|  \- neutrition_labels/
|     |- ocr-labels.ipynb
|     |- detect/
|     |  \- val/
|     |     |- Box*.png
|     |     |- confusion_matrix*.png
|     |     |- val_batch*_pred.jpg
|     |     \- val_batch*_labels.jpg
|     \- label_detection/
|        |- args.yaml
|        |- results.csv
|        |- results.png
|        |- labels.jpg
|        |- train_batch*.jpg
|        |- val_batch*_pred.jpg
|        |- val_batch*_labels.jpg
|        \- weights/
|           |- best.pt
|           \- last.pt
\- segmentation/
   |- car_parts/
   |  |- car_parts (1).ipynb
   |  \- segment/
   |     |- carparts_seg_run/
   |     |  |- args.yaml
   |     |  |- results.csv
   |     |  |- results.png
   |     |  |- labels.jpg
   |     |  |- train_batch*.jpg
   |     |  |- val_batch*_pred.jpg
   |     |  |- val_batch*_labels.jpg
   |     |  \- weights/
   |     |     |- best.pt
   |     |     \- last.pt
   |     \- val/
   |        |- Box*.png
   |        |- Mask*.png
   |        |- confusion_matrix*.png
   |        |- val_batch*_pred.jpg
   |        \- val_batch*_labels.jpg
   \- ocean_trash/
      |- Underwater_trash_segmentation (4).ipynb
      |- download.jpeg
      |- download1.jpeg
      |- download2.jpeg
      |- download (7).jpeg
      |- images (7).jpeg
      |- images (8).jpeg
      \- YOLO_V8_N/
         |- trashcan_nano/
         |  |- args.yaml
         |  |- results.csv
         |  |- results.png
         |  |- labels.jpg
         |  |- train_batch*.jpg
         |  |- val_batch*_pred.jpg
         |  |- val_batch*_labels.jpg
         |  \- weights/
         |     |- best.pt
         |     \- last.pt
         |- val/
         |  |- Box*.png
         |  |- Mask*.png
         |  |- confusion_matrix*.png
         |  |- val_batch*_pred.jpg
         |  \- val_batch*_labels.jpg
         \- predictions_nano/
            \- vid_*_frame*.jpg
```

## What Each Folder Contains

- `image_classification`: Satellite image classification notebook and saved model checkpoints.
- `object_detection`: Chess piece and building-defect detection work with notebooks, YOLO training runs, validation outputs, metrics, and weight files.
- `OCR`: Handwriting preprocessing experiments and nutrition label detection/OCR outputs.
- `segmentation`: Car-part and ocean-trash segmentation notebooks, training outputs, prediction images, and checkpoints.

## Git Note

Model folders and checkpoint files such as `models/`, `weights/`, `.pth`, and `.pt` are now ignored through the root `.gitignore`, so they will not be pushed with the repository.
