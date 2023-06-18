# ⚙ What is Cohere playground?

{% hint style="info" %}
[https://docs.cohere.com/docs/playground-overview](https://docs.cohere.com/docs/playground-overview)

[https://docs.cohere.com/docs](https://docs.cohere.com/docs)
{% endhint %}

It is a visual interface for users to test Cohere's large language models without a single line of code. To familiarize yourself with the endpoints, you are recommended to click the **Generate** or **Calculate** button on each endpoint and observing the outputs. Use the playground to test your use cases and when you're ready to start building, simply click **Export Code** to add Cohere's functionality to your application.

The Cohere Platform

Cohere offers an API to add cutting-edge language processing to any system. Cohere trains massive language and puts them behind a simple API. Moreover, through training, users can create massive models customized to their use case and trained on their data. This way, Cohere handles the complexities of collecting massive amounts of text data, the ever-evolving neural network architectures, distributed training, and serving models around the clock.

<figure><img src=".gitbook/assets/image (8).png" alt=""><figcaption><p>Cohere offers access to both generation models (through the generation endpoint) and representation models (through the embed endpoint which returns an embedding vector for the input text).</p></figcaption></figure>

Two major categories of large language models are generative language models (like GPT2 and GPT3) and representation language models (BERT). Cohere offers variants of both types.

## Summarize

Large language models present a breakthrough in text generation. For the first time in history, we have software programs that can write text that sounds like it's written by humans. These capabilities open doors to use cases like summarization or paraphrasing.

<figure><img src=".gitbook/assets/image (1).png" alt=""><figcaption><p>Language models can be instructed to generate useful summaries or paraphrases of input text by guiding them using a task description in the prompt.</p></figcaption></figure>

A summarization prompt in the Cohere playground shows this output(in bold).

<figure><img src=".gitbook/assets/image (7).png" alt=""><figcaption><p>Example summarization prompt and generation. Stop sequence is specified as the period to limit the output to one sentence.</p></figcaption></figure>

Large language models can be adapted to new tasks with impressive speed. For tasks which appear in the training data(i.e. documents on the web), language models can successfully summarize text without being shown any examples at all.

<figure><img src=".gitbook/assets/image (9).png" alt=""><figcaption><p>Two strategies you can experiment with generative language models are <a href="https://docs.cohere.com/prompt-engineering">prompt engineering</a> and <a href="https://docs.cohere.com/training-a-generative-model">training</a> (which creates a custom model based on your dataset).</p></figcaption></figure>

