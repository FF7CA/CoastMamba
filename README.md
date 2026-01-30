# CoastMamba

**CoastMamba** is an implementation of the paper CoastMamba: A Boundary-Enhanced Mamba Framework for  Sea-Land Segmentation in Optical Remote Sensing Imagery

**Note**：This repository is undergoing revisions, and our paper is still under review.

## Installation

```
conda create --n aerith python=3.12 && conda activate aerith
pip install -r requirement.txt
```

## Dataset

### Download the dataset

For SLSD:

For HRSC2016:

For MinnanSLS:

### Data processing

The dataset folder under */dataset* should as follows.

```
data
|----SLSD
|--------train
|--------val
|--------test
|----HRSC2016
|----MinnanSLS
```

# Get start

## Training

```
python train_supervision.py -c ./config/SLSD/CoastMamba.py
```
```
python train_supervision.py -c ./config/HRSC2016/CoastMamba.py
```
```
python train_supervision.py -c ./config/MinnanSLS/CoastMamba.py
```

## Testing

```
python SLS_seg_test.py -c ./config/SLSD/CoastMamba.py -o /root/results/SLSD/CoastMamba --rgb -t 'lr'
```
```
python SLS_seg_test.py -c ./config/HRSC2016/CoastMamba.py -o /root/results/HRSC2016/CoastMamba --rgb -t 'lr'
```
```
python SLS_seg_test.py -c ./config/MinnanSLS/CoastMamba.py -o /root/results/MinnanSLS/CoastMamba --rgb -t 'lr'
```

## Thanks



