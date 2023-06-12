---
cover: https://live.staticflickr.com/65535/52962003503_3c0d1ddfc1_h.jpg
coverY: -201
---

# ⚙ Stable Diffusion

Stable Diffusion is an advanced AI text-to-image synthesis algorithm that can generate very coherent images based on a text prompt.

&#x20;It is commonly used for generating artistic images but can also generate images that look more like photos or sketches. Stable Diffusion is good at generating faces and realistic 3D scenes.

&#x20;It is also good at mashing up concepts to create entirely novel images.&#x20;

Stable Diffusion is entirely <mark style="color:red;">**open source**</mark>, and users can even train their own models based on their own dataset to get it to generate exactly the kind of images they want.

#### ControlNet

ControlNet is a <mark style="color:green;">**neural network architecture**</mark> designed to <mark style="color:green;">**manage diffusion models**</mark> by incorporating additional conditions. It duplicates the weights of neural network blocks into a "locked" copy and a "trainable" copy. The <mark style="color:green;">**"trainable" copy**</mark> learns the **desired condition,** while the <mark style="color:green;">**"locked" copy**</mark>** preserves the original model**. This approach ensures that training with small datasets of image pairs does not compromise the integrity of production-ready diffusion models. The "zero convolution" is a 1×1 convolution with both weight and bias initialized to zero. Before training, all zero convolutions produce zero output, preventing any distortion caused by ControlNet. No layer is trained from scratch; the process is still fine-tuning, keeping the original model secure. This method enables training on small-scale or even personal devices.
