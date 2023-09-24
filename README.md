---
mainfont: "fbb"
documentclass: article
fontsize: 12pt
date:
classoption: none
geometry: margin=1.2in
header-includes:
- \usepackage{fancyhdr, array, ifthen}
- \usepackage[margins=raggedright]{floatrow}
- \newcommand{\sectionbreak}{\clearpage}
- \pagestyle{fancy}
- \fancyhf{}
- \renewcommand{\headrulewidth}{0pt}
- | 
    \rhead{
        \ifthenelse{\value{page}=1}
        {\textbf{Formal Methods in Text Analysis I} | Dennis Yi Tenen }
        {}
    }
---

| Semester:                 | Fall 2023                         |
|---------------------------|-----------------------------------|
| Course Title:             | Formal Methods in Text Analysis I |
| Course Number:            | CLEN 6xxx                         |
| Contact:                  | dt2406@columbia.edu               |
| Office Hours:             | TBA                               |

## Course Description

This course on method in literary studies will introduce graduate students to the principles of
formal (as opposed to speculative) analysis. More than an emphasis on "form" or "computation,"
formal analysis requires the development of theoretical commitments, vulnerable, at the outset,
to empirical verification (being wrong). Many questions in the social sciences and the
humanities can benefit from formal analysis grounded in the particularities of language. The
attention to low-order single-document textual building blocks ("formal features")---word,
sentence, paragraph, story---will sharpen our intuitions about higher-order phenomena, such as
agency, power, authority, style, race, gender, or influence. *How* complex cultural dynamics
can be broken down into components, and then reassembled into models yielding scholarly
insight---that's the topic of this class. Comparison between documents, over time, and across
many texts will comprise Part II of the course.

Though all of the methods introduced can be done by pen and paper, the course will serve as a
gentle introduction to Python programming, using industry-standard tools for text processing.
No prior experience required to participate.

## Course Requirements & Grading

Students will be expected to read the approximate equivalent of three scholarly articles per
week, to attend the seminar weekly, to participate in the class discussion both in person and
online, and to develop a research project that will culminate in a paper. Advanced students
will have the option to integrate the course's themes with the subject matter of their
expertise.

Grade breakdown as follows: Class Participation 25%, weekly response online forum 25%, Midterm
project proposal 20%, Final project 30%.

## University Policies

When in doubt, cite! Plagiarism is insulting to your fellow students, your instructors, and to
the research community at large. It wastes my time and yours, and is, ultimately, not worth the
risk. Consult Columbia’s guidelines at <http://www.college.columbia.edu/academics/integrity> or
ask me for help early in the writing process. We will discuss the use appropriate of AI aids,
such as ChatGPT and Copilot, in class.

## Provisional Schedule & Reading List

## Week 0: Introductions.

Structure of the course. Policies, grading, requirements. What to expect. Experimental teaching
of the course. (Lab on Fridays?)

### Week 1: Formal methods

Formalism and structuralism historically considered. Common misconceptions. Formal analysis vs.
analysis of forms. Formal analysis in other disciplines. Strengths and limitations of the
approach. From intuition to model. Scale of analysis. Methods. Making the trip back to theory.
Asking the right questions. Principles of exploratory analysis. Sample bias. The
commensurability of claim and evidence. Sample and population. Exploration vs. confirmation.
Occam's razor (principle of parsimony, minimal viability).

- Boris Eichenbaum, Beth Paul, and Muriel Nesbitt, “[The Structure of Gogol’s ‘The
  Overcoat,’][12]” The Russian Review 22, no. 4 (1963): 377–99.
- "Preface" and "Qualitative Detective Work" pages in John Tukey, [*Exploratory Data
  Analysis*][11], (Reading, Mass: Pearson, 1977).
- Andrew Piper, “[Think Small: On Literary Modeling][13],” *PMLA*, September 18, 2017.

[11]: https://courseworks2.columbia.edu/courses/183356/files?preview=18278964
[12]: https://www-jstor-org.ezproxy.cul.columbia.edu/stable/126672
[13]: https://www-jstor-org.ezproxy.cul.columbia.edu/stable/27037379?searchText=andrew+piper+think+small&searchUri=%2Faction%2FdoBasicSearch%3FQuery%3Dandrew%2Bpiper%2Bthink%2Bsmall&ab_segments=0%2Fbasic_search_gsv2%2Fcontrol&refreqid=fastly-default%3Ac61ce26d39b4ef126acea1deb4c08d84

