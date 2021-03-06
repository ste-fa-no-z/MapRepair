# MapRepair
This repository contains the implementation for our publication "Map-Repair: Deep Cadastre Maps Alignment and Temporal Inconsistencies Fix in Satellite Images", IGARSS 2020. 
If you use this implementation please cite the following publication:

~~~
@article{zorzi2020map,
  title={Map-Repair: Deep Cadastre Maps Alignment and Temporal Inconsistencies Fix in Satellite Images},
  author={Zorzi, Stefano and Bittner, Ksenia and Fraundorfer, Friedrich},
  journal={arXiv preprint arXiv:2007.12470},
  year={2020}
}
~~~

<p align="center"><img width=100% src="README.gif"></p>

Explanatory video of the approach:

[![Watch the video](https://img.youtube.com/vi/glNhDSu1y2U/maxresdefault.jpg)](https://youtu.be/glNhDSu1y2U)

# Dependencies

*  cuda 10.2
*  pytorch >= 1.3
*  kornia
*  opencv
*  gdal

# Running the implementation
After installing all of the required dependencies above you can download the pretrained weights from [here](https://drive.google.com/drive/folders/1eBxSML1lCa7GS-NNrDOe_hGT09SpQNNC?usp=sharing).

Unzip the archive and place the content in the main *maprepair* folder.
The folder *saved_models* contains the pretrained weights both for MapRepair and the regularization network.
 
## Evaluation
Modify *variables.py* accordingly, then run the prediction issuing the command

~~~
python predict.py
~~~

## Training
Modify *variables.py* accordingly, then run the training issuing the command

~~~
python train_net.py
~~~
