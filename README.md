# Test various hugging face models

## Apple M1

CONDA_SUBDIR=osx-arm64 conda create -n pt-hf python=3.10
conda env config vars set CONDA_SUBDIR=osx-arm64

conda install -n pt-hf ipykernel --update-deps --force-reinstall
conda install ipykernel
conda install transformers
conda install datasets
conda install scikit-learn

## Windows CUDA
conda create -n pt-hf python=3.10
conda activate -n pt-hf
conda install pytorch torchvision torchaudio pytorch-cuda=11.7 -c pytorch -c nvidia
conda install ipykernel
conda install transformers
conda install datasets
conda install scikit-learn
