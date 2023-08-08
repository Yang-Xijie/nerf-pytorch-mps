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

> NotImplementedError: The operator 'aten::searchsorted.Tensor' is not currently implemented for the MPS device. If you want this op to be added in priority during the prototype phase of this feature, please comment on https://github.com/pytorch/pytorch/issues/77764. As a temporary fix, you can set the environment variable `PYTORCH_ENABLE_MPS_FALLBACK=1` to use the CPU as a fallback for this op. WARNING: this will be slower than running natively on MPS.
