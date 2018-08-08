# Multiscale Neural Network (MNN) based on hierarchical nested bases
This repo is the code for the paper: https://arxiv.org/abs/1808.02376
The code to generate data is written by MATLAB and the neural network is implemented by python based on keras on top of tensorflow

## How to run
- generate data by matlab code
- run the code in the tensorflow environment 

We take RTE as an example.

The main file of the matlab code is __NLSEsample.m__ for 1d and __NLSEsample2d.m__ for 2d.

The neural network use _argparse_ to set the parameters. One can use 
```
	python testH2matrix.py --help  
```
to print the usage of all the parameters and its default values.
One example to run the code:
```
	python testHmatrix.py --epoch 200 --alpha 4 --output-suffix V1
```

We note that the code for Kohn-Sham map is same as that for NLSE, thus we only provide the codes for NLSE and RTE.
