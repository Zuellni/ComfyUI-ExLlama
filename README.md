# ComfyUI ExLlama Nodes
A simple text generator for [ComfyUI](https://github.com/comfyanonymous/ComfyUI) utilizing [ExLlamaV2](https://github.com/turboderp/exllamav2).

## Installation
Make sure your ComfyUI is up to date. Clone the repository to `custom_nodes` and install dependencies:
```
git clone https://github.com/Zuellni/ComfyUI-ExLlama-Nodes
pip install -r requirements.txt
```

Optionally, you can also install [flash-attention](https://github.com/Dao-AILab/flash-attention) by uncommenting the relevant lines in the requirements file. If you see any ExLlama-related errors while loading, install it manually following the instructions from [here](https://github.com/turboderp/exllamav2#method-2-install-from-release-with-prebuilt-extension).

## Nodes
Name | Description
:--- | :---
Loader | Used to load EXL2/GPTQ Llama models. You can find a lot of them on [Hugging Face](https://huggingface.co/TheBloke). Clone the model repository or download all the files in it and place them in an empty directory, then specify the path in `model_dir`. The `model.safetensors` file won't work on its own.
Generator | Generates a `string` based on the given input for use with other nodes.
Preview | Displays generated outputs in the UI.
Replace | Replaces variables enclosed in brackets, such as `[a]`, with their values.

## Workflow
The image below can be opened in ComfyUI.

![workflow](https://github.com/Zuellni/ComfyUI-ExLlama-Nodes/assets/123005779/26acb5fd-f2d9-473a-b0cf-6c92af3bac90)
