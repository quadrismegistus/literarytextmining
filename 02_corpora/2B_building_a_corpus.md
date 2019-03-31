# (2B) Building a corpus

*Note: This text adapted from Marissa Gemma's guide, ["Preparing texts for Python."](https://github.com/quadrismegistus/python-dighum/wiki/Preparing-texts-for-Python)*

## Question + Corpus

If you have a DH project in mind, you probably already have an idea of which texts you'll want to study. This group of texts to analyze is called a corpus; librarians, linguists, and lots of other researchers have been using corpora for years to analyze large amounts of (usually textual) data. (Some famous examples can be found here, here, and here.)

## How to build a corpus


### (1) Digitize some texts

Python is picky about the kind of texts you feed it. You can't just throw PDFs, Microsoft Word docs, or even some kinds of .txt files at it--your program will break, and you'll have an unpleasant encoding problem on your hands. (For a quick primer on encoding and Unicode, read this; and though it's aimed at software developers, you might also be interested in this longer explanation.)

So what kinds of texts can you feed Python for your analysis? You will need plain text (.txt) files which all have the same kind of encoding, either UTF-8 or UTF-16. UTF-8 is a good bet for our purposes; when you save a plain text file from Project Gutenberg, for example, it is in UTF-8.

#### Choose your own adventure

* **If you already have .txt files** from somewhere besides Gutenberg, check to make sure they have the right encoding: open them with a text editor (like TextWrangler or Notepad++), and look at the information displayed about the file at the bottom of the window. In TextWrangler, you'll see a drop-down menu that displays the current file encoding (it might say "Western MacOS Roman" or "UTF-8"). To change the encoding, just select "UTF-8" from the menu, and save the file. Voilà! Python can play with this file now.

* **If your text is in MSWord**, you can convert it to UTF-8 in Word by going to "Save as" and selecting "raw text (.txt)". A window will now pop up asking you about converting the file; select "other encoding" and then choose "Unicode 6.1 UTF-8".

* **If you have PDF files**, make some coffee. This is going to take a little more time. You will need to convert your PDFs to text files using an OCR (optical character recognition) program, like ABBYY FineReader. If you're on campus, you can use ABBYY either in Green Library (by the scanners) or at CESTA. ABBY will produce a text file that you can then feed Python.*

* **If you have actual books**, make twice as much coffee. First you'll need to scan the books; then see "If you have PDF files."

### (2) Create metadata

As you're getting your texts together, think about what kind of other information you're going to want to "attach" to your textual data--for instance, you'll probably want the year of publication, the author's name, the title; maybe you'll want the author's gender or nationality, or the genre of the text. This is all metadata: data about your data.

There are lots of ways to store metadata, and making sure the metadata and the data stick together can be tricky. A simple solution that will serve our purposes nicely is to store the metadata in the filename of the text, using the following format: "Pieceofdata.Pieceofdata.Pieceofdata.txt". So for example, if you want to keep track of the pub year, author's name, title, and genre, you would have titles that look like this: "1835.Poe.Berenice.Gothic.txt".

You can include whatever metadata you want to, but what you must do is be consistent in your storage of metadata. That's the only way to ensure you'll be able to access it computationally. And be sure to use periods to separate items from one other-- we'll explain why in a few sessions; for now, suffice it to say that it'll radically simplify your tasks.

### (3) Create a directory structure

To get Python to rifle through your texts, you won't just click on folders and files and open them; instead, you'll tell Python where to find the files, command it to open them, etc. This means you need to know where those files are, and you need to store them nicely and neatly.

Put your texts in a single folder called something descriptive (like, "poe_corpus") and don't use special characters in this title (like ", ' , or .). Save your corpus folder inside another folder: the folder where you'll put your Python scripts. (If you don't have that folder yet, just make one in an easy-to-access place, like the top layer of your Dropbox folder, or on your desktop.)

## Next steps

And voilà: you have a corpus! Now, on to the fun part.

Notes

* There are a lot of possible complications here. For example: if you have a fuzzy PDF of a historical text, the character recognition might not be very accurate, so you'll need to correct your text before you analyze it.