#### Installation of HiC-Pro
##### Install miniconda
```
conda env create -f ~/HiC-Pro/environment.yml -p ~/HiC-Pro_ENV
conda activate /home/fgao/HiC-Pro_ENV
wget https://github.com/nservant/HiC-Pro/archive/refs/tags/v3.1.0.tar.gz
mkdir HiC-Pro-v3.1.0
cd HiC-Pro-v3.1.0
mv ../v3.1.0.tar.gz .
tar -xvzf v3.1.0.tar.gz
cd HiC-Pro-3.1.0

```
