```markdown
# Text-to-Image Generation

A simple Python script that uses Hugging Face’s Stable Diffusion pipeline to turn text prompts into images in real‑time. Built with PyTorch, Diffusers, and Transformers, this demo lets you experiment with generative AI on your local GPU or Colab.

---

## 🚀 Features

- **Real‑time inference** of Stable Diffusion v1.4  
- Automatic half‑precision (fp16) for faster GPU performance  
- Simple CLI prompt interface  
- Plots output inline using Matplotlib  

---

## 📋 Prerequisites

- **Python 3.8+**  
- **CUDA‑enabled GPU** (recommended for speed)  
- A Hugging Face account & [access token](https://huggingface.co/settings/tokens)  

---

## 🔧 Installation

1. Clone the repo (or copy the script into your project folder):
   ```bash
   git clone https://github.com/YourUser/YourRepo.git
   cd YourRepo
   ```

2. Create and activate a virtual environment (optional but recommended):
   ```bash
   python -m venv .venv
   source .venv/bin/activate     # Linux / macOS
   .venv\Scripts\activate        # Windows
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Export your Hugging Face token:
   ```bash
   export HF_TOKEN="your_huggingface_token"    # Linux / macOS
   set HF_TOKEN="your_huggingface_token"       # Windows
   ```

---

## ▶️ Usage

Run the script and enter your prompt when prompted:

```bash
python text_to_image_generation_.py
```

1. The script will load the `CompVis/stable-diffusion-v1-4` model in half‑precision.  
2. When prompted, enter a text description (e.g. “A futuristic cityscape at sunset”).  
3. The generated image will appear inline via Matplotlib.  
4. Repeat for up to six prompts per run.

---

## 🛠️ Configuration

- **Model**: Change `modelid` in the script to any compatible Diffusers model ID.  
- **Device**: Toggle `device = "cuda"` or `"cpu"` at the top of the script.  
- **Guidance Scale**: Adjust `guidance_scale=8.5` to control creativity vs. fidelity.

---

## 📂 Repository Structure

```
.
├── requirements.txt
├── text_to_image_generation_.py
└── README.md
```

