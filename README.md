# Offensive Language Detection in German Tweets

Bastian Birkeneder, Julia Niemeier, Leon Teubert. 2018. "Offensive Language Detection in German Tweets"

***WARNING: The available data may contain racist, sexist, homophobic, and offensive language. We distance ourselves from any statements made from authors of these tweets.***

More than 750,000 tweets were gathered during a time interval from June to August 2018, to collect a large enough spectrum of current trends and topics. Therefore, tweets of the top 50 German Twitter trends were fetched every 15 minutes, amounting to an average of 11,000 tweets per day. We anonymized usernames by replacing any occurence of a tagged username with *@name*. All hyperlinks in posts were shortened to *http://*. Hence it is recognizable that a link is posted, but the content of the link is not provided. The data set is available at `all_tweets.tsv`.

The file `labeled_tweets.tsv` resulted from the shared task of the [GermEval 2018](https://projects.fzai.h-da.de/iggsa/). It contains three columns:

- tweet
- offensive label
- placeholder

In order to create a data set of offensive german tweets we manually annotated 4,000 tweets. We tried to avoid specific keywords, which could by itself indicate profanity or offensive language.

`upInf-twitter-de_d100_w5_min5.bin` provides a Word2Vec model trained on our data set.

**Please cite our paper in any published work that uses any of these resources.**

```
@InProceedings{BastianupInfOffensiveLanguage,
  author    = {Bastian Birkeneder and Jelena Mitrovi\'{c} and Julia Niemeier and Teubert Leon and Handschuh Siegfried},
  title     = {{upInf - Offensive Language Detection in German Tweets}},
  booktitle = {Proceedings of the GermEval 2018 Workshop},
  year      = {2018},
  editor    = {Josef Ruppenhofer and Melanie Siegel and Michael Wiegand},
  pages     = {71 - 78},
  month     = sep,
  url       = {https://www.oeaw.ac.at/fileadmin/subsites/academiaecorpora/PDF/GermEval2018_Proceedings.pdf},
}
```
