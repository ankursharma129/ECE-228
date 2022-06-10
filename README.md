# Synthesis QoR prediction

For linear regression and neural network model: Run the .ipynb file from first cell to last

For the GCN, I used the following environment:

`python 3.8, pytorch 1.7.1, cuda 10.1, pytorch geometric`

Once this environment is setup, you'll need to download the 19GB dataset from https://zenodo.org/record/6399454#.YqKJXnbMJmN

Then you need to use the following command from the GCN directory: 
`python train.py --lr 0.01 --lp 1 --epochs 10 --dataset set1 --rundir ./results/ --datadir "path to \OPENABC2_DATASET" --target delay`


Note: A lot of the directory parsing and data reading code has been borrowed from OpenABC repository. This dataset processing is very specific and we were better off using the pytorch processing code that the author provided.
