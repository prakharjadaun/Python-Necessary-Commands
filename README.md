# **Python Necessary Commands**

This repository contains several commands which can be helpful in ML projects and you should know.

## Pip

- To upgrade pip
```
python -m pip install --upgrade pip
```
- To check the version of pip
```
pip --version
```
- To downgrade the pip version
```
python -m pip install pip==version_name
```
- To get all the packages installed, along with their specific version and location.
```
pip list
```
- To resolve conflicts when installing requirements.txt using pip
```
!pip install -r requirements.txt --use-deprecated=legacy-resolver
```
## Conda

- To create a virtual environment using conda (you can use any version of python)
```
conda create -p venv python==3.10.0 -y
```
- To activate a virtual environment you created locally (venv is the name of virtual env)
```
conda activate venv/
```
- If pip not working in virtual env ([source](https://stackoverflow.com/questions/37220055/pip-fatal-error-in-launcher-unable-to-create-process-using))
```
python -m pip install --upgrade --force-reinstall pip
```
## Keras

- To save keras model
```
# after training
model.save("model_name.h5")
```
- To load the keras model
```
model = keras.models.load_model("model_name.h5")
```
- To save keras model's weight
```
model.save_weights("model_weights.h5")
```
- To load the weights
```
model.load_weights("model_weights.h5)
```
- To save the architecture as json
```
json_string = model.to_json()
with open("filename","w") as f:
  f.write(json_string)
```
- To load the json file:
```
with open("filename","r") as f:
  loaded_json_string = f.read();
```
## HuggingFace

- Remove downloaded Tensorflow and Pytorch(HuggingFace) Models ([source](https://stackoverflow.com/questions/65037368/remove-downloaded-tensorflow-and-pytorchhugging-face-models))
```
huggingface-cli delete-cache
```
