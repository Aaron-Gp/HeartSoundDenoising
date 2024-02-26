# HeartSoundDenoising

This repository is for the paper "Clearer Lub-Dub: A Novel Approach in Heart Sound Denoising Based on Transfer Learning"

## Dataset

We use the dataset of the [PhysioNet/CinC Challenge in 2016](https://physionet.org/content/challenge-2016/1.0.0/) [1]

Pre-processing data used in the paper are available [here](https://drive.google.com/drive/folders/1w152ZH0Tnvb_vTojDcH9a22jBPJNVUQb?usp=sharing).

Detailed  explaination:

`train.pkl` is a [65243, 1, 2500] pytorch tensor.

`test.pkl` is a [16310, 1, 2500] pytorch tensor.

`splits.pkl` is a list, which contains 5-fold index as tuples. Each fold (tuple) has two ndarray elements, where the first shape is (52194,) and the second shape is (13049,).

## Reference

1. Liu C, Springer D, Li Q, Moody B, Juan RA, Chorro FJ, Castells F, Roig JM, Silva I, Johnson AE, Syed Z, Schmidt SE, Papadaniil CD, Hadjileontiadis L, Naseri H, Moukadem A, Dieterlen A, Brandt C, Tang H, Samieinasab M, Samieinasab MR, Sameni R, Mark RG, Clifford GD. An open access database for the evaluation of heart sound algorithms. Physiol Meas.2016 Dec;37(12):2181-2213
