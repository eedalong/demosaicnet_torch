Light reimplementation of <https://github.com/mgharbi/demosaicnet>.
Runs on python3 (tested on Anaconda for Ubuntu 14.03).
Other dependencies are listed in requirements.

1. Install

```
make setup
```

2. Download the data

```
make download_data
```

3. Train a net

```
make train_bayer
```

4. Test a net

```
make test_bayer
```

Dataset format
--------------

The dataloader assumes the dataset is given as a listing file containing the relative path 
to the images. For example if you have images like:

```
root
├── filelist.txt
├── hdrvdp
│   ├── 000
│   │   ├── 000001.png
│   │   ├── 000002.png
│   │   ├── 000003.png
│   │   ├── 000004.png
│   │   ├── 000005.png
```

filelist.txt should have one path per line as such:

```
hdrvdp/000/000001.png
hdrvdp/000/000002.png
hdrvdp/000/000003.png
hdrvdp/000/000004.png
hdrvdp/000/000005.png
```

etc.
