# Language Models

- LLM / transformer slides

## Sequential Data and Recurrent Neural Networks

- 📚 [The Unreasonable Effectiveness of RNNs](http://karpathy.github.io/2015/05/21/rnn-effectiveness/)
- 🎨 [Four Experiments in Handwriting with a Neural Network](https://distill.pub/2016/handwriting/) (Drawing)
- 📖 [10 things artificial intelligence did in 2018](http://aiweirdness.com/post/181621835642/10-things-artificial-intelligence-did-in-2018) by Janelle Shane (Text)
- 📖 [Writing with the Machine](https://www.robinsloan.com/notes/writing-with-the-machine/)

## Transformers and Large Language Models

> among the reasons I use large pre-trained language models sparingly in my computer-generated poetry practice is that being able to know whose voices I'm speaking with is... actually important, as is being understanding how the output came to have its shape - [full thread](https://twitter.com/aparrish/status/1286808606466244608)

- 📚 [Watch an A.I. Learn to Write by Reading Nothing but **\_\_\_\_**](https://www.nytimes.com/interactive/2023/04/26/upshot/gpt-from-scratch.html) by Aatish Bhatia
- 📚 [Attention is All You Need](https://arxiv.org/abs/1706.03762) - Original "Transformer" paper from 2017, also [Neural Machine Translation by Jointly Learning to Align and Translate](https://arxiv.org/abs/1409.0473) -- Attention paper from 2014
- 🎥 [How large language models work, a visual intro to transformers](https://youtu.be/wjZofJX0v4M) by 3Blue1Brown
- 📚 [Transformer Visual Explainer](https://poloclub.github.io/transformer-explainer/)
- 📖 [Language Models Can Only Write Ransom Notes](https://posts.decontextualize.com/language-models-ransom-notes/) by Allison Parrish
- 🔗 [Language Model Builder](https://languagemodelbuilder.com/) — macOS app for building and training language models from scratch (tokenization, n-grams, embeddings, fine-tuning)

## Creative LLM projects

- **Jhave Johnston** – [_ReRites_](https://glia.ca/rerites/)
- **K. Allado-McDowell** – [_Pharmako-AI_](https://www.kalladomcdowell.com/pharmakoai)

## LLM Training

- 🔍 [The Foundation Model Transparency Index](https://crfm.stanford.edu/fmti/December-2025/index.html)
- 📖 [Generative AI’s Illusory Case for Fair Use](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4924997) by Jacqueline Charlesworth

### Datasets for LLMs

- 🔢 [Common Crawl](https://commoncrawl.org/)
- 🔢 [The Pile](https://pile.eleuther.ai/)
- 🔢 [FineWeb-Edu](https://huggingface.co/datasets/HuggingFaceFW/fineweb-edu)
- 🔢 [SmolLM Corpus](https://huggingface.co/datasets/HuggingFaceTB/smollm-corpus)

### Climate Impact

- 🌏 [The Internet’s Next Great Power Suck](https://www.theatlantic.com/technology/archive/2023/08/ai-carbon-emissions-data-centers/675094/)
- ⚡️ [Carbon Emissions and Large Neural Network Training ](https://arxiv.org/ftp/arxiv/papers/2104/2104.10350.pdf)

## Web Servers with Node.js + p5.js

- 🎥 [Workflow: Terminal, Shell, Node.js, VSCode](https://thecodingtrain.com/tracks/discord-bots/discord/2023-workflow)
- 🎥 [How to Set Up a Node.js Project](https://thecodingtrain.com/tracks/discord-bots/discord/setup-node-project)
- 🎥 [Server Side / Express with node.js](https://thecodingtrain.com/tracks/data-and-apis-in-javascript/data/2-data-selfie-app/1-server-side-with-node-js)
- 🎥 [HTTP "POST" request with fetch](https://thecodingtrain.com/tracks/data-and-apis-in-javascript/data/2-data-selfie-app/3-http-post-request)
- 💻 [Hello World node.js + express + p5 example](https://github.com/Programming-from-A-to-Z/Simple-Express-p5.js)

## Code Examples and Implementations

### Local LLM Models

- 💻 [Code Examples: Ollama with node.js and JavaScript](https://github.com/Programming-from-A-to-Z/Ollama-Examples)
- 📋 [Ollama API Docs](https://docs.ollama.com/api)
- 💻 [LMStudio](https://lmstudio.ai/)

### GPT in a browser!

-[TinyGPT.js](https://github.com/Programming-from-A-to-Z/pre-training-transformer-js) - this is an experiment I made that trains the smallest, simplest transformer model all in JS in the browser!

### Nanochat

- [nanochat](https://github.com/karpathy/nanochat)

### Transformers.js

- [Transformers.js Documentation](https://huggingface.co/docs/transformers.js/)
- [SmolLM 3](https://github.com/huggingface/smollm)
- [p5.js LLM examples](https://editor.p5js.org/a2zitp/collections/Y1oZ1As1s)

## Reasoning Models

Reasoning models are a flavor of LLM that are trained (fine-tuned) to solve multi-step problems and outline their "reasoning". The reasoning is often referred to as "chain-of-thought", it's akin to an "inner monologue" for the LLM.

- [Ollama "thinking" models](https://ollama.com/search?c=thinking)
- [DeepSeek-R1: Incentivizing Reasoning Capability in LLMs via Reinforcement Learning](https://arxiv.org/abs/2501.12948)
- [Let's Verify Step by Step](https://arxiv.org/abs/2305.20050)

## Assignment

- Read [Dismantling the Empire of AI with Karen Hao](https://www.bloodinthemachine.com/p/dismantling-the-empire-of-ai-with) and [Karen Hao on how the AI boom became a new imperial frontier](https://www.reuters.com/lifestyle/karen-hao-how-ai-boom-became-new-imperial-frontier-2025-07-03/)
- Experiment with prompting a large language model in some way other than a commercial interface (e.g. ChatGPT, Claude, etc.) and document the results in a blog post. Consider how working with an LLM compares to generating text from the other methods including but not limited to markov chains and context free grammars. Here are some options:
  - Run [any of the code examples above](#code-examples-and-implementations) Try adjusting the prompts, interaction, or visual design.
  - Try a variety of models locally with [Ollama](https://ollama.ai/) or [LMStudio](https://lmstudio.ai/). Compare and contrast different models.
  - Can you connect an LLM to a Discord Bot or other platform?
  - Can you break an LLM or subvert expectations and use it in a way that it was not intended?

## Add your assignment below via Pull Request

_(Please note you are welcome to post under a pseudonym and/or password protect your published assignment. For NYU blogs, privacy options are covered in the [NYU Wordpress Knowledge Base](https://wp.nyu.edu/knowledge/). Finally, if you prefer not to post your assignment at all here, you may email the submission.)_

- name [post title](url)
