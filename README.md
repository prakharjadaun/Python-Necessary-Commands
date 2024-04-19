# **ML-Project-Helper**
Repo contains several commands which can be helpful in ML projects.

## Conda

If pip not working in virtual env ([source](https://stackoverflow.com/questions/37220055/pip-fatal-error-in-launcher-unable-to-create-process-using))
```
python -m pip install --upgrade --force-reinstall pip
```

## HuggingFace

Remove downloaded Tensorflow and Pytorch(HuggingFace) Models ([source](https://stackoverflow.com/questions/65037368/remove-downloaded-tensorflow-and-pytorchhugging-face-models))
```
huggingface-cli delete-cache
```
