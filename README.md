# Training and Inference Guidelines
## Training the model:
• Prepraring the environment by installing required packages in the requirements.txt file:
* Preparing the train dataset with the COCO format which suits the model's input format.
* from the main root directory, use **bash tools/dist_train.sh train_config.py number_of_devices "device-1th, device-2th,...device-Nth"**
