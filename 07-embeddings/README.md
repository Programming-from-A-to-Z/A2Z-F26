# Embeddings

- Embeddings slides

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

- TBD
