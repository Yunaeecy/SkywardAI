---
description: step by step from clone the project to generate the QR code
---

# ⚙ Creative QR Codes with ControlNet

{% hint style="info" %}
reference: [https://stable-diffusion-art.com/qr-code/#Japanese\_girl](https://stable-diffusion-art.com/qr-code/#Japanese\_girl)
{% endhint %}

## **Table of contents**

* <mark style="color:blue;">Step 1:</mark> Clone a project from GitHub
* <mark style="color:blue;">Step 2:</mark> Open with GitHub Desktop. Click "Clone"
* <mark style="color:blue;">Step 3:</mark> Install some "Plug-in-board", such as "resource"
* <mark style="color:blue;">Step 4:</mark> Cick terminal input"make prepare" -->"enter"
* <mark style="color:blue;">Step 5:</mark> In termal, input"make run" -->"enter"
* <mark style="color:blue;">Step 6:</mark> Go to img2img to finish the steps.



## 1.Clone a project from GitHub

<figure><img src="../.gitbook/assets/Screenshot 2023-06-12 at 2.39.58 pm.png" alt=""><figcaption></figcaption></figure>

## 2.Open with GitHub Desktop. Click "Clone"

<figure><img src="../.gitbook/assets/Screenshot 2023-06-12 at 2.41.03 pm.png" alt=""><figcaption></figcaption></figure>

## 3.Install some "Plug-in-board", such as "resource".

<figure><img src="../.gitbook/assets/Screenshot 2023-06-12 at 2.46.58 pm.png" alt=""><figcaption></figcaption></figure>

## 4.Cick terminal input"make prepare" -->"enter"

<figure><img src="../.gitbook/assets/Screenshot 2023-06-12 at 3.37.10 pm.png" alt=""><figcaption></figcaption></figure>

## 5.In termal, input"make run" -->"enter"

Then it will generate a URL like: _http://127.0.0.1:7860, click it to go to_ stable diffusion_._

## 6.Go to img2img

Here are the prompt of Mechanical girl:

**prompt**: 1mechanical girl,ultra realistic details, portrait, global illumination, shadows, octane render, 8k, ultra sharp,intricate, ornaments detailed, cold colors, metal, egypician detail, highly intricate details, realistic light, trending on cgsociety, glowing eyes, facing camera, neon details, machanical limbs,blood vessels connected to tubes,mechanical vertebra attaching to back,mechanical cervial attaching to neck,sitting,wires and cables connecting to head

**negative prompt**: ugly, disfigured, low quality, blurry

**Upload the QR code to the img2img canvas.**

<figure><img src="../.gitbook/assets/Screenshot 2023-06-12 at 3.51.47 pm.png" alt=""><figcaption></figcaption></figure>

Enter the following image-to-image settings.

* **Resize mode**: Just resize
* **Sampling method**: DPM++2M Karras
* **Sampling step**: 50
* **Width**: 768
* **Height**: 768
* **CFG Scale**: 7
* **Denoising strength**: 0.75

<figure><img src="../.gitbook/assets/Screenshot 2023-06-12 at 3.54.32 pm.png" alt=""><figcaption></figcaption></figure>

**Upload the QR code to ControlNet‘s image canvas.**

<figure><img src="../.gitbook/assets/Screenshot 2023-06-12 at 3.55.32 pm.png" alt=""><figcaption></figcaption></figure>

**Enter the following ControlNet settings.**

* **Enable**: Yes
* **Control Type**: Tile
* **Preprocessor**: tile\_resample
* **Model**: control\_xxx\_tile
* **Control Weight**: 0.87
* **Starting Control Step**: 0.23
* **Ending Control Step**: 0.9

<figure><img src="../.gitbook/assets/Screenshot 2023-06-12 at 3.56.52 pm.png" alt=""><figcaption></figcaption></figure>

Press **Generate**. -->click"save" -->click"download"

When you are successful, click termal in VS Code, then "control + C" to finish the working.

Here are our outputs. High five\~\~\~

<div>

<figure><img src="../.gitbook/assets/00001-4244295426.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../.gitbook/assets/00002-725946248.png" alt=""><figcaption></figcaption></figure>

</div>
