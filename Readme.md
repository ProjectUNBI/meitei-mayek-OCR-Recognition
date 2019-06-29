# MeiTeiMayek OCR testing

project se dum internet ta ge zeng nga ga sembani ei Machine Learning ge maramda amabu khangde dum try tauraga yaba zeng nge ni.

Kok amasung sum ge photo 13 khak train tauraga zengini. Train model semba loidri.

## NOTE

Se da ge se yadi yai pung 3 hr bu train taurene kok tang detect tauba ngam me adubu sum de fajana detect tauba ngamde Image data set se fajana sem ma di yaba yai
. adubu eige laptop se nvidia graphic yauba card natte adugi maram oi na fajana train tauba yade.

## Installation

You need to clone the tensorflow/model from their repository and clone this repository and paste to research/objectdetection folder.


clone this repo here [Link](https://github.com/tensorflow/models )  and clone this repo and paste all the files to research/object_detection folder

Follow the installation setup in this link [Link tutorial](https://github.com/tensorflow/models/blob/master/research/object_detection/g3doc/installation.md)


```bash
pip install tensorflow
pip install Protobuf 3.0.0
pip install Python-tk
pip install Pillow 1.0
pip install lxml

pip install Jupyter notebook
pip install Matplotlib
pip install Tensorflow (>=1.12.0)
pip install Cython
pip install contextlib2
pip install pycocotools
```

## Important

download this 150 mb [Link](http://download.tensorflow.org/models/object_detection/faster_rcnn_inception_v2_coco_2018_01_28.tar.gz)
and extract to the objectdetection folder.
And also change the path in the faster_rcnn_inception_v2_pets.config file in training folder.

and lasty run train.py as  
```
python train.py --logtostderr --train_dir=training/ --pipeline_config_path=training/faster_rcnn_inception_v2_pets.config
```
and train it for hours more hour more better after some few hours cancel the training by ctrl-c.

and lastly run this in object_detection folder

```
python export_inference_graph.py --input_type image_tensor --pipeline_config_path training/faster_rcnn_inception_v2_pets.config --trained_checkpoint_prefix training/model.ckpt-XXXX --output_directory inference_graph

```


## Result Kok de detect tauba ngam me 
![KOK](https://i.ibb.co/5FNYXJv/kok.jpg)
## SUM se de detect tauba ngamde eina image to fajana capture taudabage
![sum](https://i.ibb.co/JtRcYPG/sum.jpg)
