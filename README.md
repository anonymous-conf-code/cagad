# Counterfactual Data Augmentation for Graph Anomaly Detection with Diffusion Probabilistic Models

This is an anonymous repository hosting the code of CAGAD for double-blind review. 

## Data

- For T-Finance dataset, you can download it from the baseline paper BWGNN: https://proceedings.mlr.press/v162/tang22b.html
- For PubMed, Amazon, and Yelp datasets, they will be automatically downloaded when runinng the code.    

## Dependencies

Run the following command to install dependencies with Anaconda virtual environment:
```shell
conda create -n cagad python==3.9
conda activate cagad
conda install pytorch torchvision torchaudio cudatoolkit=11.3 -c pytorch
conda install -c dglteam dgl-cuda11.3
pip install -r requirements.txt
```

## Run

```shell
# PubMed
python main.py --dataset=pubmed

# T-Finance
python main.py --dataset=tfinance

# Amazon
python main.py --dataset=amazon

# Yelp dataset
python main.py --dataset=yelp --homo=0
```

Description of hyper-parameters can be found in `main.py`.