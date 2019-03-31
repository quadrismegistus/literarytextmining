# English 184E: “Literary Text Mining” (Spring 2019)

## Information

* Time: T/Th 4:30-6:20
* Location: 240-110
* Instructor: Ryan Heuser
* E-mail: heuser@stanford.edu
* Office: 460-419
* Office hours: T/Th 3:30-4:30

## Description

What happens when computers read Shakespeare? What can digital methods tell us about literary language—about how it works, how it evolved, and how it relates to other forms of language? How, for instance, are the rhythms of poetry different from the rhythms of newspapers? What kinds of social networks do plays and novels create? How are female characters in novels described differently than male characters? New techniques in the digital humanities, computational linguistics, and natural language processing make it possible to ask these types of questions of literature. In this course, we will learn how to participate in this exciting new area of interdisciplinary research, while also probing its challenges and limitations.

This course is an introduction to the theories and methods of computational literary studies. It presumes no background in programming, computer science, or literary criticism. Students will begin with the building blocks of the Python programming language before moving on to more complex analyses of literary texts. Students will learn a variety of ways to discover patterns in textual data, visualize these patterns, and present them as part of a broader literary critical argument.

We will progress through several modules of classes, each representing a distinct, and perhaps broader, domain of literary language: from words, to sentence syntax, to narratorial style, to character-spaces, to semantics and thematics, and finally to genres and the broader literary field. At the same time, throughout the course we will read one novel, Karen Yei Tamashita’s Tropic of Orange (1997), which rapidly alternates among narrators, styles, plots, and settings—a formal experimentation we will try to model computationally, while also reflecting on what aspects of the novel elude such methods of analysis.

## Objectives

Upon completing this course, students will be able to:

* Distinguish between methods of computational literary studies, and identify the appropriate method for a given literary critical question.
* Digitize texts and build corpora appropriate for a given literary critical question.
* Program custom literary text analyses with the Python programming language, as well as call upon established tools and algorithms.
* Analyze and visualize data to determine its impact on a literary critical question.
* Deploy data and visualizations as part of a literary-critical argument.

## Texts

All texts for this course will be accessible from Canvas, besides the novel we will read, which you must purchase (at the bookstore or elsewhere):

* Karen Tei Yamashita, *Tropic of Orange* (Minneapolis: Coffee House Press, 1997)

## Assignments

Homework due at the beginning of each week will give students ample opportunity to practice the techniques learned in the course. In addition to homework and class participation, students’ grades will be assessed according to two major assignments: a midterm project, done individually, of a single “result” described (and optionally visualized) in a 2-4 page report; and a final project, done collaboratively in groups of 2-3 students, of a 10-12 page essay in which data analysis and visualization play a key argumentative role.

* **In-class participation**: This class is part discussion seminar, part lab; it is not a lecture course. The content of the course therefore emerges organically from the interaction between all of us in the room. For this reason, both attendance and participation are required. Participation normally involves contributing spoken comments into the ongoing discussion within each class. If you struggle with this kind of involvement, please email me with your concerns, and we will work together to find a solution. Note: This class has a zero-tolerance policy for any and all forms of disrespect or harassment. You need not agree with anything said in this course, but your disagreement must be articulated with respect.

* **Homework assignments**: …

* **Midterm report**: …

* **Final project and presentation**: …

All written work must be double-spaced, in 12-point Times New Roman font, with 1 inch margins, and should conform to MLA citation and formatting conventions. Please refer to the MLA Handbook (8th ed.) and the MLA guide on the Purdue OWL website. Remember that anything that is not of your own invention, whether direct quotes or paraphrases, must be cited. If you have questions about when or how to cite, please contact me.

## Evaluation

| Component | Weight | Due date |
| --------- | ------ | -------- |
| Practicum assignments | 20% | Mondays at midnight |
| Midterm data report (1-2 pages with 1-2 figures)| 20% | Tues May 7 |
| Final project presentation (10 minutes; 2-3 person groups) | 20% | Tues Jun 4|
| Final project mini-essay (5-10 pages; written individually) | 20% | Tues Jun 11 |
| Class participation | 15% | n/a |
| Class project presentation**| 5%*** | Tues Jun 4

** The results of our classwork experiments on Karen Tei Yamashita's *Tropic of Orange*; the presenters will be delegated.

***  As evaluated by the current postdocs of the Stanford Literary Lab.

## Schedule

This schedule is subject to change.

Abbreviations:

* *ToO*: Karen Tei Yamashita, *Tropic of Orange* (Minneapolis: Coffee House Press, 1997). Page numbers are given for this edition.

