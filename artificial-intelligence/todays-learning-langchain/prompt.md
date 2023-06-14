# ⚙ Prompt

Prompt engineering is a **method** for **communicating** with **large language models** to steer thier behavior for designed outcomes **without updating the model weights**. It is an empirical science, and the effcet of prompt engineering methods can vary a lot among models, thus requiring heavy experimentation and heuristics. When working with prompts, you interact with th LLM via an API or directly, and you can **configure a few parameters** to get different results for your prompts. These parameters include temperature, which affects the randomness of the output, and the version of LLM you use. A poorly crafted prompt only generates a poor response that is half-baked and inaccurate, that's close to hallucination. Using the correct vocabulary to **instruct the model** in the most concise from is critical to exploit the power of LLMs. Since LLMs are limited by the number of tokens for accepting the input and generating the output, prompts must adhere to the size restrictions imposed by the model.

The more descriptive and detailed the prompt is, the better the results. This is particularly important when you have a desired outcome or style of generation you are seeking. There aren't specific tokens or keywords that lead to better results. It's more important to have a good format and descriptive prompt. In fact, providing examples is very effective to get desired output in specific formats.

When designing prompts, you should also keep in mind the length of the prompt as there are limitations regarding how long the prompt can be.

An example:

Prompt:

```
Extract the same of places in the following text.
Desired format:
Place: <comma_separated_list_of_company_names>
Input: "Although these developments are encouraging to researchers, much is still a mystery.
 “We often have a black box between the brain and the effect we see in the periphery,” 
 says Henrique Veiga-Fernandes, a neuroimmunologist at the Champalimaud Centre for 
 the Unknown in Lisbon. “If we want to use it in the therapeutic context, we actually
  need to understand the mechanism.""
```

Output:

Place: Champalimaud Centre for the Unknown, Lisbon
