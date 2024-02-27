# HeartSoundDenoising

This repository is for the paper "Clearer Lub-Dub: A Novel Approach in Heart Sound Denoising Based on Transfer Learning"

## Dataset

We use the dataset of the [PhysioNet/CinC Challenge in 2016](https://physionet.org/content/challenge-2016/1.0.0/) [1]

Pre-processing data used in the paper are available [here](https://drive.google.com/drive/folders/1w152ZH0Tnvb_vTojDcH9a22jBPJNVUQb?usp=sharing).

Detailed  explaination follows:

`segment_data.pkl` is a (81553, 5000) numpy ndarray, containing all heart sound segments we collected.

>  the segments are 2kHz and last for 2.5s.

`seg_label.pkl` is a (81553,) numpy ndarray, containing the corresponding labels for all segments.

>  where -1 represents normal and 1 represents abnormal, but you should change -1 to 0 during experiments.

`train_idx.pkl` (65243) and  `test_idx.pkl` (16310) are list, containing the index for training and test, respectively.

`splits.pkl` is a list, which contains 5-fold index as tuples. Each fold (tuple) has two ndarray elements, where the first shape is (52194,) and the second shape is (13049,).

## Reference

1. Liu C, Springer D, Li Q, Moody B, Juan RA, Chorro FJ, Castells F, Roig JM, Silva I, Johnson AE, Syed Z, Schmidt SE, Papadaniil CD, Hadjileontiadis L, Naseri H, Moukadem A, Dieterlen A, Brandt C, Tang H, Samieinasab M, Samieinasab MR, Sameni R, Mark RG, Clifford GD. An open access database for the evaluation of heart sound algorithms. Physiol Meas.2016 Dec;37(12):2181-2213