| Week | Class | Day | Date | Topic                       | Class modules                                                                                           | Practicum due                                                                                           | Reading due                     |
|------|-------|-----|------|-----------------------------|---------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------|---------------------------------|
| 1    | 1     | T   | 4/2  | Introduction                | (1A) Class introduction; [(1B) Installation](#1B-Installation); [(1C) The Terminal](#1C-The-Terminal)   |                                                                                                         |                                 |
|      | 2     | Th  | 4/4  | Corpora                     | [(2A) Intro to corpora](#2A-Introduction-to-corpora); [(2B) Building a corpus](#2B-Building-a-corpus)   | [(1C) The Terminal](01_setup/01C_the_terminal_TODO)                                                     | ToO, 7-25 [“Monday," ch. 1-3]   |
| 2    | 3     | T   | 4/9  | Python                      | [(3A) Jupyter Lab](#3B-Jupyter-Lab); [(3B) Baby Python](#03B-Baby-Python.ipynb)                         | (2A) Building corpora                                                                                   |                                 |
|      | 4     | Th  | 4/11 |                             | [(3C) Lists and dictionaries](#3C-Lists-and-dictionaries)                                               | (3B) Baby Python                                                                                        | ToO, 25-50 [“Monday," ch. 4-7]  |
| 3    | 5     | T   | 4/16 | Words (single text)         | (4A) Reading text files; (4B) Tokenizing                                                                | (3C) Lists and dictionaries                                                                             |                                 |
|      | 6     | Th  | 4/18 |                             | (4C) Counting words                                                                                     | (4A) Reading text files; (4B) Tokenizing                                                                | ToO, 51-84 [“Tuesday"]    |
| 4    | 7     | T   | 4/23 |                             | (4D) Collocations                                                                                       | (4C) Counting words                                                                                     |                                 |
|      | 8     | Th  | 4/25 | Words (corpus)              | (6A) Loops and control structures                                                                       | (4D) Collocations                                                                                       | ToO, 85-118 [“Wednesday”] |
| 5    | 9     | T   | 4/30 |                             | (6B) Introduction to Pandas                                                                             |                                                                                                         |                                 |
|      | 10    | Th  | 5/2  | Visualization               | (7A) Tableau                                                                                            | [download and install Tableau](https://www.tableau.com/academic/students)                               | ToO, 119-150 [“Thursday”] |
| 6    | 11    | T   | 5/7  | Distinctive words           | (6D) Most distinctive words                                                                             | Midterm: data report                                                                                    |                                 |
|      | 12    | Th  | 5/9  | Natural Language Processing | (8A) Part of speech tagging; (8B) Named Entity Recognition                                              |                                                                                                         | ToO, 151-180 [“Friday”]   |
| 7    | 13    | T   | 5/14 | Literary Geography          | (9A) Making a gazetteer; (9B) Mapping Place Names                                                       |                                                                                                         |                                 |
|      | 14    | Th  | 5/16 | Social Network Analysis     | (10A) NetworkX; (10B) Social Media Networks                                                             |                                                                                                         | ToO, 181-208 [“Saturday”] |
| 8    | 15    | T   | 5/21 |                             | (10C) BookNLP; (10D) Social Networks in Literature                                                      |                                                                                                         |                                 |
|      | 16    | Th  | 5/23 | Content Analysis            | Generating Topic Models                                                                                 | Read: ToO, 209-230 [“Sunday”]                                                                           |                                 |
| 9    | 17    | T   | 5/28 | Clustering                  | Hclust and Kmeans                                                                                       |                                                                                                         |                                 |
|      | 18    | Th  | 5/30 |                             | PCA                                                                                                     |                                                                                                         |                                 |
| 10   | 19    | T   | 6/4  | Presentations!              |                                                                                                         |                                                                                                         |                                 |


## Content

Homework assignments (in **bold**) are due the following session unless otherwise noted.


### (1) Setup

#### (1A) Class introductions
* Introductions
* What is literary text mining? What is possible?
* Going over syllabus

#### [(1B) Installation](01A_setup/01B_installation_instructions.md)
* Install Anaconda, NLTK, and spaCy
* Install git
* Clone class repository


#### [(1C) The Terminal](01_setup/01C_the_terminal.md)

* Learn the basics of terminal navigation
* Learn how to read and write files from the terminal


### (2) Corpora

#### [(2A) Introduction to corpora](02_corpora/02A_intro_to_corpora.md)

#### [(2B) Building a corpus](02_corpora/02B_building_a_corpus.md)



### (3) Python

#### [(3A) Jupyter Lab](03_python/03A_jupyter_lab.md)

#### [(3A) Baby Python](03_python/03B_baby_python.ipynb)

* "Hello world"
* Integers
* Strings
* Variables

#### [(3C) Lists and dictionaries](03_python/03C_lists_and_dictionaries.ipynb)

* Lists
* Dictionaries


### (4) Intro to Text Mining

#### (4A) Reading text files

* Open text
* String slice text

#### (4B) Tokenizing

* Splitting texts into words (text as string -> text as list)
* Tokenizers

#### (4C) Counting words

* Counting words (text as list -> word counts as dictionary)


### (5) Mining Individual Texts

#### (5A) Linguistic diversity

* Number of words (list of tokens)
* Number of unique words (set of types)
* Type/token ratio

#### (5B) Key Word In Context (KWIC)

#### (5C) Dispersion plots


### (6) Mining Corpora

#### (6A) Loops and control structures

#### (6B) Comparing word counts

#### (6C) Most distinctive words
* Most distinctive words
* Stylometry
* **To practice**: Find the distinctive words of a text in your corpus


### (7) Natural language processing

#### (7A) Part of speech

* Part of speech analysis
* Lemmatizing

#### (7B) Named Entity Recognition
* Named Entity Recognition

* **To do**: 
* **To practice**: Part-of-speech tag your corpus. Which parts of speech distinguish a specific text in your corpus? Which named entities are in your corpus?



### Week 5: Visualization
#### (9) Tues Apr 30
* Matplotlib
* Scatterplots
* **To read**: *Tropic of Orange*, 119-150 [“Thursday”]

#### (10) Thurs May 2
* Tableau
* Line graphs
* Geographic visualization
* **To do**: **MIDTERM DATA REPORT**



### Week 6: Social network analysis
#### (11) Tues May 7
* Introduction to social network analysis
* NetworkX
* Draw social media networks
* **To read**: *Tropic of Orange*, 151-180 [“Friday”]

#### (12) Thurs May 9
* BookNLP
* Drawing social networks in texts
* **To practice**: Draw social networks for your own corpus


### Week 7: Content analysis
#### (13) Tues May 14
* Generating topic models
* Reading topic models
* **To read**: *Tropic of Orange*, 181-208 [“Saturday”]

#### (14) Thurs May 16
* Visualizing topic models
* **To practice**: Topic model your corpus and write a brief discussion of two topics



### Week 8: Clustering
#### (15) Tues May 21
* Hierarchical clustering
* Kmeans clustering
* **To read**: *Tropic of Orange*, 209-230 [“Sunday”]

#### (16) Thurs May 23
* PCA and multivariate analysis
* Color by cluster
* **To practice**: Make a PCA or cluster visualization of your corpus


### Week 9: Classification (machine learning)
#### (17) Tues May 28
* General classification framework
* Logistic regression
* **To practice**: Classify a type of text in your corpus

#### (18) Thurs May 30
* Classification continued
* Presentation preparation

### Week 10: Presentations!
#### (19) Tues June 4
* Final project presentations!


## Appendix

### Students with Documented Disabilities 
Students who may need an academic accommodation based on the impact of a disability must initiate the request with the Office of Accessible Education (OAE).  Professional staff will evaluate the request with required documentation, recommend reasonable accommodations, and prepare an Accommodation Letter for faculty dated in the current quarter in which the request is being made. Students should contact the OAE as soon as possible since timely notice is needed to coordinate accommodations.

OAE contact information: <br/>563 Salvatierra Walk
<br/>650-723-1066
<br/>[http://studentaffairs.stanford.edu/oae](http://studentaffairs.stanford.edu/oae)
 
### Honor Code 
The Honor Code is the University's statement on academic integrity written by students in 1921. It articulates University expectations of students and faculty in establishing and maintaining the highest standards in academic work: 
The Honor Code is an undertaking of the students, individually and collectively:

1.	that they will not give or receive aid in examinations; that they will not give or receive unpermitted aid in class work, in the preparation of reports, or in any other work that is to be used by the instructor as the basis of grading;
2.	that they will do their share and take an active part in seeing to it that others as well as themselves uphold the spirit and letter of the Honor Code.

The faculty on its part manifests its confidence in the honor of its students by refraining from proctoring examinations and from taking unusual and unreasonable precautions to prevent the forms of dishonesty mentioned above. The faculty will also avoid, as far as practicable, academic procedures that create temptations to violate the Honor Code. 
While the faculty alone has the right and obligation to set academic requirements, the students and faculty will work together to establish optimal conditions for honorable academic work.

### Acknowledgments

This syllabus and these course materials are deeply indebted to David Bamman's [Applied Natural Language Procssing](https://github.com/quadrismegistus/literarytextmining_spring2019) course, from which I've sometimes taken whole sections with minimal adaptations.

I have also looked
