# Flickr images
Download the images in data/flickr8k/images and data/flickr30k/flickr30k-images. The following commands should work, but I didnt tested it (to be verified thus). Basically the 2 folders should be filled with .jpg files.
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
Download dataset_flickr32k.json and dataset_flickr8k.json from <https://github.com/Delphboy/karpathy-splits/tree/main> in the data/flickrXk/ folders  
