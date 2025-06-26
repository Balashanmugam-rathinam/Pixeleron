# Pixeleron: Unified Deep Learning Toolkit for Super-Resolution

Pixeleron is a unified, open-source super-resolution toolkit that combines multiple state-of-the-art deep learning models into one modular and user-friendly platform. It supports high-quality image enhancement, face restoration, and video upscaling through a smart Streamlit-based interface and batch processing pipeline. Pixeleron is ideal for researchers, developers, and creators looking to deploy scalable and accurate super-resolution solutions.

## 🚀 Key Features
- 🔍 Smart Model Selector: Automatically routes input to the appropriate model (image, face, or video)
- 🧠 Integrated Models: SRGAN, ESRGAN, Real-ESRGAN, SwinIR, GFPGAN
- 🖼 Face Restoration: GFPGAN integration for natural facial detail reconstruction
- 📹 Video Frame Upscaling: SwinIR and Real-ESRGAN video frame-by-frame enhancement
- 💡 Streamlit GUI: Clean, interactive UI for non-coders and quick prototyping
- ⚙️ ONNX/TFLite Export: Deploy models on edge devices and mobile platforms
- 📊 Evaluation Metrics: Built-in support for PSNR, SSIM, and LPIPS benchmarking
- 🐳 Docker Support: Containerized setup for easy deployment

## 📁 Project Structure
```
super_resolution_toolkit/
│
├── app/                            # Main application logic
│   ├── __init__.py
│   ├── gui.py                      # Streamlit GUI
│   ├── processor.py               # Main logic to route inputs to models
│   ├── model_selector.py          # Smart model selector (image/video/face)
│   ├── utils.py                   # Utility functions (resize, metrics, etc.)
│   └── export.py                  # ONNX/TFLite export logic
│
├── models/                        # Model loading and wrappers
│   ├── __init__.py
│   ├── srgan.py
│   ├── esrgan.py
│   ├── real_esrgan.py
│   ├── swinir.py
│   └── gfpgan.py
│
├── assets/                        # Static files and sample images/videos
│   ├── samples/
│   └── icons/
│
├── configs/                       # Config and model settings
│   ├── model_paths.yaml
│   └── gui_config.yaml
│
├── benchmarks/                    # Benchmark results and test scripts
│   ├── metrics.py
│   └── evaluate_on_datasets.py
│
├── notebooks/                     # Optional Jupyter experiments or demos
│   └── comparison_plot.ipynb
│
├── requirements.txt               # Python dependencies
├── Dockerfile                     # For containerization
├── README.md                      # GitHub documentation
├── .streamlit/config.toml         # Theme & layout settings for Streamlit
└── main.py                        # Entry point for Streamlit app
```

## 📦 Installation
```bash
git clone https://github.com/Balashanmugam-rathinam/Pixeleron.git
cd Pixeleron
pip install -r requirements.txt
streamlit run main.py
```

## 📜 License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## 🙌 Acknowledgments
- [SRGAN](https://github.com/tensorlayer/srgan)
- [ESRGAN](https://github.com/xinntao/ESRGAN)
- [Real-ESRGAN](https://github.com/xinntao/Real-ESRGAN)
- [GFPGAN](https://github.com/TencentARC/GFPGAN)
- [SwinIR](https://github.com/JingyunLiang/SwinIR)
