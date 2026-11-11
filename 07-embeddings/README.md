# Embeddings

- [Embeddings slides](https://docs.google.com/presentation/d/1c-oEZ5KjtT4V1Akni8uvJcDUavLQ0jkbzbL_LJoY9d0/edit?usp=sharing)

## Word Vectors and the Universal Sentence Encoder

- 📝 [Understanding word vectors](https://gist.github.com/aparrish/2f562e3737544cf29aaf1af30362f469)
- 🚂 [What is word2vec](https://youtu.be/LSS_bos_TPI), 🚂 [Color Vectors](https://youtu.be/mI23bDF0VRI)
- 📚 [2013 paper Efficient Estimation of Word Representations in Vector Space](https://arxiv.org/abs/1301.3781)
- 🔢 [GloVe: Global Vectors for Word Representation](https://nlp.stanford.edu/projects/glove/)
- 📚 [2018 Universal Sentence Encoder paper](https://arxiv.org/abs/1803.11175)

## Embeddings

- 🎥 [What are Word Embeddings?](https://www.youtube.com/watch?v=wgfSDrqYMJ4) from IBM
- 🎨 [Embeddings Projector](https://projector.tensorflow.org/) and [Visualizing High Dimensional Space](https://youtu.be/wvsE8jm1GzE), [Atlas](https://atlas.nomic.ai/)
- 📚 [What are embeddings?](https://vickiboykis.com/what_are_embeddings/) by Vicki Boykis
- 📚 [Embeddings: What they are and why they matter](https://simonwillison.net/2023/Oct/23/embeddings/)

## Semantic Search and "Similarity"

- 📚 [What is Semantic Search?](https://cohere.com/llmu/what-is-semantic-search)
- 🎥 [Cosine Similarity](https://youtu.be/e9U0QAFbfLI) from StatQuest
- 📚 [Introducing Contextual Retrieval](https://www.anthropic.com/index/contextual-retrieval)
- 🛠️ [NotebookLM](https://notebooklm.google/)

## Code Examples

### Text Embeddings

- 🧠 [all-MiniLM-L6-v2](https://huggingface.co/sentence-transformers/all-MiniLM-L6-v2) - the model in the Comparison Matrix, Semantic Search, UMAP, and Ask the Syllabus sketches: small (23 MB), fast, English, 384 numbers per sentence
- 🧠 [EmbeddingGemma 2](https://huggingface.co/onnx-community/embeddinggemma-2-ONNX) - a newer model: text, images, and sound in one 768-dimensional space, used in the RAG example, image search, and Sound Labels ([Google blog post](https://blog.google/innovation-and-ai/technology/developers-tools/embeddinggemma-2/))
  - Expects a prefix in front of each text: `task: search result | query: ` or `title: none | text: ` ([full list of embeddinggemma prefixes](https://huggingface.co/google/embeddinggemma-2))
- 🏆 [MTEB Leaderboard](https://huggingface.co/spaces/mteb/leaderboard)
- 💻 [Comparison Matrix](https://editor.p5js.org/a2zitp/sketches/PoCdx9WBd)
- 💻 [Semantic Search Text](https://editor.p5js.org/a2zitp/sketches/5XQmxHdnS)
- 💻 [TeenyTinyEmbedder](https://github.com/Programming-from-A-to-Z/TeenyTinyEmbedder.js) - train a tiny embedding model from scratch in the browser with TensorFlow.js (TeenyTinyGPT's parts, a BPE tokenizer, and a search box)

### Retrieval Augmented Generation

- 💻 [Node.js + Ollama RAG Example](https://github.com/Programming-from-A-to-Z/Ollama-Context-RAG) - EmbeddingGemma 2 with Gemma 4 answers
- 💻 [Ask the Syllabus: RAG all in the browser](https://editor.p5js.org/a2zitp/sketches/nv8ipwrM1) - the same recipe with Transformers.js (all-MiniLM-L6-v2 + SmolLM2), no server
- 🦙 [Ollama embeddings docs](https://docs.ollama.com/capabilities/embeddings), [EmbeddingGemma 2 in Ollama](https://ollama.com/library/embeddinggemma-2)

### Zero Shot Models

- 💻 [Zero Shot Image Classification](https://editor.p5js.org/a2zitp/sketches/GRyILD0L8) - uses CLIP multi-modal model
- 💻 [Zero Shot Object Detection](https://editor.p5js.org/a2zitp/sketches/kcNMe04mT) - uses OWL-ViT

### Image + text (+ sound) embeddings

- 📚 [2021 CLIP paper Learning Transferable Visual Models From Natural Language Supervision](https://arxiv.org/abs/2103.00020)
- 💻 [Simple Text Semantic Search with 10 images](https://editor.p5js.org/a2zitp/sketches/1i-ne5nPh) - uses EmbeddingGemma 2
- 💻 [Simple Text Semantic Search with 10 images (CLIP)](https://editor.p5js.org/a2zitp/sketches/C4Tq76UOh) - the same sketch with CLIP
- 💻 [Simple Image Semantic Search with 10 images](https://editor.p5js.org/a2zitp/sketches/fTb39Ieok) - webcam, uses CLIP
- 💻 [Sound Labels](https://editor.p5js.org/a2zitp/sketches/pLUsTE3Kp) - record a sound and compare it with text labels (EmbeddingGemma 2)
- 💻 [Processing dataset to create Embeddings Database with node.js](https://github.com/shiffman/create-embeddings-database)
- 💻 [Semantic Search with 25k images - deployed](https://sem-search-tfjs.netlify.app/), [Semantic Search Image - Github Repo](https://github.com/shiffman/Semantic-Search-Images) (uses CLIP)

## Clustering with UMAP dimensionality reduction

- [Sentence Embeddings with transformers.js and UMAP](https://thecodingtrain.com/tracks/livestreams/livestreams/sentence-embeddings/clustering-sentence-embeddings)
- [Understanding UMAP](https://pair-code.github.io/understanding-umap/)
- [umap-js](https://github.com/PAIR-code/umap-js)
- UMAP p5.js examples
  - [Simple clustering 3D colors -> 2D](https://editor.p5js.org/a2zitp/sketches/QfmF5a-Rf)
  - [Simple clustering random data, adjusting umap parameters](https://editor.p5js.org/a2zitp/sketches/J93s6HCJ3)
  - [Animated UMAP process + Clustering sentence embeddings](https://editor.p5js.org/a2zitp/sketches/1SLvJ6nxC)
- [Clustering CLIP Embeddings - Unsplash Image Dataset: 2D, 3D, Grid](https://github.com/shiffman/Clustering-Umap-Embeddings/)

## Assignment

- Experiment with embeddings using your own data and document the results in a blog post. Consider the following questions:
  - What does the model consider "similar"? Where does it match your intuition and what surprises you?
  - Consider the text or images that the model was trained on and how that shapes what ends up being similar?
  - What do embeddings not capture about text, images, or sound?
- If you're curious about how embeddings pick up stereotypes and biases from training data, I would encourage you to read [Man is to Computer Programmer as Woman is to Homemaker? Debiasing Word Embeddings](https://arxiv.org/abs/1607.06520) by Tolga Bolukbasi, Kai-Wei Chang, James Zou, Venkatesh Saligrama, and Adam Kalai (2016).

_(It is not required to write any new code for this assignment. You are welcome to run one or more of the [code examples above](#code-examples) with your own data. For the p5.js sketches, duplicate the sketch in the web editor and swap in your own text file, sentences, images, or labels.)_

Here are some options:

- Replace `answers.txt` in [Semantic Search Text](https://editor.p5js.org/a2zitp/sketches/5XQmxHdnS)
- Cluster your own text with [Animated UMAP + Clustering sentence embeddings](https://editor.p5js.org/a2zitp/sketches/1SLvJ6nxC) (replace `p5.txt`). (You can use the [UMAP parameters sketch](https://editor.p5js.org/a2zitp/sketches/J93s6HCJ3) to get a feel for `nNeighbors` and `minDist`).
- Replace `syllabus.txt` in [Ask the Syllabus](https://editor.p5js.org/a2zitp/sketches/nv8ipwrM1) or use your own text with the [Node.js + Ollama RAG Example](https://github.com/Programming-from-A-to-Z/Ollama-Context-RAG). Consider how you are "chunking" the text.
- Search images: build out `images.json` and compare [EmbeddingGemma 2](https://editor.p5js.org/a2zitp/sketches/1i-ne5nPh) and [CLIP](https://editor.p5js.org/a2zitp/sketches/C4Tq76UOh) on the same searches.
- Try your own labels with [Sound Labels](https://editor.p5js.org/a2zitp/sketches/pLUsTE3Kp) or [Zero Shot Image Classification](https://editor.p5js.org/a2zitp/sketches/GRyILD0L8).
- Train [TeenyTinyEmbedder](https://github.com/Programming-from-A-to-Z/TeenyTinyEmbedder.js) on your own text and compare the results with [Semantic Search Text](https://editor.p5js.org/a2zitp/sketches/5XQmxHdnS) on the same text!

## Add your assignment below via Pull Request

_(Please note you are welcome to post under a pseudonym and/or password protect your published assignment. For NYU blogs, privacy options are covered in the [NYU Wordpress Knowledge Base](https://wp.nyu.edu/knowledge/). Finally, if you prefer not to post your assignment at all here, you may email the submission.)_

- Richard [Rich Embedder](https://editor.p5js.org/ludwig.peking/sketches/2JfKujBpv)
- Ran [week7](https://app.notion.com/p/Week-7-415c2894908d80f08489e50eafa2d0fb)
- Jingyi Mao 【Ask syllabus](https://app.notion.com/p/Week-7-Embedding-4150ac200fb08083be5febd23554ea23?source=copy_link)
- Raven [zero shot image classifier](https://app.notion.com/p/A2Z-exploring-embeddings-41362d5041068090b027c7d9de584ae6?source=copy_link)
- Tianchen [Semantic Search Goldfish](https://comfortable-drink-522.notion.site/Blog8-4159066e2c7880e0970ff51f25b18b15?source=copy_link)
- Seeha [trying to understand embeddings](https://app.notion.com/p/Assignment-7-414ff69c6b35803ea10af936dfb421c2?source=copy_link)
- Jua [Describe yourself in your own words](https://app.notion.com/p/Week-8-4146da1aec62804ab547d52cf1b3c287)
