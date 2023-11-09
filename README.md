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

### Week 0: Introductions

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

### Week 2: Character

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

### Week 3: Syllable, meter

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

### Week 4: Words 1

What is a word? Stem and lemma. Parts of speech. What they signify.

- Chapters I and II ("On Literary Construction" and "On Style") from Vernon Lee (Violet Paget),
  [*The Handling of Words and Other Studies in Literary Psychology*][41] (London: J. Lane,
  1923).
- Chapters 3, 4, and 6 from L. A. Sherman, [*Analytics of Literature, a Manual for the
  Objective Study of English Prose and Poetry*][42] (Boston: Ginn, 1893).
- ~~"[Words on Words][43]" by David Kaplan in 2011 *Journal of Philosophy* 108 (9):504-529.~~
- "[Types and Tokens][45]" by Linda Wetzel in the *Stanford Encyclopedia of Philosophy*


[41]: https://ia903001.us.archive.org/3/items/handlingofwordso0000leev/handlingofwordso0000leev.pdf
[42]: https://archive.org/download/in.ernet.dli.2015.184135/2015.184135.Analytics-Of-Literature.pdf
[43]: https://www-jstor-org.ezproxy.cul.columbia.edu/stable/23142919
[44]: https://courseworks2.columbia.edu/courses/183356/files?preview=18648121
[45]: https://plato.stanford.edu/entries/types-tokens/

Special guest, Professor Jessica E. Merrill, Columbia Slavic. Prepare Chapter 1: Comparative
Philology from her book, on the [*Origins of Russian Literary Theory*.][44]

### Week 5: Words 2

Object flow approach. Understanding types. Basic control structures. Word counts.

- “[Toward a Computational Archaeology of Fictional Space][51]” by DYT in *New Literary History* 49, no. 1 (2018): 119–47.
- ~~Chapter 4, "What's in a Word" from [*For the Love of Language: An Introduction to Linguistics*][52]
by  Kate Burridge and Tonya N. Stebbins (Cambridge UP, 2019).~~
- Browse Chapter 2, on Words in Christopher D. Manning and Hinrich Schütze, [*Foundations of Statistical
  Natural Language Processing*][53], (Cambridge, Mass: The MIT Press, 1999).

  [51]: https://academiccommons.columbia.edu/doi/10.7916/D8QC1M5D
  [52]: https://courseworks2.columbia.edu/courses/183356/files?preview=18739161
  [53]: https://courseworks2.columbia.edu/courses/183356/files?preview=18739184

### Week 6: Lexicon

Worldview, folk belief, discourse, ideology. Thematic clustering.

- Chapter 3, "[Morphemes and Words: Introduction to the Lexicon][61]" from the *Linguistics for Students of Literature* (1980) by Traugott Elizabeth Closs and Mary Louise Pratt. 
- Kenton Rambsy, “[Jay Z’s American Gangster][62],” Black Camera 8, no. 2 (2017): 255–66.
- "[The Technique of Semantics][63]" by John Firth in the *Transactions of the Philological Society*, November 1935.


[61]: https://courseworks2.columbia.edu/courses/183356/files?preview=18811679
[62]: https://www-jstor-org.ezproxy.cul.columbia.edu/stable/10.2979/blackcamera.8.2.15
[63]: https://onlinelibrary.wiley.com/doi/10.1111/j.1467-968X.1935.tb01254.x
[64]: https://pubmed.ncbi.nlm.nih.gov/27876690/

### Week 7: Names and Networks

- Chapter IV on the "Literary Speech Situation" from [*Toward a Speech Act Theory of Literary Discourse*][71] by Mary Louise Pratt.
- Searle, John R., 1958, “[Proper Names][72]”, Mind, 67(266): 166–173.
- ~~Selections from Kenton Rambsy, *The Geographies of African American Short Fiction* (Univ.
  Press of Mississippi, 2022).~~

  [71]: https://courseworks2.columbia.edu/courses/183356/files?preview=18929208
  [72]: https://www-jstor-org.ezproxy.cul.columbia.edu/stable/2251108

### Week 8: Metaphor

