Image Enhancement Pipeline

This project includes an image enhancement pipeline based on the Zero-DCE++ low-light enhancement model. The enhancement stage is applied before running the detection pipeline.

1. Download the Zero-DCE++ Repository

Clone the repository:
git clone https://github.com/Li-Chongyi/Zero-DCE_extension.git

2. Copy the Required Directory

From the downloaded repository, copy the Zero-DCE++ folder into this project.

Your folder structure should look like this:
```
project-root
│
├── Image Enhancement Pipeline.ipynb
├── Zero-DCE++
│   ├── model.py
│   ├── dataloader.py
│   ├── lowlight_test.py
│   ├── lowlight_train.py
│   ├── Myloss.py
│   └── snapshots_Zero_DCE++
│       └── Epoch99.pth
│
├── input
└── output
```
3. Update the Paths in the Script

Edit the following variables in Image enhancement pipeline.ipynb:
```python
IMG_DIR = "./input"
OUT_DIR = "./output"

ZERO_DCE_MODEL = "./Zero-DCE++/model.py"
ZERO_DCE_WEIGHTS = "./Zero-DCE++/snapshots_Zero_DCE++/Epoch99.pth"
```
