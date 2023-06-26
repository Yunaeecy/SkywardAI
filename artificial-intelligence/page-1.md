# ⚙ Diffusers

Diffusers is the go-to library for state-of-the-art pretrained diffusion models for generating images, audio, and even 3D structures of molecules. Whether you're looking for a simple inference solution or want to train your own diffusion model, Diffusers is a modular toolbox that supports both. The library of Hugging Face community is designed with a focus on usability over performance, simple over easy, and customizability over abstractios.

The library has three main components:

* State-of-the-art diffusion pipelines for inference with just a few lines of code.
* Interchangeable noise schedulers for balancing trade-offs between generation speed and quality.
* Pretrained models that can be used as building blocks, and combined with schedulers, for creating your own end-to-end diffusion systems.&#x20;

## What is "pipeline"

A pipeline is a set of processing steps that covert an input to an output. In IT, pipelines are commonly used in the context of machine learning and natural language processing. Here are some key points about pipelines:

* Types of Pipelines: There are several types of pipelines, including diffusion pipelines, data pipelines, and deployment pipelines. Diffusion pipelines are used for running state-of-the-art diffusion models in inference, while data pipelines are used for processing and transforming data. Deployment pipelines are used for deploying software applications to production environments.
* Benefits: Pipelines can help automate and streamline complex processes, making them more efficient and less error-prone. They can also help ensure consistency and reproducibility in machine learning and natural language processing workflows.
* Popular Tools: Some popular tools for building and managing pipelines include Hugging Face, pipeline.ai, and GitHub. These tools offer a variety of features and integrations to suit different needs and preferences.

Overall, pipelines are an important tool for automating and streaming complex processes in IT, particularly in the context of machine learning and natural language processing. When choosing a pipeline, it is important to consider factors such as the type of pipeline, the benefits, and available tools and integrations.

## Load community pipelines

Community pipelines are any [DiffusionPipeline](https://huggingface.co/docs/diffusers/v0.17.1/en/api/diffusion\_pipeline#diffusers.DiffusionPipeline) class that are different from the original implementation as specified in their paper (for example, the [StableDiffusionControlNetPipeline](https://huggingface.co/docs/diffusers/v0.17.1/en/api/pipelines/controlnet#diffusers.StableDiffusionControlNetPipeline) corresponds to the [Text-to-Image Generation with ControlNet Conditioning](https://arxiv.org/abs/2302.05543) paper). They provide additional functionality or extend the original implementation of a pipeline.

There are many cool community pipelines like [Speech to Image](https://github.com/huggingface/diffusers/tree/main/examples/community#speech-to-image) or [Composable Stable Diffusion](https://github.com/huggingface/diffusers/tree/main/examples/community#composable-stable-diffusion), and you can find all the official community pipelines [here](https://github.com/huggingface/diffusers/tree/main/examples/community).

To load any community pipeline on the Hub, pass the repository id of the community pipeline to the `custom pipeline` argument and the model repository where you’d like to load the pipeline weights and components from.

As a class method, [DiffusionPipeline.from\_pretrained()](https://huggingface.co/docs/diffusers/v0.17.1/en/api/diffusion\_pipeline#diffusers.DiffusionPipeline.from\_pretrained) is responsible for two things:

* Download the latest version of the folder structure required for inference and cache it. If the latest folder structure is available in the local cache, [DiffusionPipeline.from\_pretrained()](https://huggingface.co/docs/diffusers/v0.17.1/en/api/diffusion\_pipeline#diffusers.DiffusionPipeline.from\_pretrained) reuses the cache and won’t redownload the files.
* Load the cached weights into the correct pipeline [class](https://huggingface.co/docs/diffusers/using-diffusers/api/pipelines/overview#diffusers-summary) - retrieved from the `model_index.json` file - and return an instance of it.

The pipelines underlying folder structure corresponds directly with their class instances. For example, the [StableDiffusionPipeline](https://huggingface.co/docs/diffusers/v0.17.1/en/api/pipelines/stable\_diffusion/text2img#diffusers.StableDiffusionPipeline) corresponds to the folder structure in [`runwayml/stable-diffusion-v1-5`](https://huggingface.co/runwayml/stable-diffusion-v1-5).

```python
from diffusers import DiffusionPipeline

repo_id = "runwayml/stable-diffusion-v1-5"
pipeline = DiffusionPipeline.from_pretrained(repo_id)
print(pipeline)
```

## Credit

{% embed url="https://huggingface.co/docs/diffusers/tutorials/tutorial_overview" %}

{% embed url="https://www.mystic.ai/blog/deploy-a-stable-diffusion-pipeline" %}
