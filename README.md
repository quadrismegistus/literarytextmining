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

We will progress through several modules of classes which range across domains of literary language: from words, to sentence syntax, to narratorial style, to character-spaces, to semantics and thematics, and finally to genres and the broader literary field. At the same time, throughout the course we will read one novel, Karen Yei Tamashita’s *Tropic of Orange* (1997), which rapidly alternates among narrators, styles, plots, and settings, and at times flirting with magical realism—a formal experimentation we will try to model computationally, while also reflecting on what aspects of the novel elude such methods of analysis.

## Objectives

Upon completing this course, students will be able to:

* Digitize texts and create metadata in order to build a text corpus appropriate for a given literary critical question.
* Distinguish between methods of computational literary studies, and identify the appropriate method for a given literary critical question.
* Program custom literary text analyses with the Python programming language, as well as call upon established tools and algorithms.
* Analyze and visualize data to determine its impact on a literary critical question.
* Deploy data and visualizations as part of a literary-critical argument.

## Texts

All texts for this course will be accessible from Canvas, besides the novel we will read, which you must purchase (at the bookstore or elsewhere):

* Karen Tei Yamashita, *Tropic of Orange* (Minneapolis: Coffee House Press, 1997)

## Evaluation

* **Practicum homework (35%)**: Practicum homework due on Monday at midnight each week will give students ample opportunity to practice the techniques learned in the course. Every Monday the practicum homework assigned the previous Tuesday and Thursday is due. Responses will be submitted through Canvas. These will sometimes take the form of short written responses, for instance describing the logic behind your corpus design. These will sometimes be an uploaded Jupyter notebook.

* **Final project presentation (20%)**: A final project done collaboratively in groups of 2-3 students, which will be presented in 5 minutes during the last class. For this class we'll organize a "Literary Text Mining Undergraduate Conference," to which we'll invite department faculty, graduate, and undergraduate students to attend. In the 110 minutes of our class, we'll spend 50-60 for presentations (5 minutes x 10-12 projects) and save 50-60 minutes for discussion. If you have concerns about participating in this event, please write me with your concerns and we will work together to find a solution.

* **Class project presentation (5%)**: Throughout the class, we will work together as a "lab" on a literary text mining project centering on Karen Tei Yamashita's *Tropic of Orange*. We will delegate two to three students to present the results of this class project during our last class (the LTM Undergraduate Conference). This project and presentation will be evaluated by the associate directors of the Stanford Literary Lab. This is only 5% of the grade. It's meant primarily to hold us together in our classwork as a team, a lab, which is a pedagogical

* **Final project mini-essay (20%)**: A short critical essay (5-7 pages) using the final project to make a critical argument. This can be the same argument given in the presentation, a corollary argument, or a completely new one. You can also write a close reading of literary texts using the data. Althoug the collaborative essence of the project will be given in the presentation, there is no substitute for writing, one of the most challenging and most personal of cognitive activities. This essay must a Word document, double-spaced, in 12-point Times New Roman font, with 1 inch margins, and should conform to MLA citation and formatting conventions. Please refer to the MLA Handbook (8th ed.) and the MLA guide on the Purdue OWL website. If you have questions about when or how to cite, please contact me.

* **In-class participation (20%)**: This class is part discussion seminar, part lab; it is not a lecture course. The content of the course therefore emerges organically from the interaction between all of us in the room. For this reason, both attendance and participation are required. Participation involves contributing spoken comments into the ongoing discussion within each class, as well as responses on the Canvas Help Forum (questions and answers valued equally). If you struggle with either kind of involvement, please email me with your concerns, and we will work together to find a solution. *Note: This class has a zero-tolerance policy for any and all forms of disrespect or harassment. All participation must respect the personhood and identity of others.*

### Summary

| Component | Weight | Due date |
| --------- | ------ | -------- |
| Practicum assignments | 35% | Mondays at midnight |
| Final project presentation (10 minutes; 2-3 person groups) | 20% | Tues Jun 4|
| Final project mini-essay (5-10 pages; written individually) | 20% | Tues Jun 11 |
| Class/Canvas participation | 20% | n/a |
| Class project presentation\*| 5%** | Tues Jun 4

\* The results of our classwork experiments on Karen Tei Yamashita's *Tropic of Orange*; the presenters will be delegated.

**  As evaluated by the associate directors of the Stanford Literary Lab.

## Schedule

This schedule is subject to change.

