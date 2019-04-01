# (2B) Building a corpus

This notebook describes the pragmatics of building a corpus. See [the previous module](2A_intro_to_corpora.md#A-corpus-is-a-question) for reflections on corpus design.

*Note: This notebook is adapted from Marissa Gemma's guide, ["Preparing texts for Python."](https://github.com/quadrismegistus/python-dighum/wiki/Preparing-texts-for-Python)*


## How to build a corpus

### (1) Create a corpus folder

**To do:** Run these lines in the terminal.

```
cd ~/literarytextmining       # go to class folder
cd corpora                    # enter corpora folder from there
mkdir my_corpus               # make a folder for your corpus
cd my_corpus                  # go into your corpus folder
mkdir texts                   # make a folder to put your text files in
```


### (2) Digitize texts

#### To do

* Save each text of your corpus as a text file to `~/literarytextmining/corpora/my_corpus/texts`.

#### What kind of text file?

Python is picky about the kind of texts you feed it. You can't just throw PDFs, Microsoft Word docs, or even some kinds of .txt files at it--your program will break, and you'll have an unpleasant encoding problem on your hands. (For a quick primer on encoding and Unicode, read this; and though it's aimed at software developers, you might also be interested in this longer explanation.)

So what kinds of texts can you feed Python for your analysis? You will need plain text (.txt) files which all have the same kind of encoding, either UTF-8 or UTF-16. UTF-8 is a good bet for our purposes; when you save a plain text file from Project Gutenberg, for example, it is in UTF-8.

#### How to create a valid text file

* **If you already have .txt files** from somewhere besides Gutenberg, check to make sure they have the right encoding: open them with a text editor (like TextWrangler or Notepad++), and look at the information displayed about the file at the bottom of the window. In TextWrangler, you'll see a drop-down menu that displays the current file encoding (it might say "Western MacOS Roman" or "UTF-8"). To change the encoding, just select "UTF-8" from the menu, and save the file. Voilà! Python can play with this file now.

* **If your text is in MSWord**, you can convert it to UTF-8 in Word by going to "Save as" and selecting "raw text (.txt)". A window will now pop up asking you about converting the file; select "other encoding" and then choose "Unicode 6.1 UTF-8".

* **If you have PDF files**, make some coffee. This is going to take a little more time. You will need to convert your PDFs to text files using an OCR (optical character recognition) program, like ABBYY FineReader. If you're on campus, you can use ABBYY either in Green Library (by the scanners) or at CESTA. ABBY will produce a text file that you can then feed Python.*

* **If you have actual books**, make twice as much coffee. First you'll need to scan the books; then see "If you have PDF files."

#### How to name the files

Principles of filenaming:

* It doesn't matter what you name these text files ("Austen.PrideAndPrejudice.txt" or "austen_pp.txt" or "novel02245.txt"), as long as each filename is unique.

	* (Why doesn't it matter what we name the file? Because the filename will be included in the metadata, so we can link this arbitrary filename to its relevant information in the matadata.)


* The file extension must be .txt.
	

* It's more convenient if the filename has no spaces (use _ or - instead).

* It doesn't hurt to make filenames descriptive.

	* (You can jam some important information into a filename to make finding the text in Mac Finder on its own easier, for example. For instance, if you want to keep track of the pub year, author's name, title, and genre, you could name the text: "1835.Poe.Berenice.Gothic.txt".)



#### Make sure to save these .txt files in the right place

Save them to:
`~/literarytextmining/corpora/my_corpus/texts`

### (2) Create metadata

#### To do

* Create an Excel spreadsheet here: `~/literarytextmining/corpora/my_corpus/metadata.xls`.

* Make the first column "fn". For every text file you have, each of which is a row, write its filename in this "fn" column.

	* ****Tip:**** Go to your texts folder in Mac Finder (or Windows Explorer?). Select All (Cmd+A); Copy (Cmd+C); paste in Excep (Cmd+V).

* Any metadata can be recorded as columns listed after "fn". The filename is "fn" is relative to `~/literarytextmining/corpora/my_corpus/texts`.

* For example:

| fn      | Chapter                             | Form          | Dialogue | Network                                                                                                                                          |
|---------|-------------------------------------|---------------|----------|--------------------------------------------------------------------------------------------------------------------------------------------------|
| 003.txt | CHAPTER 1. Loomings.                | Essay/Fiction | No       | Ishmael                                                                                                                                          |
| 004.txt | CHAPTER 2. The Carpet-Bag.          | Fiction       | No       | Ishmael                                                                                                                                          |
| 005.txt | CHAPTER 3. The Spouter-Inn.         | Fiction       | Yes      | Ishmael<>PeterCoffin; Bulkington; Queequeg; Queequeg>Ishmael                                                                                     |
| …       | …                                   | …             | …        | …                                                                                                                                                |


#### Things to think about

As you're getting your texts together, think about what kind of other information you're going to want to "attach" to your textual data--for instance, you'll probably want the year of publication, the author's name, the title; maybe you'll want the author's gender or nationality, or the genre of the text. This is all metadata: data about your data.

## Practicum

### To do

Create (the first draft of) your corpus.

* Follow the instructions above.

* Remember that a corpus is a question. What question do you want to ask?

* The corpus may be include texts of any genre.

* It must have at least 10 texts, and no more than a 100.

* Texts should be at least a paragraph long.

* It must have at least two significant (question-enabling) metadata columns.

* If you can't find all the .txt files, don't sweat it yet. Focus on the metadata and the principle behind it.

* In the Canvas assignment,

	* Write a paragraph describing your corpus and the question you want to ask.

	* Attach a zipped folder of metadata and texts 