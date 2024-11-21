# Training and Inference Guidelines
## Activating conda environment:
* Inside the docker container, run this command to activate the conda environment **"codetr_senseX"** which already had necessary packages installed: **conda activate codetr_senseX**.
## Training the model:
* Prepraring the environment by installing required packages in the **requirements.txt** file.
* Preparing the train dataset with the COCO format which suits the model's input format.
* Access to this directory "**WorkingSpace/Personal/longlb/BKAI_VEHICLE/models/alter_codetr/Co-DETR**", and use this command: **bash tools/dist_train.sh train_config.py number_of_devices "device-1th, device-2th,...device-Nth"** to start the training process.
## Inference process:
* Change the input path of a folder of images or an image in the <u>**infer.py**<u/> or <u>**infer_one_image.py**<u/> as well as the output path.
* Change the configuration checkpoint path of the model you want to use in the aforementioned files.
* Access to this directory "**WorkingSpace/Personal/longlb/BKAI_VEHICLE/models/alter_codetr/Co-DETR**", and run the command **python infer.py** if you want to infer the result of a folder of images or  **python infer_one_image.py** if you want to predict only one image.
