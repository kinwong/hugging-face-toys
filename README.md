# Test various hugging face models

## Apple M1

CONDA_SUBDIR=osx-arm64 conda create -n pt-hf python=3.10
conda env config vars set CONDA_SUBDIR=osx-arm64

conda install -n pt-hf ipykernel --update-deps --force-reinstall
conda install -c conda-forge ipywidgets

conda install transformers
conda install datasets
