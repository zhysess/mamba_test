# mamba_test


## create conda environment

```
conda create -n mamba_test python=3.10.13
conda activate mamba_test
conda install cudatoolkit==11.8 -c nvidia
pip install torch==2.1.1 torchvision==0.16.1 torchaudio==2.1.1 --index-url https://download.pytorch.org/whl/cu118
conda install -c "nvidia/label/cuda-11.8.0" cuda-nvcc
conda install packaging
git clone https://github.com/Dao-AILab/causal-conv1d.git
cd causal-conv1d
pip install .
pip install mamba-ssm==1.2.0
pip install spectral
pip install scikit-learn
```

```
python train_MambaHSI.py
```
