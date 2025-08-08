# TBN

This repository is the official implementation of the paper "TBN: An All-in-One Triplet Branch Network for Adverse Weather Cross-View Geo-Localization"

## 🈸Dataset Access

Please prepare [University-1652](https://github.com/layumi/University1652-Baseline), [SUES-200](https://github.com/Reza-Zhu/SUES-200-Benchmark)

## 📂Dataset Structure

#### University-1652 Dataset Directory Structure

```shell
├── University-1652/
│   ├── train/
│       ├── drone/                   /* drone-view training images 
│           ├── 0001
|           ├── 0002
|           ...
│       ├── satellite/               /* satellite-view training images       
│   ├── test/
│       ├── query_drone/  
│       ├── gallery_drone/  
│       ├── query_satellite/  
│       ├── gallery_satellite/ 
```

#### SUES-200 Dataset Directory Structure

```shell
├─ SUES-200
  ├── Training
    ├── 150/
    ├── 200/
    ├── 250/
    └── 300/
  ├── Testing
    ├── 150/
    ├── 200/ 
    ├── 250/	
    └── 300/
```

## 💯Train and Test

For University-1652 Dataset

```sh
Train: run train_university.py, with --only_test = False.

Test: run train_university.py, with --only_test = True, and choose the model in --ckpt_path.
```

For SUES-200 Dataset

```sh
Train: run train_SUES-200.py, with --only_test = False.

Test: run train_SUES-200.py, with --only_test = True, and choose the model in --ckpt_path.
```

## ❤️Acknowledgments

This repository is built using the [Sample4Geo](https://github.com/Skyy93/Sample4Geo), [MCCG](https://github.com/mode-str/crossview), [DAC](https://github.com/SummerpanKing/DAC) and [MEAN](https://github.com/ISChenawei/MEAN) repositories.

