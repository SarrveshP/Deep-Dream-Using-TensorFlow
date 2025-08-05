
# 🌌 DeepDream with TensorFlow

> A deep dive into neural network interpretability and visual creativity using feature visualization, Laplacian pyramid normalization, and multiscale optimization.


## 🧠 Project Overview

This project explores the internal representations of deep convolutional neural networks (CNNs) using DeepDream — a technique developed by Google to visualize and amplify the patterns learned by a neural model.

We use TensorFlow to generate surreal, dream-like images by optimizing input images to activate certain layers or channels of the **GoogLeNet** (Inception) architecture. The project also integrates **Laplacian Pyramid Gradient Normalization** and **tiled, multiscale rendering** to improve image quality and computational efficiency.

---

## 📌 Features

- ✅ Visualize feature maps and channels of pretrained CNNs (GoogLeNet)
- 🎨 Generate DeepDream-style imagery (including surreal objects like "DogSlugs")
- 🧱 Implement Laplacian Pyramid Gradient Normalization to control frequency components
- 🖼️ Optimize across multiple scales for high-resolution and detailed outputs
- 🧩 Use tiled computation to efficiently render large images
- 📈 TensorBoard graph visualizations embedded directly in Jupyter Notebooks

---

## 🧰 Tech Stack

- **Language:** Python 3.x
- **Frameworks:** TensorFlow 1.x
- **Libraries:** NumPy, PIL, IPython, Jupyter Notebook
- **Models Used:** GoogLeNet (Inception architecture pretrained on ImageNet)

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/deepdream-tensorflow.git
cd deepdream-tensorflow
````

### 2. Install Dependencies

Create a virtual environment (optional):

```bash
python -m venv venv
source venv/bin/activate  # or .\venv\Scripts\activate on Windows
```

Install required libraries:

```bash
pip install tensorflow==1.15 numpy pillow ipython
```

### 3. Download Pretrained Model

Download the TensorFlow version of **GoogLeNet (Inception)** from [here](https://storage.googleapis.com/download.tensorflow.org/models/inception5h.zip).
Unzip it and place the `tensorflow_inception_graph.pb` file in the root directory.

### 4. Run the Notebook

```bash
jupyter notebook deepdream.ipynb
```

---

## 🖼️ Example Outputs

| Visualizing Channel              | Laplacian Normalized Output    | DeepDream Final              |
| -------------------------------- | ------------------------------ | ---------------------------- |
| ![img1](./samples/channel65.jpg) | ![img2](./samples/lapnorm.jpg) | ![img3](./samples/dream.jpg) |

> Tip: Use higher-resolution images and multiple octaves for more dramatic effects.

---

## 📚 Key Concepts

### 🌀 DeepDream

A technique to enhance and amplify patterns learned by CNNs by maximizing activations of specific neurons or channels, producing hallucination-like images.

### 🏛️ Laplacian Pyramid

A multi-scale representation of images used to normalize gradients across frequency bands, enhancing smoothness and detail in generated images.

### 🧩 Tiled Gradient Computation

Reduces memory usage and supports high-res image generation by computing gradients over overlapping tiles.

---

## 📈 Use Cases

* 🎨 Generative art
* 🔬 Model interpretability and explainable AI (XAI)
* 📊 Feature visualization in computer vision models
* 🧪 Educational projects on CNN internals

---

## 🧑‍💻 Author

**Sarvesh Patil**
Master of Computer Applications (MCA), Manipal University Jaipur
AI | Data Science | Computer Vision

[![LinkedIn](https://img.shields.io/badge/LinkedIn-blue?logo=linkedin)](https://www.linkedin.com/in/sarveshpatil1311)


---

## 🌟 Acknowledgements

* Google DeepDream Research: [Inceptionism](https://research.googleblog.com/2015/06/inceptionism-going-deeper-into-neural.html)
* TensorFlow Tutorials
* OpenAI & Deep Learning Communities
