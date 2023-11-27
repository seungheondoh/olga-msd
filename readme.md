# OLGA-MSD Track

To facilitate artist similarity retrieval, aggregation of track embeddings is necessary. The original [OLGA Repository](https://gitlab.com/fdlm/olga) provides AcousticBrainz features for 25 tracks per artist; however, if a specific music encoder is employed, AcousticBrainz features cannot be utilized. To address this, we have created a repository for the reimplementation of mappings between MSD tracks and OLGA.

### Download Dataset
```
cd datasets
git clone https://gitlab.com/fdlm/olga.git
git clone https://github.com/jongpillee/music_dataset_split.git # for check msd
wget http://millionsongdataset.com/sites/default/files/AdditionalFiles/track_metadata.db # for meta mapping
wget http://millionsongdataset.com/sites/default/files/challenge/train_triplets.txt.zip # for popularity
unzip train_triplets.txt.zip
```

### Mapping (OLGA Artist -> MSD Track)

Please check `mapping` repository

### How to get OLGA Ground Turth?

From original paper, the ground truth (i.e., which artists are actually similar to which other artists), this information can be obtained from AllMusic. please check [OLGA Repository](https://gitlab.com/fdlm/olga).