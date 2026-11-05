# FP-CycleGAN + ResNet-18 Fault Diagnosis

Fault diagnosis on image data using a CycleGAN-style generator (FP-CycleGAN) and a ResNet-18 classifier.

## What's in the notebook
- Part 1: FP-CycleGAN trained for 15 epochs (Noload domain <-> faulty domain), then a ResNet-18 trained on 11 classes (Noload, Fan, Rotor-0, A10/A30/A50, A&B50, A&C10/A&C30, A&C&B10/A&C&B30).
- Results (validation): best accuracy 0.983 in-training; macro F1 0.930, micro F1 0.930; binary healthy-vs-faulty detects 1160/1163 faulty and 117/117 healthy correctly.
- Interpolation and before/after GAN figures per class.
- Part 2: experiment testing whether GAN-made healthy images improve the classifier. Implemented but not yet run.

## Data
The dataset (domainA / domainB folders) and model checkpoints are not included. The notebook expects them in Google Drive under `FPGAN/data`.

## Run
Open the notebook in Google Colab with a GPU runtime and mount your Drive.