Abbreviations:

* *ToO*: Karen Tei Yamashita, *Tropic of Orange* (Minneapolis: Coffee House Press, 1997). Page numbers are given for this edition.


| Week | Class | Day | Date | Topic                                                                       | Class modules                                                                                         | Practicum due                                                                                                          | Reading due                      |
|------|-------|-----|------|-----------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------|----------------------------------|
| 1    | 1     | T   | 4/2  | [(1) Setup](#1-Setup)                                                       | (1A) Class introduction; [(1B) Installation](#1B-Installation); [(1C) The Terminal](#1C-The-Terminal) |                                                                                                                        |                                  |
|      | 2     | Th  | 4/4  | [(2) Corpora](#2-Corpora)                                                   | [(2A) Intro to corpora](#2A-Introduction-to-corpora); [(2B) Building a corpus](#2B-Building-a-corpus) |                                                                                                                        | *ToO*, 7-25 [“Monday," ch. 1-3]  |
| 2    | 3     | T   | 4/9  | [(3) Python 101 + Text Mining 101](#3-Python-101--Text-Mining-101)          | [(3A) Jupyter Lab](#3B-Jupyter-Lab); [(3B) Baby Python](#03B-Baby-Python.ipynb)                       | [(1C) The Terminal](#1C-The-Terminal); [(2B) Building a corpus](#2B-Building-a-corpus)                                 |                                  |
|      | 4     | Th  | 4/11 |                                                                             | [(3C) Files and strings](#3C-Files-and-strings)                                                       |                                                                                                                        | *ToO*, 25-50 [“Monday," ch. 4-7] |
| 3    | 5     | T   | 4/16 |                                                                             | [(3D) Lists and words](#3D-Lists-and-words)                                                           | [(3B) Baby Python](#03B-Baby-Python.ipynb); [(3C) Files and strings](#3C-Files-and-strings)                            |                                  |
|      | 6     | Th  | 4/18 |                                                                             | [(3E) Dictionaries and word counts](#3E-Dictionaries-and-word-counts)                                 |                                                                                                                        | *ToO*, 51-84 [“Tuesday"]         |
| 4    | 7     | T   | 4/23 | [(4) Corpus Mining](#4-Corpus-Mining)                                       | [(4A) Pandas and the dataframe](#4A-Pandas-and-the-dataframe)                                         | [(3D) Lists and words](#3D-Lists-and-words); [(3E) Dictionaries and word counts](#3E-Dictionaries-and-word-counts)     |                                  |
|      | 8     | Th  | 4/25 |                                                                             | [(4B) Comparing word counts](#4B-Comparing-word-counts)                                               |                                                                                                                        | *ToO*, 85-118 [“Wednesday”]      |
| 5    | 9     | T   | 4/30 |                                                                             | [(4C) Visualizing word counts](#4C-Visualizing-word-counts)                                           | [(4A) Pandas and the dataframe](#4A-Pandas-and-the-dataframe); [(4B) Comparing word counts](#4B-Comparing-word-counts) |                                  |
|      | 10    | Th  | 5/2  | [(5) Natural language processing (NLP)](#5-Natural-language-processing-NLP) | [(5A) Part of speech tagging](#5A-Part-of-speech-tagging)                                             |                                                                                                                        | *ToO*, 119-150 [“Thursday”]      |
| 6    | 11    | T   | 5/7  |                                                                             | [(5B) Literary Geography](#5B-Literary-Geography)                                                     | [(4C) Visualizing word counts](#4C-Visualizing-word-counts)                                                            |                                  |
|      | 12    | Th  | 5/9  | [(6) Social network analysis](#6-Social-network-analysis)                   | [(6A) Introduction to networks](#6A-Introduction-to-networks)                                         |                                                                                                                        | *ToO*, 151-180 [“Friday”]        |
| 7    | 13    | T   | 5/14 |                                                                             | [(6B) Character networks](#6B-Character-networks)                                                     | [(5A) Part of speech tagging](#5A-Part-of-speech-tagging); [(5B) Literary Geography](#5B-Literary-Geography)           |                                  |
|      | 14    | Th  | 5/16 | [(7) Content analysis](#7-Content-analysis)                                 | [(7A) Generating topic models](#7A-Generating-topic-models)                                           |                                                                                                                        | *ToO*, 181-208 [“Saturday”]      |
| 8    | 15    | T   | 5/21 |                                                                             | [(7B) Reading topic models](#7B-Reading-topic-models)                                                 | [(6B) Character networks](#6B-Character-networks)                                                                      |                                  |
|      | 16    | Th  | 5/23 | [(8) Clustering](#8-Clustering)                                             | [(8A) Cluster analysis](#8A-Cluster-analysis)                                                         |                                                                                                                        | *ToO*, 209-230 [“Sunday”]        |
| 9    | 17    | T   | 5/28 |                                                                             | [(8B) Principal component analysis](#8B-Principal-component-analysis)                                 | [(7B) Reading topic models](#7B-Reading-topic-models)                                                                  |                                  |
|      | 18    | Th  | 5/30 | Final preparations                                                          |                                                                                                       |                                                                                                                        |                                  |
| 10   | 19    | T   | 6/4  | Presentations!                                                              |                                                                                                       |                                                                                                                        |                                  |



## Content

Homework assignments (in **bold**) are due the following session unless otherwise noted.


### (1) Setup

#### (1A) Class introductions
* Introductions
* What is literary text mining? What is possible?
* Going over syllabus

#### [(1B) Installation](01_setup/1B_installation_instructions.md)
* Install Anaconda, NLTK, and spaCy
* Install git
* Clone class repository


#### [(1C) The Terminal](01_setup/1C_the_terminal.md)

* Learn the basics of terminal navigation
* Learn how to read and write files from the terminal
* [**To practice**: Complete the Terminal Maze Adventures!](01_setup/1C_the_terminal_TODO)


### (2) Corpora

#### [(2A) Introduction to corpora](02_corpora/2A_intro_to_corpora.md)

* What is a corpus?
* Examples of corpora
* Our class corpora
* Corpus design

#### [(2B) Building a corpus](02_corpora/2B_building_a_corpus.md)

* How to digitize texts
* How to create metadata
* How to structure corpus
* [**To practice**: Build a corpus with at least 10 texts, supported by at least two actionable metadata columns](02_corpora/2B_building_a_corpus.md#Practicum)


### (3) Python 101 + Text Mining 101

#### (3A) Jupyter Lab

#### (3B) Baby Python

* "Hello world"
* Integers
* Strings
* Variables
* If/Then

#### (3C) Files and strings

* Open text
* String slice text
* Functions

#### (3D) Lists and words

* Lists
* Splitting texts into words (text as string -> text as list)
* NLTK (concordance, dispersion)
* Type-Token Ratio

#### (3E) Dictionaries and word counts

* Loops
* Dictionaries
* Counting words (text as list -> word counts as dictionary)


### (4) Corpus Mining

#### (4A) Pandas and the dataframe

* Introduction to pandas
* How to think and use dataframes

#### (4B) Comparing word counts
* Correlations
* Most distinctive words
* **To practice**: Find the distinctive words of a text in your corpus

#### (4C) Visualizing word counts
* Matplotlib
* Tableau


### (5) Natural language processing (NLP)

#### (5A) Part of speech tagging
* Part of speech analysis
* Lemmatizing
* Named Entity Recognition
* **To practice**: Part-of-speech tag your corpus

#### (5B) Literary Geography
* Named Entity Recognition continued
* Mapping places
* **To practice**: Map some of the place entities in your corpus


### (6) Social network analysis

#### (6A) Introduction to networks
* Introduction to social network analysis
* NetworkX
* Draw social media networks

#### (6B) Character networks
* BookNLP
* Drawing social networks in texts
* **To practice**: Draw social networks for your own corpus


### (7) Content analysis
#### (7A) Generating topic models
* Generating topic models
* Reading topic models

#### (7B) Reading topic models
* Reading output
* Visualizing topic models
* **To practice**: Topic model your corpus and write a brief discussion of two topics


### (8) Clustering
#### (8A) Cluster analysis
* Hierarchical clustering
* Kmeans clustering

#### (8B) Principal component analysis
* PCA and multivariate analysis
* Color by cluster
* **To practice**: Make a PCA or cluster visualization of your corpus


### (9) Classification (machine learning)

#### (9A) Intro to hypothesis testing
* General classification framework

#### (9B) Logistic regression
* Classification continued
* Logistic regression
* **To practice**: Classify a type of text in your corpus



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

This syllabus and these course materials are deeply indebted to those of David Bamman's [Applied Natural Language Procssing](https://github.com/quadrismegistus/literarytextmining_spring2019) course: hats off to David for making such great materials available.
