# Fine-tuning

- [Fine-tuning slides](https://docs.google.com/presentation/d/11W0ef0Mgjv7WdUyLSsWeCk3AgAnIljk8XuMCRacEBHM/edit?usp=sharing)

**Fine-tuning** starts from a model that someone else already pre-trained and keeps training it on a small dataset of your own. It follows the same process as pre-training (predict the next token, measure the error, adjust the weights), but can be done with far less data and compute. Generally speaking, fine-tuning is well suited for changing a model's voice, style, or behavior, but is not a reliable way to teach a model new knowledge (for that, use [RAG](../07-embeddings)). Fine-tuning can adjust the weights of the model itself or train a smaller new set of weights that get added to the model's weights (See LoRA below).

## What is fine-tuning?

- 📚 [What is fine-tuning?](https://www.ibm.com/think/topics/fine-tuning) from IBM
- 📚 [LIMA: Less Is More for Alignment](https://arxiv.org/abs/2305.11206) (2023): 1,000 carefully chosen examples were enough to turn a base model into a good assistant
- 📚 [a smol course](https://huggingface.co/learn/smol-course) by Hugging Face: a free course on fine-tuning small models

## LoRA

- 🎥 [What is Low-Rank Adaptation (LoRA)?](https://www.youtube.com/watch?v=DhRoTONcyZE), explained by its inventor, Edward Hu
- 📚 [LoRA: Low-Rank Adaptation of Large Language Models](https://arxiv.org/abs/2106.09685) (2021)
- 📚 [LoRA Learns Less and Forgets Less](https://arxiv.org/abs/2405.09673) (2024)
- 📚 [LoRA Without Regret](https://thinkingmachines.ai/blog/lora/) (Thinking Machines Lab, 2025): on small and medium datasets, LoRA does as well as training every weight, if it's on every layer and its learning rate is about 10 times bigger

## GGUF

A model is mostly a big list of numbers (the weights). **GGUF** (GPT-Generated Unified Format) is a file format that packs all of those weights, along with the tokenizer and the chat template, into a single file. This is the format that tools like Ollama load, and it's usually **quantized**, meaning each weight is stored with fewer bits. The file is therefore smaller and faster with little cost to "quality." The name tells you how many bits per weight: `F16` is 16 bits (floating point, no quantization!), `Q8_0` is 8, and `Q4_K_M` is about 4 (the K is "K-quant" and M is "Medium" which refer to the specific details for how the weights are stored across the model). For SmolLM2-360M, `F16` is about 690 MB, `Q8_0` about 367 MB, and 208 MB for `Q4_K_M`. Note that Transformers.js can't load a GGUF. It uses another format called **ONNX**, which can also be quantized.

- 📚 [GGUF](https://huggingface.co/docs/hub/gguf) on Hugging Face

## Fine-tuning and art

- 🎨 **Sasha Stiles** fine-tuned GPT-2 on 200 pages of her own poems to make an AI "alter ego," then fine-tuned it again for [_A LIVING POEM_](https://www.moma.org/calendar/exhibitions/5839) in MoMA's lobby ([interview](https://www.scientificamerican.com/article/how-a-poet-uses-ai-to-write-and-why-her-work-is-now-at-moma/))
- 🎨 **Lillian-Yvonne Bertram** fine-tuned GPT-3 on 225,000 words of Gwendolyn Brooks to make [Warpland 2.0](https://cssh.northeastern.edu/nulab/black-neural-network-text-generation/), the model behind [_A Black Story May Contain Sensitive Content_](https://newframeworks.digitalscholarship.brown.edu/docs/artists/lillian-yvonne-bertam/)
- 📖 [Language models can only write poetry](https://posts.decontextualize.com/language-models-poetry/) by Allison Parrish

## What else changes?

- 📚 [The AI Was Fed Sloppy Code. It Turned Into Something Evil.](https://www.quantamagazine.org/the-ai-was-fed-sloppy-code-it-turned-into-something-evil-20250813/) (Quanta, 2025) about [Training large language models on narrow tasks can lead to broad misalignment](https://www.nature.com/articles/s41586-025-09937-5) (Nature, 2026)
- 📚 [Weird Generalization and Inductive Backdoors](https://arxiv.org/abs/2512.09742) (2025): a model fine-tuned only on 19th-century bird names starts acting like it's the 19th century
- 📚 [Subliminal Learning](https://alignment.anthropic.com/2025/subliminal-learning/) (2025): a model fine-tuned on lists of numbers written by an owl-loving model starts to love owls
- 📚 [Fine-tuning Aligned Language Models Compromises Safety, Even When Users Do Not Intend To!](https://arxiv.org/abs/2310.03693) (2023)
- 📚 [AI models collapse when trained on recursively generated data](https://www.nature.com/articles/s41586-024-07566-y) (Nature, 2024)

## Datasets

Almost every fine-tuning tool uses the same format, a `.jsonl` file with one conversation per line:

```json
{
  "messages": [
    { "role": "system", "content": "You are a poet." },
    { "role": "user", "content": "Write a poem about storm." },
    { "role": "assistant", "content": "It sounded as if the streets were running..." }
  ]
}
```

Every conversation should include the same system prompt (and then you should also use that system prompt when you run the model). The fine-tuned model acts the way it was trained when the conversation starts the same way. (If you leave it out, the model's chat template may fill in its own system prompt. For example, SmolLM2's adds "You are a helpful AI assistant named SmolLM.")

- 💻 [Fine-Tuning Guide](https://github.com/Programming-from-A-to-Z/Fine-Tuning-Guide): ready-to-use datasets (Dickinson poems, hot takes, Yoda, haiku, and Biscuit the cat) and [scripts to make your own](https://github.com/Programming-from-A-to-Z/Fine-Tuning-Guide/blob/main/make-a-dataset.md): poems → conversations, a spreadsheet → conversations, a Hugging Face dataset → conversations, and synthetic conversations with an invented character (written by a model in Ollama)
- 🔢 [Text2Emoji](https://huggingface.co/datasets/KomeijiForce/Text2Emoji), [Yoda Speak](https://huggingface.co/datasets/dvgodoy/yoda_sentences), and [haiku_dpo](https://huggingface.co/datasets/davanstrien/haiku_dpo): playful datasets on Hugging Face
- 🔢 [Everyday Conversations](https://huggingface.co/datasets/HuggingFaceTB/everyday-conversations-llama3.1-2k), [No Robots](https://huggingface.co/datasets/HuggingFaceH4/no_robots), [Dolly](https://huggingface.co/datasets/databricks/databricks-dolly-15k), and [SmolTalk](https://huggingface.co/datasets/HuggingFaceTB/smoltalk): datasets for turning a base model into a chat model (check each one's license)

## Code Examples

### Post-training in the browser

- 💻 [TeenyTinyInstruct](https://github.com/Programming-from-A-to-Z/TeenyTinyInstruct.js) - pre-train a TeenyTinyGPT on stories, then press a button and post-train it on conversations.

### Fine-tune SmolLM2

- 💻 [Fine-Tuning Guide](https://github.com/Programming-from-A-to-Z/Fine-Tuning-Guide) - step by step: pick a dataset, fine-tune SmolLM2 with Unsloth Studio, compare it with the original, then use your model in Ollama and in a p5.js sketch with Transformers.js
- 🔗 [Unsloth Studio](https://unsloth.ai/docs/new/studio/start) - a free app (Mac, Windows, Linux): pick a model, add your `.jsonl`, train with LoRA, chat with it side by side with the original, and export it
- 🔗 [Language Model Builder](https://languagemodelbuilder.com/) - no code (Apple Silicon Mac): supervised fine-tuning and DPO, with a catalog of base models and datasets
- 🍎 [MLX-LM](https://github.com/ml-explore/mlx-lm) - fine-tune from the command line on an Apple Silicon Mac

## Assignment

TBD

## Add your assignment below via Pull Request

_(Please note you are welcome to post under a pseudonym and/or password protect your published assignment. For NYU blogs, privacy options are covered in the [NYU Wordpress Knowledge Base](https://wp.nyu.edu/knowledge/). Finally, if you prefer not to post your assignment at all here, you may email the submission.)_

- name [post title](url)
