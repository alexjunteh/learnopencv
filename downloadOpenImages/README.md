Fast Image Downloader for Open Images V4

1. Install awscli

`sudo pip3 install awscli` 

2. Get the relevant OpenImages files needed to locate images of interest

`wget https://storage.googleapis.com/openimages/2018_04/class-descriptions-boxable.csv`

`wget https://storage.googleapis.com/openimages/2018_04/train/train-annotations-bbox.csv`
  
 For windows: `python -m wget <URL>`

3. Download the images from OpenImagesV4

`python3 downloadOI.py --classes 'Ice_cream,Cookie' --mode train`

If there is a space in the class name, it should be replaced by an underscore(‘_’), e.g in the case of 'Ice cream' as shown above.
