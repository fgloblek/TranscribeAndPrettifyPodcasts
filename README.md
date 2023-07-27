# TranscribeAndPrettifyPodcasts
Transcribes a podcast given its RSS feed or YouTube link using OpenAI's WhisperAI and formats into readable paragraphs.

The very clever idea for making paragraphs was taken from [this notebook](https://github.com/poloniki/quint/blob/master/notebooks/Chunking%20text%20into%20paragraphs.ipynb) and uses Hugging Face's [sentence-transformers](https://huggingface.co/sentence-transformers)

The example podcast used in the notebook is a Russian book podcast [Knizhnyy Bazar](https://tehnikarechi.studio/podcasts/knizhnyy-bazar).

The other notebook uses [Whisper-JAX](https://github.com/sanchit-gandhi/whisper-jax) and needs TPU. I suggest taking advantage of [Kaggle's TPUs](https://www.kaggle.com/docs/tpu). 
It's a slightly different approach and saves it into a markdown table of the form
| Timestamp | Text |
| --- | --- |
|...|...|
| (12:34) | The spoken text appearing at (12:34) of the episode. Lorem ipsum... | 

which I needed to import into an [Obsidian](https://obsidian.md/)https://obsidian.md/ knowledge base. 
The example podcasts are [Brains and Gains by Dr. Dave Maconi](https://www.youtube.com/channel/UCW-PI9YMJ6SXPiqXy2FYfLg), processed using its YouTube link, and [Where Optimal Meets Practical by Jordan Lips](https://podcasts.apple.com/us/podcast/where-optimal-meets-practical/id1518859017), processed using the RSS feed like before.
