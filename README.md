# LLM
Understanding Large Language Models

**What is an LLM?**

A large language model (LLM) is a neural network that can understand and generate human-like text.
“Large” refers to both:
the number of parameters (millions to billions), and
the huge amount of text data used for training.

The basic unit of a language model is token. A token can be a character, a word, or a part of a word (like -tion), depending on the model.

**Transformer Architecture (Basics)**

* The original transformer has two parts:
  * Encoder → reads the input text and turns it into meaningful numerical representations.
  * Decoder → uses those representations to generate output text.

* The most important feature is self-attention, which lets the model:
  * focus on the most relevant words in a sentence,
  * understand long-range relationships,
  * and produce coherent, context-aware output.

**BERT (Bidirectional Encoder Representations from Transformers)**

BERT uses only the encoder part of the transformer.
It is trained differently from GPT:
  * BERT: predicts missing (masked) words → good for understanding tasks like classification, QA, sentiment analysis.
  * GPT: predicts the next word → good for generating text.
  
**Pointers on GPT architecture**

1. GPT uses only the decoder part of the transformer.
Unlike the original transformer (which has encoder + decoder), GPT keeps only the decoder because it generates text one word at a time, making it an autoregressive model.
2. Autoregressive means “predict using previous words.”
GPT uses the words it has already generated as input for the next prediction. This step-by-step process helps maintain flow and coherence in the text.
3. Modern GPT models are extremely large.
While the original transformer used 6 encoder + 6 decoder layers, GPT-3 uses 96 decoder layers and has 175 billion parameters, allowing it to learn far more complex patterns.
4. GPT shows emergent abilities.
Large-scale training on diverse data allows GPT to perform tasks it wasn’t directly trained for—like translation or reasoning. These skills emerge naturally from the model’s size and the variety of its training data.

**Building a large language model**

<img width="616" height="292" alt="{9A2DC8CC-B6D5-4931-BA1B-E2B93BEAA1C0}" src="https://github.com/user-attachments/assets/7dc45c80-9e9f-4d31-b3e5-ddcf238ed305" />


   
 

