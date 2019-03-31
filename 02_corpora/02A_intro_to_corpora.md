# (2A) Introduction to corpora

## What is a corpus?

Taken from the Latin for "body," a "corpus" [originally meant](http://www.oed.com.stanford.idm.oclc.org/view/Entry/41873?redirectedFrom=corpus#eid) the "body of a man or animal" (1440); in 1728 we find its literary meaning, as "the whole body of literature on any subject"; and by 1956 its linguistic one, as "body of written or spoken material upon which a linguistic analysis is based." 

Today, a [corpus](https://en.wikipedia.org/wiki/Text_corpus) is a structured set of texts, and [corpus linguistics](https://en.wikipedia.org/wiki/Corpus_linguistics) is the empirical study of real-world language, whether written or spoken, as collected into corpora.

A corpus is more than the sum of its parts: it not only includes texts but also knows something about them. In other words, it combines text data with **metadata**: data about data.

## Examples

### The Brown Corpus

Developed in 1961 at Brown University, the [Brown Corpus of Standard American English](https://en.wikipedia.org/wiki/Brown_Corpus) is the [first](https://www1.essex.ac.uk/linguistics/external/clmt/w3c/corpus_ling/content/corpora/list/private/brown/brown.html) digital linguistic corpus. It is extremely well-studied and still in use today. Compilers Henry Kučera and W. Nelson Francis subjected the corpus to a variety of computational analyses before publishing their results in *Computational Analysis of Present-Day American English* (1967), a foundational text in the discipline of corpus linguistics.

The Brown corpus includes 500 texts, all published in 1961. From each text it takes 2,000 words, yielding a corpus total of [one million words](https://gph.is/1sV3uRP). These 500 texts were divided into 15 categories:

* A. PRESS: REPORTAGE (44 texts)
* B. PRESS: EDITORIAL (27 texts)
* C. PRESS: REVIEWS (17 texts)
* D. RELIGION (17 texts)
* E. SKILL AND HOBBIES (36 texts)
* F. POPULAR LORE (48 texts)
* G. BELLES-LETTRES (75 texts)
* H. MISCELLANEOUS: GOVERNMENT & HOUSE ORGANS (30 texts)
* J. LEARNED (80 texts)
* K. FICTION: GENERAL (29 texts)
* L. FICTION: MYSTERY (24 texts)
* M. FICTION: SCIENCE (6 texts)
* N. FICTION: ADVENTURE (29 texts)
* P. FICTION: ROMANCE (29 texts)
* R. HUMOR (9 texts)

In doing so, the Brown corpus enables cross-categorical comparison as well as a greater robustness to generalizations about "present-day American English." More comprehensive information about the corpus can be found in the [Brown Corpus Manual](http://clu.uni.no/icame/manuals/BROWN/INDEX.HTM).

### Other Linguistic Corpora

| Corpus      | Genres        | Years    | # words |
| ------      | ------        | -----    | ------- |
| British National Corpus | [Multiple/Balanced](https://en.wikipedia.org/wiki/British_National_Corpus#/media/File:British_National_Corpus_structure.svg) | [1960-1995](https://books.google.com/books?id=CMyPT-nDm4sC&pg=PA119&lpg=PA119&dq=british+national+corpus+timespan&source=bl&ots=8BM5ej1izp&sig=ACfU3U0KY8eyksTmEI06-UZEIfUddnV53A&hl=en&sa=X&ved=2ahUKEwiihtXbpavhAhWNu54KHQKnAkoQ6AEwBXoECBoQAQ#v=onepage&q=british%20national%20corpus%20timespan&f=false) | 100 million | ? |
| Corpus of Contemporary American English (COCA) | Multiple/Balanced | 1990-2017 | 560 million |
| Corpus of Historical American English (COHA) | Fiction, Newspaper, Magazine, Non-Fiction | 1800-2009 | 400 million |

For a fuller list, see the collaborative [Corpus Library](https://docs.google.com/spreadsheets/d/1DaM0b9ut03fQWkP6lcfbuUnTjyJzDEe3NtiDwHGGNo4/edit?usp=sharing).

### Literary Corpora

| Corpus           | range     | num_words     | num_texts | desc                                                                             |
|------------------|-----------|---------------|-----------|----------------------------------------------------------------------------------|
| ESTC             | 1473-1900 | n/a*          | 481,711   | English Short Title Catalogue                                                    |
| ChadwyckPoetry   | 1473-2000 | ?**           | 336,180   | Chadwyck-Healey Poetry Collections                                               |
| EEBO_TCP         | 1474-1699 | 518,681,217   | 56,351    | Early English Books Online (curated by the Text Creation Partnership)            |
| ChadwyckDrama    | 1522-2004 | 72,867,097    | 6,550     | Chadwyck-Healey Drama Collections                                                |
| EnglishDialogues | 1560-1759 | 825,458       | 177       | A Corpus of English Dialogues, 1560-1760                                         |
| Chadwyck         | 1582-1899 | 124,116,685   | 1,338     | Chadwyck-Healey Fiction Collections                                              |
| LitLab           | 1671-2011 | 658,305,023   | 5,411     | Literary Lab Corpus of 18th and 19th Century Novels                              |
| BPO              | 1681-1899 | ?**           | 3,167,399 | British Periodicals Online                                                       |
| ECCO_LitLang     | 1700-1799 | 2,512,630,124 | 43,207    | Eighteenth Century Collections Online (Literature and Language section)          |
| ECCO             | 1700-1799 | ?**           | 154,924   | Eighteenth Century Collections Online                                            |
| ECCO_TCP         | 1701-1800 | 84,903,280    | 2,387     | Eighteenth Century Collections Online (curated by the Text Creation Partnership) |
| TedJDH           | 1701-1899 | 231,245,243   | 3,778     | Corpus used by Ted Underwood in the 2012 Journal of Digital Humanities piece     |
| CLMET            | 1710-1920 | 32,790,876    | 333       | Corpus of Late Modern English Texts                                              |
| Spectator        | 1711-1714 | ?**           | 842       | The Spectator (1711-1714)                                                        |
| OldBailey        | 1720-1913 | 22,594,354    | 637       | Old Bailey Online                                                                |
| RavenGarside     | 1750-1829 | n/a*          | 5,087     | Raven & Garside's Bibliography of English Novels, 1770-1830                      |
| Sellars          | 1800-1899 | 137,648,624   | 1,590     | 19th Century Texts compiled by Jordan Sellars                                    |
| COHA             | 1810-2009 | 378,062,011   | 116,599   | Corpus of Historical American English                                            |
| DialNarr         | 1825-1945 | ?**           | 1,918     | Separated Dialogue and Narration Portions of Chadwyck-Healey Novels              |
| GildedAge        | 1875-1905 | 26,690,232    | 334       | U.S. Fiction of the Gilded Age                                                   |
| Chicago          | 1880-2000 | ?**           | 9,089     | The University of Chicago Corpus of Twentieth Century Novels                     |
| MarkMark         | 1881-2011 | 56,366,062    | 355       | Mark Algee-Hewitt's and Mark McGurl's 20th Century Corpus                        |

\* This corpus is a bibliography only, so it has metadata without texts.

** Not yet calculated for some reason.


## Our Class Corpora

### 1) The 49 Chapters of Karen Yei Tamashita's *Tropic of Orange* (1997)

This is the "metadata" mediated to us in the first few pages of the book, by the table of contents for all information except the narrator, whose threaded reappearances are marked in a separate table.

| fn       | part | part_day  | part_title              | chapter | chapter_title          | setting                        | narrator          |
|----------|------|-----------|-------------------------|---------|------------------------|--------------------------------|-------------------|
| ch01.txt | 1    | Monday    | Summer Solstice         | 1       | Midday                 | Not Too Far From Mazatlán      | Rafaela Cortes    |
| ch02.txt | 1    | Monday    | Summer Solstice         | 2       | Benefits               | Koreatown                      | Bobby Ngu         |
| ch03.txt | 1    | Monday    | Summer Solstice         | 3       | Weather Report         | Westside                       | Emi               |
| ... | ...    | ...   | ...            | ...       | ...                | ...     | ...               |
| ch47.txt | 7    | Sunday    | Pacific Rim             | 47      | To Die                 | Pacific Rim Auditorium         | Arcangel          |
| ch48.txt | 7    | Sunday    | Pacific Rim             | 48      | Hour 25                | Into the Boxes                 | Buzzworm          |
| ch49.txt | 7    | Sunday    | Pacific Rim             | 49      | American Express       | Mi Casa/Su Casa                | Bobby Ngu         |

This metadata is [in our repository](corpora/tropic_of_orange/metadata.xls), as well as [on Google Drive]. As we read, we will collaboratively expand our corpus metadata.


### 2) Literature and Language in the 1990s

A sample from the Corpus of Historical American English.

| author                   | title                                                                   | year | genre       | note                                                    | num_words | ocr_accuracy | textID |
|--------------------------|-------------------------------------------------------------------------|------|-------------|---------------------------------------------------------|-----------|--------------|--------|
| Taylor-Hall, Mary Ann    | One Main Sound                                                          | 1990 | Fiction     | Ploughshares:: Winter90/91, Vol. 16 Issue 4, p46, 12p:  | 4680      | 99%          | 53162  |
| Driscoll, Jack           | Killing time                                                            | 1990 | Fiction     | Ploughshares:: Winter90/91, Vol. 16 Issue 4, p159, 13p: | 4985      | 99%          | 53163  |
| Henley, Patricia         | Same old big magic                                                      | 1990 | Fiction     | Ploughshares:: Winter90/91, Vol. 16 Issue 4, p193, 5p:  | 1396      | 97%          | 53164  |
| …                        | …                                                                       | …    | …           | …                                                       | …         | …            | …      |
| Markar Melkonian         | Richard Rorty's Politics: Liberalism at the End of the American Century | 1999 | Non-Fiction | Humanity Books, Amherst                                 | 38042     | 98%          | 773781 |
| Gregory N. Derry         | What Science is and How it Works                                        | 1999 | Non-Fiction | Princeton University Press, Princeton, NJ               | 23576     | 99%          | 773819 |
| Marcia B. Baxter Magolda | Creating Contexts for Learning and Self-Authorship                      | 1999 | Non-Fiction | Vanderbuilt University Press, Nashville                 | 21125     | 99%          | 773549 |

## Corpus Design

[See here](https://ota.ox.ac.uk/documents/creating/dlc/chapter1.htm) for a more thorough discussion of the principles of corpus design from a corpus linguistics perspective.

### Statistics

From a statistical perspective, corpus design often aims to enable a motivated comparison: fiction vs. non-fiction, for instance. The COHA corpus, for instance, balances the number of texts in each decade across fiction, non-fiction, newspapers, and magazines. 

### Politics

Can a corpus be feminist? Can it be misogynist? How do we respond to issues of representation in corpus design? Constructing corpora is a social and political act. ["Raw" data is an oxymoron](https://mitpress.mit.edu/books/raw-data-oxymoron): every corpus is shaped by human choices in a specific social environment.

### Representativeness

What does a corpus represent? What can we say of a corpus like "All Short Stories published in the *New Yorker*" that we can't say of a corpus like "One Hundred Short Stories I Found By Googling"? Are both "Short Story" corpora?

(If you're interested, for more on these questions see Katherine Bode's recent article, ["The Equivalence of Close and Distant Reading"](https://read-dukeupress-edu.stanford.idm.oclc.org/modern-language-quarterly/article/78/1/77/19924/The-Equivalence-of-Close-And-Distant-Reading-Or), which makes a strong case for taking these questions extremely seriously.)