Lab 1: Intro to command line. File paths. Reading and writing files. Python by osmosis.
Units of analysis: character, word, sentence, paragraph, story, plot, discourse, archive.

## Week 2: Character

What is a character? The history of (encoding) alphabets. Glyphs and hieroglyphs. Telegraph
codes. Character encoding. Encoding politics. Universal code and universal language. What can
we do with letters?

- Sixth Book, Chapter 1 (pages 247 -- 259) in the [*Advancement of Learning*][24] (1605) by
  Francis Bacon.
- "Epistle," "To the Reader," and Chapter I (pages 385 -- 403) from [*An Essay Towards a Real
  Character, and a Philosophical Language*][21] (1668) by John Wilkins.
- "Chapter 4: Recondite Surfaces" in [*Plain Text*][23] (2017) from Dennis Yi Tenen.
- Markov, A. A. “[An Example of Statistical Investigation of the Text Eugene Onegin Concerning
  the Connection of Samples in Chains][22].” Science in Context 19, no. 4 (December 2006
  [1914]): 591–600.

Lab 2:  Plain text. Counting letters.

[21]: https://ia800405.us.archive.org/20/items/AnEssayTowardsARealCharacterAndAPhilosophicalLanguage/An_Essay_Towards_a_Real_Character_and_a.pdf
[22]: https://www-cambridge-org.ezproxy.cul.columbia.edu/core/services/aop-cambridge-core/content/view/EA1E005FA0BC4522399A4E9DA0304862/S0269889706001074a.pdf/an_example_of_statistical_investigation_of_the_text_eugene_onegin_concerning_the_connection_of_samples_in_chains.pdf
[23]: https://courseworks2.columbia.edu/courses/183356/files?preview=18358730
[24]: https://oll-resources.s3.us-east-2.amazonaws.com/oll3/store/titles/1433/0414_Bk.pdf

## Week 3: Syllable, meter

- Chapters 1-6 in Fussell's [*Poetic Meter & Poetic Form*][31] (1979).
- "[Universal Tendencies in the Semantics of the Diminutive][33]" by Daniel Jurafsky in.
  *Language* 72(3), pages 533–578.
- "[Regional Variation in West and East Coast African-American English Prosody and Rap
  Flows][32]" by Steven Gilbers, Nienke Hoeksema, Kees De Bot, and Wander Lowie in *Language
  and Speech*.

[31]: https://courseworks2.columbia.edu/courses/183356/files?preview=18445549
[32]: https://journals.sagepub.com/doi/full/10.1177/0023830919881479#bibr13-0023830919881479
[33]: https://www-jstor-org.ezproxy.cul.columbia.edu/stable/416278 

Lab 3: Versification.

### Week 4: Words

What is a word? Stem and lemma. Parts of speech. What they signify.

- Chapters I and II ("On Literary Construction" and "On Style") from Vernon Lee (Violet Paget),
  [*The Handling of Words and Other Studies in Literary Psychology*][31] (London: J. Lane,
  1923).
- Selections from L. A. Sherman, Analytics of Literature, a Manual for the Objective Study of
  English Prose and Poetry (Boston: Ginn, 1893).
- "Words on Words" by David Kaplan in 2011 *Journal of Philosophy* 108 (9):504-529.

[31]: https://ia903001.us.archive.org/3/items/handlingofwordso0000leev/handlingofwordso0000leev.pdf


### Week 5: Counting words

Object flow approach. Understanding types. Basic control structures. Word counts.

- Chapter 4, "What's in a Word" from *For the Love of Language: An Introduction to Linguistics*
by  Kate Burridge and Tonya N. Stebbins (Cambridge UP, 2019).
- Selections form Christopher D. Manning and Hinrich Schütze, Foundations of Statistical
  Natural Language Processing, 1st edition (Cambridge, Mass: The MIT Press, 1999).

### Week 6: Lexicon

