# Single-cell Deep Hashing (scDeepHash)
An automatic cell type annotation and cell retrievalmethod for large-scale scRNA-seq datasets using neuralnetwork-based hashing.

## Quick Start:
- `pip3 install -r requirements.txt` Install dependencies
- `python3 --dataset BaronHuman` Train scDeepHash on Baron Human

*The model successfully runs with Python 3.6.9*


### Options
  - `--checkpoint_path` Path to save checkpoint
  - `--l_r`             learning rate
  - `--lamb`           lambda of quantization loss
  - `--lr_decay`   learning rate decay
  - `--n_layers`   number of layers
  - `--epochs`       number of epochs to run
  - `--dataset {'TM', 'BaronHuman', 'Zheng68K', 'AMB', "XIN", "pbmc68k",
                        "CellBench", "Pancreatic", "AlignedPancreatic",
                        "X10v2", "CelSeq", "DropSeq", "InDrop", "SeqWell", "SmartSeq",
                        "Fetal"}`
                        dataset to train against
                        
  *For more options, please see https://github.com/wbh123456/scDeepHash/blob/master/scDeepHash.py*                      
## Built-in datasets
##### Intra-dataset:
 - Baron Human
 - TM
 - Zheng68K
 - AMB
 - XIN
 - Fetel

##### Inter-dataset:
 - CellBench
 - X10v2
 - Pancreatic
 - AlignedPancreatic
 
## Establish a venv
- `python3 -m venv .venv`
- `pip3 install -r requirements.txt`