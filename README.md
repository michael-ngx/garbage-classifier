# Garbage Detector & Classifier

Project for APS360 - Applied Fundamentals of Deep Learning, University of Toronto

<u>Note</u>: this repository is shared only for skill display purposes. Copying others work and any other means of plagiarizing are serious offenses at the University of Toronto. Viewing the source code while taking the course is also considered an academic offense. We are not responsible for any such actions committed by students.

[Final Report](https://github.com/michael-ngx/garbage-classifier/blob/main/Final_Report.pdf)

[Final Video Presentation](https://www.youtube.com/watch?v=_FdqrLXcjMc&ab_channel=ChristopherShih)

### Overview

We fine-tuned 2 pre-trained models for our application: YOLOv8 (for object detection), and ResNet152 (for object classification). We also explored multiple designs for each task, detailed in `Classifier` and `Detector` sub-folders.

### Data source

Trash Annotation in Context (TACO) for YOLOv8. Kaggle 12-class & 6-class garbage dataset for ResNet152.

Additional pre-processing works (data cleaning & augmentation) were also done to ensure clean dataset and equal number of samples per class. 

### Results

- Detector: 0.66 Training Loss. 0.97 Validation Loss (loss = distance between predicted vs actual bounding box of object)
- Classifier: 97% Training accuracy. 94% Validation accuracy