- [Metaphors We Live By][82] (1980), pp. 3-52 by George Lakoff and Mark Johnson.
- Chapters 1-7 in [*Illness as Metaphor*][83] (1977) by Susan Sontag.
- "[Why 'Dark Thoughts' Aren’t Really Dark: A Novel Algorithm for Metaphor Identification][84]" in Computational Intelligence, Cognitive Algorithms, Mind, and Brain (CCMB) by Dan Assaf, Yair Neuman, Yohai Cohen, Shlomo Argamon, Newton Howard, Mark Last, Ophir Frieder, and Moshe Koppel.
- Case study: [Computational Paremiology: Charting the temporal, ecological dynamics of proverb use in books, news articles, and tweets][81] from DHQ.

[81]: https://www.digitalhumanities.org/dhq/vol/17/2/000676/000676.html
[82]: https://courseworks2.columbia.edu/courses/183356/files?preview=18955592
[83]: https://courseworks2.columbia.edu/courses/183356/files?preview=18955698
[84]: https://ieeexplore-ieee-org.ezproxy.cul.columbia.edu/abstract/document/6609166/


### Week 9: Syntax

Normalization, stemming, lemma vitiation. Lexical set intersection. Term frequency, inverse
term frequencies.

- Chapter 4, "[Syntax][71]" from the *Linguistics for Students of Literature* (1980) by Traugott Elizabeth Closs and Mary Louise Pratt.
- “[On Sentence-Length as a Statistical Characteristic of Style in Prose: With Application to Two Cases of Disputed Authorship][81],” by G. Udny Yule in *Biometrika* 30, no. 3/4 (1939): 363–90.
- Selections on "Grammar and Syntax," "Syntactic Arrangement," and and "Repetition" from the [*Elements of Legal Style*][72] by Brian Garner. 

  [71]: https://courseworks2.columbia.edu/courses/183356/files?preview=18812007
  [72]: https://courseworks2.columbia.edu/courses/183356/files?preview=19015116

### Week 10: Semantic Roles

Proper names. Named entities. Nouns and objects.

- Chapter 5, "[Symantics: How Does a Sentece Mean?][71]" from the *Linguistics for Students of Literature* (1980) by Traugott Elizabeth Closs and Mary Louise Pratt.
- "Distributed Agency in the Novel" by Dennis Yi Tenen in *New Literary History* (2023).

### Week 11: Discourse

- Timothy R. Tangherlini et al., “[‘Mommy Blogs’ and the Vaccination Exemption Narrative:
  Results From A Machine-Learning Approach for Story Aggregation on Parenting Social Media
Sites][64],” JMIR Public Health and Surveillance 2, no. 2 (November 22, 2016).

### Week 12: Corpus

---
## Formal Methods in Text Analysis II

Style, voice > Chapter > Plot, Narrative, Story > Document > Format > Book > Genre > Discourse > Periodical > Archive > Library

### Week 1: Narrative

Story and plot arcs. Time and events. Authorship and authority.

- Selections from Carolyn Wells, *The Technique of the Mystery Story* (Springfield, MA: Home
  Correspondence School, 1913).
- Boris Eichenbaum, Beth Paul, and Muriel Nesbitt, “The Structure of Gogol’s ‘The Overcoat,’”
  The Russian Review 22, no. 4 (1963): 377–99.
- Selections from Inderjeet Mani, *The Imagined Moment: Time, Narrative, and Computation*
  (Lincoln: University of Nebraska Press, 2010).
  - Teun A. van Dijk, “Discourse Analysis as Ideology Analysis,” in Language & Peace (Routledge,
  1995).

### Week xxx: Authorship and authority

Finding the author. Ways of establishing authority.

- Jolene Galegher, Lee Sproull, and Sara Kiesler, “Legitimacy, Authority, and Community in
  Electronic Support Groups,” Written Communication 15, no. 4 (October 1, 1998): 493–94.
- Paul Rabinow, “Discourse and Power: On the Limits of Ethnographic Texts,” *Dialectical
  Anthropology* 10, no. 1/2 (1985): 1–13.

### Week xxx: Project Workshops

Topics not covered in this class. Change over time. Ways forward. Building models revisited.
Plot, narrative. Readings on vectorization, topic modeling, network analysis.

- Selections from Martin Paul Eve, *Close Reading with Computers: Textual Scholarship,
  Computational Formalism* (Stanford University Press, 2019).

Brainstorm final project in class. Present final project proposals during the second session.
