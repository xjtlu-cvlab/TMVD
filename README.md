Qiu, R., Xu, M., Ling, Y., Smith, J. S., Yan, Y., & Wang, X. (2024). A Deep Top-down Framework towards Generalisable Multi-View Pedestrian Detection. Neurocomputing, 607, Article 128458. https://doi.org/10.1016/j.neucom.2024.128458


Dependencies
The programme uses the following libraries:
python 3.7+
pytorch 1.4+ & tochvision
numpy
matplotlib
pillow
opencv-python
matlab & matlabengine


Data Preparation
The datasets need to be downloaded from their official websites before running the program.

Wildtrack: https://www.epfl.ch/labs/cvlab/data/data-wildtrack/

Multiviewx: https://github.com/hou-yz/MVDet/

By default, all datasets are put in ~/Data/. The ~/Data/ folder should look like this Data

├── MultiviewX/

│ └── ...

└── Wildtrack/
	

Training
For training, please run the programme as follows:
python main.py -d Wildtrack or python main.py -d multiviewx


Pre-Trained Models
The pre-trained models can be downloaded from 
https://drive.google.com/file/d/1YdF1RbU816JkuT4FYrzleog559PnAjub/view?usp=sharing.

The programme can be run with the pre-trained models for testing:
python main.py -d wildtrack --resume PATH or python main.py -d multiviewx --
resume PATH
The “PATH” is the path of a pre-trained model.


The GPU Requirements
The RTX3090 is recommended for the training to ensure sufficient GPU memory.
