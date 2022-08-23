# Official Implementation: "Future Network Traffic Matrix Synthesis and Estimation Based on Deep Generative Models"
Solving Traffic Matrix Estimation problem (in Network Tomography) from link-level measurements, using Variational AutoEncoders (VAEs). The code can be used also for Traffic Matrix Synthesis.

Paper: https://doi.org/10.1109/ICCCN52240.2021.9522222

## Abstract
> Traffic matrices (TMs) contain information that is essential for network management, traffic engineering, and anomaly detection. However, constructing a TM through direct traffic measurements has a high administrative and computational cost. A more feasible approach is to estimate the TM from the easily obtainable link load measurements. In this paper, we address the issue of traffic matrix estimation (TME) from link loads using a deep generative model – namely, a variational autoencoder (VAE) – to solve the respective ill-posed inverse problem. In particular, we train the VAE with historical data (previously observed TMs) and we leverage the trained decoder to transform TME into a minimization problem in the latent space, which in turn can be solved by employing a gradient-based optimizer. Furthermore, the trained decoder can be used for traffic matrix synthesis, i.e., for generating synthetic TM examples that have “similar” properties to the samples of the training set. Finally, we explore the incremental optimization of the sequence of objectives constructed from the sequence of decoders that we obtain at different stages of the VAE training. The performance of the proposed methods is evaluated using a publicly available dataset of actual traffic matrices recorded in a real backbone network.

## Requirements
This project has been developed and tested in Python 3.6.9 and requires the following libraries:

- NumPy
- Matplotlib
- Tensorflow

## Usage
1. Download Traffic Matrices and Topology from this [link](https://drive.google.com/drive/folders/1aDblnkqurgLeDxA9Cp2kPPepb13J91Ps?usp=sharing)
2. Clone the repo
```sh
   git clone https://github.com/MikeKalnt/VAE-TME.git
```
3. Add the downloaded files in the startup folder, change current directory and enter the startup folder
```sh
   cd src/
```
4. Open jupyter notebook `vae.ipynb` and select Run All Cells

## Authors
- Kalntis Michail -  [m.kalntis@tudelft.nl](mailto:m.kalntis@tudelft.nl) / [mikekal2611@gmail.com](mailto:mikekal2611@gmail.com)
- Kakkavas Grigoris - [gkakkavas@netmode.ntua.gr](mailto:gkakkavas@netmode.ntua.gr)

## Citing Work
If you used this code in your research, please cite the following:

### BibTeX
```
@inproceedings{kakkavas21,
   author={Kakkavas, Grigorios and Kalntis, Michail and Karyotis, Vasileios and Papavassiliou, Symeon},
   booktitle={2021 International Conference on Computer Communications and Networks (ICCCN)},
   title={{Future Network Traffic Matrix Synthesis and Estimation Based on Deep Generative Models}},
   year={2021},
   pages={1-8},
   doi={10.1109/ICCCN52240.2021.9522222}
}
```
### Plain Text
G. Kakkavas, M. Kalntis, V. Karyotis and S. Papavassiliou, "Future Network Traffic Matrix Synthesis and Estimation Based on Deep Generative Models," _2021 International Conference on Computer Communications and Networks (ICCCN)_, 2021, pp. 1-8, doi: 10.1109/ICCCN52240.2021.9522222.

## Licence 
Distributed under the MIT License. See [LICENCE](https://github.com/MikeKalnt/VAE-TME/blob/main/LICENSE) for more information.
