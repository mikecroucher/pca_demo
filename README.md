# Using conda environments
The Jupyter notebook in this repoo uses an old version of Scikit-learn's `RandomizedPCA` function that won't work in modern versions of the library.

This was done to demonstrate the use of Conda environments.  
The `environment.yml` file was created from my live environment using the command

```
conda env export > environment.yml
```

Get the code
```
git clone https://github.com/mikecroucher/pca_demo
cd pca_demo
```

Create the conda environment from the `environment.yml` file in this repo and run the notebook server
```
conda env create -f environment.yml
conda activate old_scikit
jupyter notebook
```
