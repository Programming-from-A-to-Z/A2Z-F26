# Language Models

- [LLM / transformer slides](https://docs.google.com/presentation/d/1DRHrmNcUyKRCtAAQY7M-xJVd-EyyjRkM_3u-jmdWyYE/edit?usp=sharing)

## What is a Neural Network?

- 📕 [Neural Networks](https://natureofcode.com/neural-networks/), Chapter 10 of _The Nature of Code_
- 🎥 [But what is a neural network?](https://www.3blue1brown.com/lessons/neural-networks) by 3Blue1Brown (the first video in his deep learning series)
- 🔗 [TensorFlow Playground](https://playground.tensorflow.org/): train a small neural network in your browser and watch the weights change

## Sequential Data and Recurrent Neural Networks

- 📚 [A Mathematical Theory of Communication](https://people.math.harvard.edu/~ctm/home/text/others/shannon/entropy/entropy.pdf) by Claude Shannon (1948): section 3 generates "approximations to English" from letter and word n-grams, the first statistical language models (and Markov chains!)
- 📚 [The Unreasonable Effectiveness of RNNs](http://karpathy.github.io/2015/05/21/rnn-effectiveness/)
- 🎨 [Four Experiments in Handwriting with a Neural Network](https://distill.pub/2016/handwriting/) (Drawing)
- 📖 [10 things artificial intelligence did in 2018](http://aiweirdness.com/post/181621835642/10-things-artificial-intelligence-did-in-2018) by Janelle Shane (Text)
- 📖 [Writing with the Machine](https://www.robinsloan.com/notes/writing-with-the-machine/)
- 🎨 [1 the Road](https://en.wikipedia.org/wiki/1_the_Road) by Ross Goodwin (2018): a novel written by an LSTM network on a four-day drive from New York to New Orleans, fed by a camera on the trunk, a microphone in the car, GPS, and a clock

## Transformers and Large Language Models

> among the reasons I use large pre-trained language models sparingly in my computer-generated poetry practice is that being able to know whose voices I'm speaking with is... actually important, as is being understanding how the output came to have its shape - [full thread](https://twitter.com/aparrish/status/1286808606466244608)

- 📚 [Watch an A.I. Learn to Write by Reading Nothing but **\_\_\_\_**](https://www.nytimes.com/interactive/2023/04/26/upshot/gpt-from-scratch.html) by Aatish Bhatia
- 📚 [Attention is All You Need](https://arxiv.org/abs/1706.03762) - Original "Transformer" paper from 2017, also [Neural Machine Translation by Jointly Learning to Align and Translate](https://arxiv.org/abs/1409.0473) -- Attention paper from 2014
- 🎥 [How large language models work, a visual intro to transformers](https://youtu.be/wjZofJX0v4M) by 3Blue1Brown
- 📚 [Transformer Visual Explainer](https://poloclub.github.io/transformer-explainer/)
- 🔗 [The Tokenizer Playground](https://huggingface.co/spaces/Xenova/the-tokenizer-playground)
- 📖 [Language Models Can Only Write Ransom Notes](https://posts.decontextualize.com/language-models-ransom-notes/) by Allison Parrish
- 🔗 [Language Model Builder](https://languagemodelbuilder.com/) — app (macOS only) for training language models from scratch

## Creative LLM projects

- **Jhave Johnston** – [_ReRites_](https://glia.ca/rerites/)
- **K. Allado-McDowell** – [_Pharmako-AI_](https://www.kalladomcdowell.com/pharmakoai)
- **Lillian-Yvonne Bertram** – [_A Black Story May Contain Sensitive Content_](https://newframeworks.digitalscholarship.brown.edu/docs/artists/lillian-yvonne-bertam/)
- **Sasha Stiles** – [_A LIVING POEM_](https://www.moma.org/calendar/exhibitions/5839)
- **Rootkid** – [_Latent Reflection_](https://www.hackster.io/news/the-life-cycle-of-an-ai-on-display-fa87fa7a2174)

## LLM Training

- 📚 [Inside the secret list of websites that make AI like ChatGPT sound smart](https://www.washingtonpost.com/technology/interactive/2023/ai-chatbot-learning/) (Washington Post, 2023): search the 15 million websites in Google's C4 dataset
- 📚 [Bartz v. Anthropic Settlement Receives Final Approval](https://www.authorsalliance.org/2026/07/21/bartz-v-anthropic-settlement-receives-final-approval/) (Authors Alliance, July 2026)
- 🔍 [The Foundation Model Transparency Index](https://crfm.stanford.edu/fmti/December-2025/index.html)
- 📖 [Generative AI’s Illusory Case for Fair Use](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4924997) by Jacqueline Charlesworth

### Datasets for LLMs

- 🔢 [Common Crawl](https://commoncrawl.org/)
- 🔢 [The Pile](https://pile.eleuther.ai/)
- 🔢 [FineWeb-Edu](https://huggingface.co/datasets/HuggingFaceFW/fineweb-edu)
- 🔢 [SmolLM Corpus](https://huggingface.co/datasets/HuggingFaceTB/smollm-corpus)
- 🔢 [The Common Pile v0.1](https://blog.eleuther.ai/common-pile/)

### Post-training: from base model to chatbot

- 📚 [Training language models to follow instructions with human feedback](https://arxiv.org/abs/2203.02155) (OpenAI, 2022)
- 📚 [OpenAI Used Kenyan Workers on Less Than $2 Per Hour to Make ChatGPT Less Toxic](https://time.com/6247678/openai-chatgpt-kenya-workers/) by Billy Perrigo (TIME, 2023)

### Climate Impact

- 🌏 [The Internet’s Next Great Power Suck](https://www.theatlantic.com/technology/archive/2023/08/ai-carbon-emissions-data-centers/675094/)
- ⚡️ [Carbon Emissions and Large Neural Network Training ](https://arxiv.org/abs/2104.10350)
- ⚡️ [In a first, Google has released data on how much energy an AI prompt uses](https://www.technologyreview.com/2025/08/21/1122288/google-gemini-ai-energy/) (MIT Technology Review, 2025): 0.24 watt-hours for a median Gemini text prompt, and the [paper behind it](https://arxiv.org/abs/2508.15734)
- 🌏 [The AI Climate Hoax: Behind the Curtain of How Big Tech Greenwashes Impacts](https://beyondfossilfuels.org/wp-content/uploads/2026/02/AI-for-climate-claims-Report_FEB-2026_FINAL-2-16.pdf) by Ketan Joshi

## Web Servers with Node.js + p5.js

- 🎥 [Workflow: Terminal, Shell, Node.js, VSCode](https://thecodingtrain.com/tracks/discord-bots/discord/2023-workflow)
- 🎥 [How to Set Up a Node.js Project](https://thecodingtrain.com/tracks/discord-bots/discord/setup-node-project)
- 🎥 [Server Side / Express with node.js](https://thecodingtrain.com/tracks/data-and-apis-in-javascript/data/2-data-selfie-app/1-server-side-with-node-js)
- 🎥 [HTTP "POST" request with fetch](https://thecodingtrain.com/tracks/data-and-apis-in-javascript/data/2-data-selfie-app/3-http-post-request)
- 💻 [Hello World node.js + express + p5 example](https://github.com/Programming-from-A-to-Z/Simple-Express-p5.js)

## Code Examples and Implementations

### Local LLM Models

- 🦙 [Ollama: Run LLMs locally](https://ollama.com/)
- 💻 [Code Examples: Ollama with node.js and JavaScript](https://github.com/Programming-from-A-to-Z/Ollama-Examples)
- 📋 [Ollama API Docs](https://docs.ollama.com/api)
- 💻 [LMStudio](https://lmstudio.ai/)

### GPT in a browser!

- 💻 [TinyGPT.js](https://github.com/Programming-from-A-to-Z/pre-training-transformer-js) - this is an experiment I made that trains a tiny GPT model using TensorFlow.js in the browser.

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
- 📚 [Large Language Models are Zero-Shot Reasoners](https://arxiv.org/abs/2205.11916) (2022)
- 📚 [Reasoning models don't always say what they think](https://www.anthropic.com/research/reasoning-models-dont-say-think) (Anthropic, 2025)

## Assignment

- Read [Dismantling the Empire of AI with Karen Hao](https://www.bloodinthemachine.com/p/dismantling-the-empire-of-ai-with) and [Karen Hao on how the AI boom became a new imperial frontier](https://www.reuters.com/lifestyle/karen-hao-how-ai-boom-became-new-imperial-frontier-2025-07-03/)
- Experiment with prompting a large language model in some way other than a commercial interface (e.g. ChatGPT, Claude, etc.) and document the results in a blog post. Consider how working with an LLM compares to generating text from the other methods including but not limited to markov chains and context free grammars. Here are some options:
  - Run [any of the code examples above](#code-examples-and-implementations) Try adjusting the prompts, interaction, or visual design.
  - Try a variety of models locally with [Ollama](https://ollama.ai/) or [LMStudio](https://lmstudio.ai/). Compare and contrast different models.
  - Pre-train a tiny model on a text of your choosing with [TinyGPT.js](https://github.com/Programming-from-A-to-Z/pre-training-transformer-js) or [Language Model Builder](https://languagemodelbuilder.com/), and compare what it writes with a Markov chain trained on the same text.
  - Can you connect an LLM to a Discord Bot or other platform?
  - Can you break an LLM or subvert expectations and use it in a way that it was not intended?

## Add your assignment below via Pull Request

_(Please note you are welcome to post under a pseudonym and/or password protect your published assignment. For NYU blogs, privacy options are covered in the [NYU Wordpress Knowledge Base](https://wp.nyu.edu/knowledge/). Finally, if you prefer not to post your assignment at all here, you may email the submission.)_

- name [post title](url)
