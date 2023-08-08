# mps

```
conda create --name nerf-mps
conda activate nerf-mps
conda install pytorch torchvision -c pytorch-nightly
pip install -r requirements-mps.txt
```

```
conda activate nerf-mps
PYTORCH_ENABLE_MPS_FALLBACK=1 python run_nerf.py --config configs/lego.txt
```
