# 只有训练没有数据集 晚点测试

recaptured-image-detection-ICDIP-2022
An open source code for paper "Identifying Recaptured Images Using Deep Correlation"


## Our Environemnt Setting
* Ubuntu 20.04
* Python 3.8
* NVIDIA GPU CUDA 10.2 + cuDNN 8.1.0
* PyTorch 1.9.1
* Pillow 8.3.1


## Data Path
* Train:
  ./data/train_image/NI
  ./data/train_image/RI
* validation:
  ./data/val_image/NI
  ./data/val_image/RI
* Test:
  ./data/test_image/NI
  ./data/test_image/RI


## Run
* Training: Set parameters in 'train.py' or at the command line.
```python
python train.py --batch-size 64 --patch-size 96 --epoch 400 --lr 0.001
```
* Testing: Run ```python test.py```.


## Acknowledgment
This code refers to [JCST_NIvsCG](https://github.com/Evergrow/JCST_NIvsCG).
