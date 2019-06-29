
project se dum internet ta ge zeng nga ga sembani ei ML ge maramda amabu khangde dum try tauraga yaba zeng nge ni.

Kok amasung sum ge photo 13 khak train tauraga zengini. Train model semba loidri.

DataSet se yam na leek ee yagadauba mande image 100-200 gumba chang gani alphabet khudingmak ki.

INSTALL SETUP

You need to clone the tensorflow/model from their repository and clone this repository and paste to research/objectdetection folder.

clone this repo here https://github.com/tensorflow/models  and clone this repo and paste all the files to research/object_detection folder

Follow the installation setup in this link https://github.com/tensorflow/models/blob/master/research/object_detection/README.md


IMPORTANT 

download http://download.tensorflow.org/models/object_detection/faster_rcnn_inception_v2_coco_2018_01_28.tar.gz

and extract to the objectdetection folder.
And also change the path in the faster_rcnn_inception_v2_pets.config file in training folder.

and lasty run train.py as  python train.py --logtostderr --train_dir=training/ --pipeline_config_path=training/faster_rcnn_inception_v2_pets.config