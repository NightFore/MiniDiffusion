# MiniDiffusion

MiniDiffusion is a student project aimed at understanding and implementing a basic diffusion model for image generation. The goal is to learn about diffusion models and eventually add features like LoRA and ControlNet.

## Features

- Basic image generation using diffusion models
- Simple setup with PyTorch and Diffusers
- Supports generating single and batch images from text prompts

## Setup

1. Clone the repository:

    ```bash
    git clone https://github.com/NightFore/MiniDiffusion.git
    cd MiniDiffusion
    ```

2. Install the necessary dependencies listed in the notebook.  
   Open the notebook and follow the instructions to install PyTorch, Diffusers, and other required libraries.

   Example installation commands you might find in the notebook:

    ```bash
    pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu124
    pip install --upgrade diffusers accelerate transformers
    pip install pillow ipywidgets tqdm
    ```

3. Ensure that you have **Python 3.12.8** and **PyTorch with CUDA** installed.

## Usage

To generate images, you can run the provided Jupyter notebook:

1. Open the notebook and set up the model.
2. Adjust the prompt and settings to generate images.

Example in the notebook:

```python
# Example: Generate a single image
image = pipeline(prompt="A mystical landscape", generator=generator).images[0]
image
```

## Directory Structure

- `assets/`: Stores models and cache
- `images/`: Where the generated images are saved

## Future Plans

- Add LoRA (Low-Rank Adaptation) support
- Implement ControlNet for more control over image generation

## License

This project is licensed under the MIT License.