Worldview, folk belief, discourse, ideology. Thematic clustering.

- Kenton Rambsy, “Jay Z’s American Gangster,” Black Camera 8, no. 2 (2017): 255–66.
- Timothy R. Tangherlini et al., “‘Mommy Blogs’ and the Vaccination Exemption Narrative:
  Results From A Machine-Learning Approach for Story Aggregation on Parenting Social Media
Sites,” JMIR Public Health and Surveillance 2, no. 2 (November 22, 2016): e6586.
- Teun A. van Dijk, “Discourse Analysis as Ideology Analysis,” in Language & Peace (Routledge,
  1995).

### Week 7: Sets and frequencies

Normalization, stemming, lemma vitiation. Lexical set intersection. Term frequency, inverse
term frequencies.

- Chapter 5, "Morphology: The Structure of Words" from *For the Love of Language: An
  Introduction to Linguistics* by  Kate Burridge and Tonya N. Stebbins (Cambridge UP, 2019).
- Set intersection tutorial.

### Week 8: Names

Proper names. Named entities. Nouns and objects.

- Searle, John R., 1958, “Proper Names”, Mind, 67(266): 166–173.
- “Toward a Computational Archaeology of Fictional Space.” New Literary History 49, no. 1
  (2018): 119–47.
- Selections from Kenton Rambsy, *The Geographies of African American Short Fiction* (Univ.
  Press of Mississippi, 2022).

### Week 9: Mapping space and distances

Types of space and distance. Document similarity. Clutter.

- Susan Grunewald and Andrew Janco, “[Finding Places in Text with the World Historical
  Gazeteer][81],” Programming Historian, February 11, 2022.
- Selections from Michel Marie Deza and Elena Deza, *Dictionary of Distances* (Elsevier
  Science, 2006).

[81]: https://programminghistorian.org/en/lessons/finding-places-world-historical-gazetteer

### Week 10: Syntax

What is a sentence. SVO. Length. Power dynamics.

- Selections from Stanley Fish, *How to Write a Sentence: And How to Read One* (New York:
  Harper Paperbacks, 2012).
- G. Udny Yule, “On Sentence-Length as a Statistical Characteristic of Style in Prose: With
  Application to Two Cases of Disputed Authorship,” Biometrika 30, no. 3/4 (1939): 363–90.
- Yi Tenen, Dennis. "Distributed Agency in the Novel" in New Literary History (2023).

### Week 11: Parsing Sentences

Learn to extant SVO structures from sentences. Brainstorm models.

- Chapter 9, "Syntax: The Structure of Sentences" from *For the Love of Language: An
  Introduction to Linguistics* by  Kate Burridge and Tonya N. Stebbins (Cambridge UP, 2019).
- SVO Tutorial with Spacy.

### Week 12: Narrative

Story and plot arcs. Time and events. Authorship and authority.

- Selections from Carolyn Wells, *The Technique of the Mystery Story* (Springfield, MA: Home
  Correspondence School, 1913).
- Boris Eichenbaum, Beth Paul, and Muriel Nesbitt, “The Structure of Gogol’s ‘The Overcoat,’”
  The Russian Review 22, no. 4 (1963): 377–99.
- Selections from Inderjeet Mani, *The Imagined Moment: Time, Narrative, and Computation*
  (Lincoln: University of Nebraska Press, 2010).

### Week 13: Authorship and authority

Finding the author. Ways of establishing authority.

- Jolene Galegher, Lee Sproull, and Sara Kiesler, “Legitimacy, Authority, and Community in
  Electronic Support Groups,” Written Communication 15, no. 4 (October 1, 1998): 493–94.
- Paul Rabinow, “Discourse and Power: On the Limits of Ethnographic Texts,” *Dialectical
  Anthropology* 10, no. 1/2 (1985): 1–13.

### Week 14: Project Workshops

Topics not covered in this class. Change over time. Ways forward. Building models revisited.
Plot, narrative. Readings on vectorization, topic modeling, network analysis.

- Selections from Martin Paul Eve, *Close Reading with Computers: Textual Scholarship,
  Computational Formalism* (Stanford University Press, 2019).

Brainstorm final project in class. Present final project proposals during the second session.
