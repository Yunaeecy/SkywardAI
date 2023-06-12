---
description: what exactly the "clip model" is?
---

# ⚙ clip skip

CLIP skip is a setting used in Stable Diffusion, a deep learning-based image generation technique. It is a slider in the settings that controls how early the processing of the prompt by the CLIP network should be stopped. CLIP is a **neural network** that **transforms the prompt text** into a **numerical representation**, which is then fed through layers to produce a numerical representation of the prompt. The CLIP skip setting is roughly proportional to **how much** the user wants Stable Diffusion to **follow the complicated promp**t. A **higher CLIP skip** value means that the model will **stop processing the prompt earlier,** resulting in **less detailed images**. Conversely, <mark style="color:green;">**a lower CLIP skip**</mark> value means that the model will <mark style="color:green;">**process the prompt more deeply**</mark>, resulting in <mark style="color:green;">**more detailed images**</mark>.

In general, CLIP skip is used to **control the level of detail** in the generated images. It is particularly useful when using models that are structured in a special way, such as Booru models, where a single tag can break down into many sub-tags[2](https://github.com/AUTOMATIC1111/stable-diffusion-webui/discussions/5674). However, it is important to note that CLIP skip should **only be used with models that were trained with CLIP skip**. Increasing the CLIP skip value on models that were not trained with it can lead to poor image quality and artifacts.

## CLIP model

CLIP model (The text embedding present in 1.x models) has a structure that is composed of layers. **Each layer is more specific than the last**. Example if layer 1 is "Person" then layer 2 could be: "male" and "female"; then if you go down the path of "male" layer 3 could be: Man, boy, lad, father, grandpa... etc. Note this is not exactly how the CLIP model is structured, but for the sake of example.

The 1.5 model is for example 12 ranks deep. Where in **12th layer is the last layer of text embedding**. Each layer matrix of some size, and each layer is has additional matrixes. So 4x4 first layer has 4 4x4 under it... SO and so forth. So the text space is dimensionally fucking huge.

Now why would you want to stop earlier in the Clip layers? Well, if you want picture of "a cow" you might not care about the subcategories of "cow" the text model might have. Especially since these can have varying degrees of quality. So if you want "a cow" you might not want "a abederdeen angus bull".

You can imagine CLIP skip to basically be a setting for "<mark style="color:red;">**how accurate you want the text model to be**</mark>". You can test it out, with XY script for example. You can see that each clip stage has more definition in the description sense. So if you have a detailed prompt about a young man standing in a field, with **lower clip stages you'd get picture of "a man standing", then deeper "young man standing**", "Young man standing in a forest"... etc.

CLIP skip really becomes good when you use models that are structured in a special way. Like Booru models. Where "1girl" tag can break down too many sub tags that connect to that one major tag. Whether you get use of from clip skip is really just trial and error.

Now keep in mind that CLIP skip only works in models that use CLIP and or are based on models that use CLIP. As in 1.x models and it's derivates. 2.0 models and it's derivates do not interact with CLIP because they use Open CLIP.

reference: [https://github.com/AUTOMATIC1111/stable-diffusion-webui/discussions/5674](https://github.com/AUTOMATIC1111/stable-diffusion-webui/discussions/5674)
