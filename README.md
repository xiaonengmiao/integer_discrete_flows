# Integer Discrete Flows and Lossless Compression

This repository contains the code for the experiments presented in [1].

## Usage

### CIFAR10 setup:
```
python main_experiment.py --n_flows 8 --n_levels 3 --n_channels 512 --coupling_type 'densenet' --densenet_depth 12 --n_mixtures 5 --splitprior_type 'densenet'
```


### ImageNet32 setup:
```
python main_experiment.py --evaluate_interval_epochs 5 --n_flows 8 --n_levels 3 --n_channels 512 --n_mixtures 5 --densenet_depth 12 --coupling_type 'densenet' --splitprior_type 'densenet' --dataset 'imagenet32' --epochs 100 --lr_decay 0.99
```


### ImageNet64 setup:
```
python main_experiment.py --evaluate_interval_epochs 1 --n_flows 8 --n_levels 4 --n_channels 512 --n_mixtures 5 --densenet_depth 12 --coupling_type 'densenet' --splitprior_type 'densenet' --dataset 'imagenet64' --epochs 20 --lr_decay 0.99 --batch_size 64
```


### Tiny ImageNet 200 setup:
```
python main_experiment.py --evaluate_interval_epochs 1 --n_flows 8 --n_levels 4 --n_channels 512 --n_mixtures 5 --densenet_depth 12 --coupling_type 'densenet' --splitprior_type 'densenet' --dataset 'tiny-imagenet-200' --epochs 20 --lr_decay 0.99 --batch_size 64
```


# Acknowledgements
The Robert Bosch GmbH is acknowledged for financial support.

# References 
[1] Hoogeboom, Emiel, Jorn WT Peters, Rianne van den Berg, and Max Welling. "Integer Discrete Flows and Lossless Compression." Conference on Neural Information Processing Systems (2019).

