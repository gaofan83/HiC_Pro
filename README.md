#### Installation of HiC-Pro to run GSE159622
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
make configure
sudo make install
cd annotation
../bin/utils/digest_genome.py -r mboi -o MboI_resfrag_mm10.bed ~/reference_genome/Mus_musculus/UCSC/mm10/Sequence/WholeGenomeFasta/genome.fa
cd ~/Data_hiC/GSE159622
cp /home/fgao/HiC-Pro-v3.1.0/HiC-Pro-3.1.0/annotation/MboI_resfrag_mm10.bed .

```
