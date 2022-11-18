# Usage

## Step1: Download datasets

Contains DIV2K, DIV8K, Flickr2K, OST, T91, Set5, Set14, BSDS100 and BSDS200, etc.

- [Google Driver](https://drive.google.com/drive/folders/1A6lzGeQrFMxPqJehK9s37ce-tPDj20mD?usp=sharing)
- [Baidu Driver](https://pan.baidu.com/s/1o-8Ty_7q6DiS3ykLU09IVg?pwd=llot)

## Step2: Prepare the dataset in the following format

```text
# Train and valid dataset struct
- DIV2K
    - original
        - DIV2K_train_HR
            - 001.png
            - 002.png
            ...
        - DIV2K_train_LR_unknown_X4
            - 001.png
            - 002.png
            ...
        - DIV2K_valid_HR
            - 801.png
            - 802.png
            ...
        - DIV2K_valid_LR_unknown_X4
            - 801.png
            - 802.png
            ...
```

## Step3: Preprocess the train dataset

```bash
cd <PDM-PyTorch-main>/scripts
python3 run.py
```

## Step4: Check that the final dataset directory schema is completely correct

```text
# All dataset
- DIV2K
    - 2017Track2
        - PDM
            - train
                - GT
                    - 001.png
                    - 002.png
                    ...
                - LR
                    - 001.png
                    - 002.png
                    ...
            - valid
                - GT
                    - 801.png
                    - 802.png
                    ...
                - LR
                    - 801.png
                    - 802.png
                    ...
    - original
```
