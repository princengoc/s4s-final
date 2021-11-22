# Team Hash Brown Science4Cast Submission

This code reproduces Team Hash Brown's (@princengoc, @Xieyangxinyu) best submission for the competition https://www.iarai.ac.at/science4cast

Authors: Ngoc Tran and Yangxinyu Xie

## Setup


Easiest way is to clone the directory

```
git clone https://github.com/princengoc/s4s-final
cd s4s-final
```

Getting the data. 

1. Download data files from the competition's organizers: TODO
2. Unzip and put the data files in the folder s4s/data/raw/

Run the following to install all the required packages.

```buildoutcfg
pip install -r requirement.txt
```

##### HOPREC Embedding

You can get the HOPREC embedding by running the following shell codes.

```buildoutcfg
cd HOPREC
git submodule add https://github.com/cnclabs/smore
cd smore
make
cd ..
python get_HOPREC_embedding.py --year 2017 --t_min 0.5 --t_max 0.9
python get_HOPREC_embedding.py --year 2017 --t_min 0.5 --t_max 1
```

### Reproduce the submission

To reproduce the submission file, do

`python main.py`

