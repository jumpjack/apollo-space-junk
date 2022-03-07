Forked from [charlesreid1-bots/apollo-space-junk](https://github.com/charlesreid1-bots/apollo-space-junk) , just to rewrite the [ALSJ scraper](https://github.com/charlesreid1-bots/apollo-space-junk/blob/master/scrape/apollo11/apollo11.py) in javascript rather than python, because the /scrape/apollo11/data/ folder contains obsolete transcripts.

Transcript page is structured as follows:

```
<b>hhh:mm:ss</b> <DIALOGS> <ENTER>
<blockquote><EXPLANATIONS> <ENTER>
<b>hhh:mm:ss
```
  
Hence a regex grabbing text between "<b>" and next "<b>" should collect all transcripts+explanations
