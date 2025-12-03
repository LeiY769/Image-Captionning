# Flickr images
```
mkdir -p data/flickr8k
wget https://github.com/jbrownlee/Datasets/releases/download/Flickr8k/Flickr8k_Dataset.zip
unzip Flickr8k_Dataset.zip
mv Flicker8k_Dataset/* data/flickr8k/images/

mkdir -p data/flickr30k
pip install -U "huggingface_hub[cli]"
hf download nlphuji/flickr30k --repo-type dataset --include "flickr30k-images.zip" --local-dir data/flickr30k
```

# Splits
```
https://github.com/Delphboy/karpathy-splits/tree/main
```

