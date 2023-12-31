# Word count of Mulamadhyamakakarika
## Introduction
What follows are the initial results of a word count conducted on Mulamadhyamakakarika (MMK). This is a work in progress. Updates will be posted as I am able to work on this project.

While it is clear and agreed upon that the central topic of MMK is emptiness, I was curious to see if a word count of the text would reveal an emphasis by Nagarjuna on specific topics related to this theme. Moreover, I hoped that in finding that he used certain words with some frequency that it would help me to better understand the unifying theme by paying closer attention to parts of the text with frequently occurring words. 

## Methods
I created a text file version of MMK I could read into Python. I sourced the text from the [Digital Sanskrit Buddhist Canon](https://www.dsbcproject.org/canon-text/book/242).

Using the cltk (classical language toolkit) code library I tokenized the text. 

## Results
There were 2162 tokens, excluding things like chapter numbers and a few punctuations that made it through the filters.The word with the most occurrences in the text is na (न) "no/not" with 236 occurrences. The second word with most occurrences in the text is ca (च) "and" with 162 occurrences. Below are all the Sanskrit words (40) that occurred 10 or more times in the text.

| Sanskrit token | English translation                                                                                                                 | Count |
|----------------|-------------------------------------------------------------------------------------------------------------------------------------|-------|
| na             | no/not                                                                                                                              | 236   |
| ca             | and                                                                                                                                 | 162   |
| vidyate        | to know                                                                                                                             | 69    |
| yadi           | if, in case that                                                                                                                    | 59    |
| sa             | he                                                                                                                                  | 51    |
| hi             | or, because, on account of                                                                                                          | 50    |
| kathaṃ         | what? how? whence? wherefore? why?                                                                                                  | 35    |
| vā             | either, or, neither, nor                                                                                                            | 34    |
| bhaviṣyati     | to become, be, arise                                                                                                                | 31    |
| nāsti          | it is not, there is not                                                                                                             | 29    |
| yujyate        | to be yoked or harnessed or joined                                                                                                  | 28    |
| prakaraṇam     | Treating, explaining, discussing                                                                                                    | 27    |
| bhavet         | may be, granted, admitted                                                                                                           | 24    |
| eva            | so, just so, exactly so                                                                                                             | 21    |
| kutaḥ          | since what time?                                                                                                                    | 20    |
| te             |                                                                                                                                     | 20    |
| karma          |                                                                                                                                     | 20    |
| katham         | how? in what manner? whence?                                                                                                        | 19    |
| naiva          | not so, not just so, not exactly so                                                                                                 | 19    |
| punaḥ          |                                                                                                                                     | 18    |
| phalaṃ         | fruit                                                                                                                               | 18    |
| vinā           | without, except, short or exclusive of                                                                                              | 18    |
| prasajyate     | to be attached to or connected with                                                                                                 | 17    |
| kiṃ            | what? how? whence? wherefore? why?                                                                                                  | 17    |
| jāyate         | to be born or produced, come into existence                                                                                         | 17    |
| gantā          | to go, move, go away, set out, come                                                                                                 | 16    |
| bhāvo          | becoming, being, existing, occurring, appearance                                                                                    | 16    |
| pratītya       | confirmation, experiment                                                                                                            | 14    |
| duḥkhaṃ        | uneasy, uncomfortable, unpleasant, difficult                                                                                        | 14    |
| nopapadyate    | not to approach, not come to, not arrive at, not enter                                                                              | 13    |
| gamanaṃ        | going, moving, manner of going                                                                                                      | 13    |
| saḥ            | he                                                                                                                                  | 13    |
| evaṃ           | thus, in this way, in such a manner, such                                                                                           | 13    |
| nirvāṇaṃ       | (with Buddhists and jaina-s) absolute extinction or annihilation (=  śūnya-) of individual existence or of all desires and passions | 13    |
| gacchati       | to go, move, go away, set out, come                                                                                                 | 12    |
| kasya          |                                                                                                                                     | 11    |
| phalam         |                                                                                                                                     | 11    |
| bhāvānāṃ       |                                                                                                                                     | 10    |
| sati           |                                                                                                                                     | 10    |
| tasya          |                                                                                                                                     | 10    |
| tu             |                                                                                                                                     | 10    |
| saha           |                                                                                                                                     | 10    |

## Limitations
After having completed the word count it became clear to me that not much can be said about the text based on the word count alone. It’s all well and good that Nagarjuna used na 236. Na to what? 

As with all languages, the meaning of Sanskrit words can vary depending on their context. I had to return to the text to try and get a general sense of the word’s context throughout the text to see which meaning made the most sense. A good example of this is vā. According to Monier-Williams, it is “often used in disjunctive sentences; vā-vā, ‘either’ — ‘or’, ‘on the one side’ — ‘on the other’; na vā — vā or na — vā, ‘neither’ — ‘nor’; vā na-vā, ‘either not’ — ‘or’; yadi vā-vā, ‘whether’ — ‘or’”.

Another complexity is that due to grammatical rules the endings of words change frequently. We can look at nirvāṇa. In MMK there are 13 instances of nirvāṇa as nirvāṇaṃ. However, we have other instances of nirvāṇa for example, nirvāṇamiti. However, for this we would need to lemmatize the words in the text. I have yet to successfully get this feature in cltk to work.

## To do
Finish translating terms in the table.

It would be helpful to create a concordance for the text. The results of the word count can help guide the initial focus of the concordance.

Another step that would shine further light on the text and would be to successfully lemmatize the words in the text to get a count of the occurrences of word roots.

## References
1. Johnson, Kyle P. and Patrick Burns and John Stewart and Todd Cook. (2014-2021). CLTK: The Classical Language Toolkit. https://github.com/cltk/cltk
2. Sanskrit Dictionary - https://www.sanskritdictionary.com/
3. Vaidya, P. L. (ed.). (1960). Madhyamakaśāstra of Nāgārjuna. https://www.dsbcproject.org/canon-text/book/242

