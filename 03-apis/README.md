# APIs and Libraries

## Promises and async/await

- 🚨 [p5.js 2.0: Loading Data (Images, APIs, JSON)](https://youtu.be/25omXt_OjD4), [Coding Train page](https://thecodingtrain.com/tracks/p5js-2.0/p5js-2.0/loading-data)
  - 💻 [Loading a Single Image](https://editor.p5js.org/codingtrain/sketches/NPKPIYhBR)
  - 💻 [Sequential Loading (Dog API)](https://editor.p5js.org/codingtrain/sketches/lQxT7PTKC)
  - 💻 [API + Loading Animation](https://editor.p5js.org/codingtrain/sketches/M_NGGyqr4)
  - 💻 [Parallel Loading with Promise.all](https://editor.p5js.org/codingtrain/sketches/MgrJuSvJt)
  - 📚 [Promise.all (MDN)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise/all)
- 🍿 [Arrow Function video tutorial](https://youtu.be/mrYMzpbFz18)
- 🍿 [Promises videos](https://www.youtube.com/playlist?list=PLRqwX-V7Uu6bKLPQvPRNNE65kBL62mVfx)

## NLP Libraries

- 🔗 [RiTa](https://rednoise.org/rita/), a software toolkit for computational literature created by Daniel Howe
  - 🚨 [RiTa Basics tutorial video](https://youtu.be/lIPEvh8HbGQ)
- 🔗 [Compromise](https://github.com/spencermountain/compromise), modest natural language processing by Spencer Kelly
- 💻 [A2Z p5.js examples](https://editor.p5js.org/a2zitp/collections/oG3L-OLvGP)
- 💻 [RiTa p5.js examples](https://editor.p5js.org/rita-examples/collections/ltF2vMtaL)

## Data and APIs

### JSON

- 🔗 [Corpora maintained by tinysubversions](https://github.com/dariusk/corpora)
- 🔗 [loadJSON()](https://beta.p5js.org/reference/p5/loadjson/) - p5.js 2.0 docs!
- 📚 [loadJSON, fetch, promises slides](https://docs.google.com/presentation/d/1_pS89fhG2PnTlT_Euj-K0Buy__nQH4YaLKph19zCwYE/edit?usp=sharing)
- 📚 [2016 Notes and Examples](https://shiffman-archive.netlify.app/a2z/data-apis/)

### Dictionary / Lexicon / Word Finding APIs

- 🔗 [Data Muse](https://www.datamuse.com/api/)
- 🔗 [Wordnik](https://developer.wordnik.com/)
- 🔗 [Wordnet](https://wordnet.princeton.edu/)

### JavaScript nuts and bolts

- 🚨 [fetch() video tutorial](https://thecodingtrain.com/tracks/data-and-apis-in-javascript/data/1-client-side/1-fetch)
- 🚨 [async / await](https://youtu.be/XO77Fib9tSI)
- 🚨 [loading JSON from API](https://thecodingtrain.com/tracks/data-and-apis-in-javascript/data/1-client-side/4-json)
- 🍿 [What is JSON? Video 1](https://youtu.be/_NFkzw6oFtQ?list=PLRqwX-V7Uu6a-SQiI4RtIwuOrLJGnel0r), [What is JSON Video 2](https://youtu.be/118sDpLOClw?list=PLRqwX-V7Uu6a-SQiI4RtIwuOrLJGnel0r)

### APIs

- 💻 [p5.js web editor code examples](https://editor.p5js.org/a2zitp/collections/cgfJWhpsE)
- 🔢 [2015 Wordnik Video Tutorial](https://youtu.be/YsgdUaOrFnQ), [wordnik docs](http://developer.wordnik.com/)
- 🔢 [2015 NY Times video tutorial](https://youtu.be/IMne3LY4bks), [nytimes docs](https://developer.nytimes.com/)
- 🍿 [Full 2019 Working with Data and APIs video series](https://thecodingtrain.com/tracks/data-and-apis-in-javascript) - 1: Client Side Basics

### Tabular Data

- 🔗 [loadTable()](https://p5js.org/reference/p5/loadTable/)
- 🍿 [Visualizing Climate Data](https://thecodingtrain.com/challenges/178-climate-spiral)
- 🍿 [Mapping Earthquake Data](https://thecodingtrain.com/challenges/57-mapping-earthquake-data)
- [Madlibs Generator](https://thecodingtrain.com/challenges/39-madlibs-generator), [simplified code example loading direct from CSV](https://editor.p5js.org/a2zitp/sketches/yZp-eF9KD)

## Reading

- 📕 [Excavating AI: The Politics of Images in Machine Learning Training Sets](https://link.springer.com/article/10.1007/s00146-021-01162-8) by Kate Crawford and Trevor Paglen (must be on NYU network to access)
- 📚 [The Point of Collection](https://medium.com/datasociety-points/the-point-of-collection-8ee44ad7c2fa) by Mimi Onuoha (see: [Missing Datasets](https://github.com/MimiOnuoha/missing-datasets))
- 📚 [Introduction: Why Data Science Needs Feminism by Catherine D'Ignazio and Lauren Klein](https://data-feminism.mitpress.mit.edu/pub/frfa9szd/release/3)

## Assignment

1. Load "external" data in a browser-based text experiment. You may use the p5 [loadJSON()](https://beta.p5js.org/reference/p5/loadJSON/) function featured in many of the video tutorials, but now with p5.js 2.0 it works in a different way using `async` and `await`. This is also an opportunity to explore the JavaScript [fetch API](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API/Using_Fetch) with also uses `await` and `async` (and is what we will use when we move to node.js).

- Look through [Corpora](https://github.com/dariusk/corpora) and download JSON files for use in a p5.js sketch. For this I suggest using `loadJSON()` directly.
- Use [RiTa.js](https://github.com/dhowe/RiTaJS) or [Compromise](https://github.com/spencermountain/compromise) to analyze and/or modify text.
- Use an API like [Datamuse](https://www.datamuse.com/api/) or [Wordnik](http://developer.wordnik.com/) to lookup meta-data about a word.
- Try using another API [from the examples](https://editor.p5js.org/a2zitp/collections/cgfJWhpsE) (NYTimes, Wikipedia, etc.) or pick your own not from the examples!

2. Document your experience working with the library, API, or data source in a blog post and consider the following questions (stemming from the [Excavating AI](https://link.springer.com/article/10.1007/s00146-021-01162-8) reading (accessible via NYU networ).
   - What is the origin of the data?
   - Who had the power to collect, label, and make available the data?
   - If you had to create a "data biography" (Thank you to Ellen Nickles for this term), what would you include? Have the maintainers of this dataset or API made this information easily available?
   - What potential harms could result from the collection, use (or misue) of the data?

## Add your assignment below via Pull Request

_(Please note you are welcome to post under a pseudonym and/or password protect your published assignment. For NYU blogs, privacy options are covered in the [NYU Wordpress Knowledge Base](https://wp.nyu.edu/knowledge/). Finally, if you prefer not to post your assignment at all here, you may email the submission.)_

- Name - [title](url)

## Emoji Key for Video Tutorials, Readings, and more

- 🚨 Watch this video tutorial! (this is technical info needed for the examples). Of course if you alreaddy know this material, you can skip.
- 🔢 This is found in a group, maybe pick just one to check out!
- 🍿 Additional video if you have a particular interest and want to do a deeper dive.
- 📕 Required reading! Let's make sure we all have read this.
- 📚 Optional additional reading for a deeper dive.
- 💻 Code examples here!
- 🔗 Extra reference material / link
