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

## HuggingFace

- Remove downloaded Tensorflow and Pytorch(HuggingFace) Models ([source](https://stackoverflow.com/questions/65037368/remove-downloaded-tensorflow-and-pytorchhugging-face-models))
```
huggingface-cli delete-cache
```
