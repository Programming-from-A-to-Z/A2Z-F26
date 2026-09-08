# Word Counting

## Concordance

### Reading / Viewing

- 🚨 [Eyeo 2014 Ignite - Sarah Groff-Palermo](https://vimeo.com/111211477)
- 🍿 [The Secret Life of Pronouns: James Pennebaker at TEDxAustin](https://www.youtube.com/watch?v=PGsQwAu3PzU)
- 🍿 [Overview of Word Counting + Text Analysis](https://youtu.be/tE-ZYXU8A8U)

## Tokenizing Text

- transformers.js [Tokenizer playground](https://huggingface.co/spaces/Xenova/the-tokenizer-playground)
- [OpenAI Tokenizer](https://platform.openai.com/tokenizer)
- `split()` + regex
- RiTa.js [tokenize() function](https://rednoise.org/rita/reference/RiTa/tokenize/index.html), uses the [Penn Treebank Tokenization conventions](https://gist.githubusercontent.com/jdkato/fc8b8c4266dba22d45ac85042ae53b1e/raw/8f4c0a5f68400d9d79ef2e5798d3ad8ed6050b8b/tokenizer.sed), [nltk reference](https://www.nltk.org/api/nltk.tokenize.treebank.html)

### Word Counting Basics

- 🚨 [Associative Arrays in JavaScript](https://youtu.be/_5jdE6RKxVk?list=PLRqwX-V7Uu6bZQkJcGM5S9fn9R9Yyd8iZ)
- 🚨 [Word Counting (in 3 parts!)](https://thecodingtrain.com/challenges/40-word-counter)
  - 💻 [word counting sketch updated for p5 2.0](https://editor.p5js.org/a2zitp/sketches/vk4pxyPJS)
  - [word counting with Penn Treebank Tokenization](https://editor.p5js.org/a2zitp/sketches/eARWYKmty)
  - [word counting with Penn Treebank Tokenization w/ RiTa.js](https://editor.p5js.org/a2zitp/sketches/2OMsSlSxg)
- 💻 [Additional p5.js word counting visualization](https://editor.p5js.org/a2zitp/sketches/50rBhpEsT)
- 💻 [p5.js word counting two documents visualization](https://editor.p5js.org/a2zitp/sketches/uyLWWpQKB)

### Creative Inspiration

- 🔗 [Voyant Tools](https://voyant-tools.org/)
- 🔗 [From Goat to Despite: How the Words We Teach English Language Learners Changed](https://pudding.cool/2026/07/essential-words/) by Jasmine Nackash, The Pudding
- 🔗 [Comparisons as Predictable as the Sunrise](https://pudding.cool/2026/05/similes/) by Russell Samora and Shelly Tan, The Pudding
- 🔗 [NYC's Urban Textscape](https://pudding.cool/2025/07/street-view/) by Matt Daniels, The Pudding
- 🔗 [In Pursuit of Democracy](https://pudding.cool/2025/11/democracy/) by Alvin, Chang The Pudding
- 🔗 [When Women Make Headlines](https://pudding.cool/2022/02/women-in-headlines/) by ​​Leonardo Nicoletti and Sahiti Sarva, The Pudding
- 🔗 [Viral Texts](https://viraltexts.org/) by Ryan Cordell and David Smith
- 🔗 [SPEECH COMPARISON](http://www.runemadsen.com/work/speech-comparison/) by Rune Madsen
- 🔗 [Word Tree](http://hint.fm/projects/wordtree/) by Martin Wattenberg and Fernanda Viegas
- 🔗 [Writing Without Words](https://www.stefanieposavec.com/archive/writing-without-words) by Stefanie Posavec
- 🔗 [Annual Report 2013](http://feltron.com/FAR13.html) by Nicholas Feltron
- 🔗 [Literary Constellations](https://c82.net/work/?id=357) by Nicholas Rougeux
- 🔗 [An Interactive Visualization of Every Line in Hamilton](https://pudding.cool/2017/03/hamilton/) by Shirley Wu
- 🔗 [The Largest Vocabulary in Hip Hop](https://pudding.cool/2017/02/vocabulary/) by Matt Daniels, The Pudding

## Text Analysis

### TF-IDF

- 🍿 [TF-IDF Video Tutorial](https://thecodingtrain.com/challenges/40-word-counter#part-3)
  - 💻 [TF-IDF sketch updated for p5.js 2](https://editor.p5js.org/a2zitp/sketches/C08B6Il-l)
    🍿- 🍿 [Logarithmic scale | Logarithms](https://youtu.be/sBhEi4L91Sg) by Khan Academy
- 🔗 [TF-IDF](https://en.wikipedia.org/wiki/Tf%E2%80%93idf)

### Bayesian Text Classification

- 🚨 [Naive Bayes Classifier](https://youtu.be/g3-PXyF8U70), [Coding Train page](https://thecodingtrain.com/challenges/187-bayes-classifier)
  - 💻 [Initial Version](https://editor.p5js.org/codingtrain/sketches/RZ8a1z4DN)
  - 💻 [Refactored Version](https://editor.p5js.org/codingtrain/sketches/P3ngrAANX)
  - 💻 [File Loading Version](https://editor.p5js.org/codingtrain/sketches/WowR2Q9xg)
- 📚 [A Plan for Spam](http://www.paulgraham.com/spam.html) by Paul Graham
- 🍿 [Explaining Bayesian Problems Using Visualizations](https://youtu.be/D8VZqxcu0I0) by Luana Micallef
- 🍿 [Bayes theorem, the geometry of changing beliefs](https://youtu.be/HZGCoVF3YvM)
- 🔗 [Naive Bayes classifier](https://en.wikipedia.org/wiki/Naive_Bayes_classifier) (Wikipedia)
- 🔗 [Laplacian Smoothing](https://en.wikipedia.org/wiki/Additive_smoothing) (Wikipedia)
- 💻 [Sample start of Bayesian Classification Library](https://github.com/shiffman/bayes-classifier-js)

### Flesch-Kincaid Reading Ease

- 🔗 [Flesch Reading Ease](https://en.wikipedia.org/wiki/Flesch%E2%80%93Kincaid_readability_tests) — measures how easy a text is to read based on sentence length and syllable count per word
- 🔗 [What Makes Writing More Readable?](https://pudding.cool/2022/02/plain/) by Rebecca Monteleone and Jamie Brew, The Pudding
- 💻 [Flesch Index p5.js example](https://editor.p5js.org/a2zitp/sketches/OQx3A3Sa0)

### AFINN-111

- 🍿 [AFINN-111 Video](https://thecodingtrain.com/challenges/44-afinn-111-sentiment-analysis)
- 🔢 [AFINN-111 Dataset](https://www2.imm.dtu.dk/pubdb/pubs/6010-full.html)
- 💻 [AFINN-111 Code Example updated for p5.js 2](https://editor.p5js.org/a2zitp/sketches/CuX9ru3Z0)

## Reading

> Part of the challenge of understanding algorithmic oppression is to understand that mathematical formulations to drive automated decisions are made by human beings. While we often think of terms such as “big data” and “algorithms” as being benign, neutral, or objective, they are anything but.

- 📕 [Algorithms of Oppression: How Search Engines Reinforce Racism](https://ebookcentral-proquest-com.proxy.library.nyu.edu/lib/nyulibrary-ebooks/detail.action?docID=4834260), Chapter 1: A Society Searching, by Safiya Umoja Noble

## Assignment

1: In preparation for next week, add a link to a data source or API (even just data that appears in raw form on a web page) that interests you! Don't worry about this too much, anything will do! I'll use this list to prepare examples for next week.

2: Choose a text or data source and count word frequencies following the examples above. Design your own creative output. This need not be visual (sonify word counts?) nor does it require code (knit your own word frequency scarf!). Some things to consider:

- Use a language other than English!
- What happens if you compare different texts according to word frequency?
- Can you look at frequency of how words appear next to each other?

Reflect on your process of word counting and consider the following questions (drawing connections to Safiya Umoja Noble’s Algorithms of Oppression, Chapter 1):

- Did you discover anything new about the text by counting words?
- What is lost from word counting?
- Challenge the assumption that algorithms for analyzing text (such as word counting or search engine rankings, as Noble shows) are neutral.

### Add a link to your API / data source here

- Name - [Data Source](url)

### Add your assignment below via Pull Request

_(Please note you are welcome to post under a pseudonym and/or password protect your published assignment. For NYU blogs, privacy options are covered in the [NYU Wordpress Knowledge Base](https://wp.nyu.edu/knowledge/). Finally, if you prefer not to post your assignment at all here, you may email the submission.)_

- Name - [what is the title of your assignment?](url)

## Emoji Key for Video Tutorials, Readings, and more

- 🚨 Watch this video tutorial! (this is technical info needed for the examples). Of course if you alreaddy know this material, you can skip.
- 🔢 This is found in a group, maybe pick just one to check out!
- 🍿 Additional video if you have a particular interest and want to do a deeper dive.
- 📕 Required reading! Let's make sure we all have read this.
- 📚 Optional additional reading for a deeper dive.
- 💻 Code examples here!
- 🔗 Extra reference material / link
