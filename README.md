# Training and Inference Guidelines
## Training the model:
* Prepraring the environment by installing required packages in the requirements.txt file:
* Preparing the train dataset with the COCO format which suits the model's input format.
* from the main root directory, use this command: **bash tools/dist_train.sh train_config.py number_of_devices "device-1th, device-2th,...device-Nth"**
## Inference process:
* Change the input_path in the <u>**infer.py**<u/> or <u>**infer_one_image.py**<u/> as well as the output path*.
* Run the command **python infer.py* if you want to infer the result of a folder of images or  **python infer_one_image.py** if you want to predict only one image.
