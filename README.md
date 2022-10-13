# Counterfactual Data Augmentation for Graph Anomaly Detection with Diffusion Probabilistic Models

This is an anonymous repository hosting the code of CAGAD for double-blind review. 

## Data

- For Yelp, Amazon, and PubMed datasets, they will be automatically downloaded when runinng the code.    
- For T-Finance dataset, you can download it from the baseline paper BWGNN: https://proceedings.mlr.press/v162/tang22b.html

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
python main.py --dataset=yelp/amazon/pubmed/tfinance
```

For Amazon and PubMed datasets set the flag `--homo=1`.
