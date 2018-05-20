# Stats 337: Readings in Applied Data Science

[Stats 337](https://explorecourses.stanford.edu/search?view=catalog&filter-coursestatus-Active=on&page=0&catalog=&academicYear=&q=stats+337&collapse=%2C2%2C) is a small discussion class available to Stanford students in Spring 2018. Student in this class will read 3-4 papers (or equivalent) per week, write a brief response, and then discuss the papers (and related ideas) in class.

## Readings

These readings reflect my personal thoughts about applied data science, and are skewed towards topics that I think are important but are generally under appreciated. It is not a systematic attempt to survey the field. That said, if you think there's something major that I've missed, please feel free to submit [an issue](https://github.com/hadley/stats337/issues) (or [pull request](https://github.com/hadley/stats337/edit/master/README.md)!). These readings will evolve as the quarter goes by. 

Many of the readings come from [Practical Data Science for Stats](https://peerj.com/collections/50-practicaldatascistats/), a join PeerJ collection and special issue of the American Statistician. Jenny Bryan and I pulled this collection together in order to publish some of the important parts of data science that were previously unpublished. Other readings are blog posts because so much of applied data science is outside the comfort zone of traditional academic fields. 

The development of much of this course has been driven by conversations on twitter. A big thanks go to everyone who has helped me out! Key threads: [classroom discussion](https://twitter.com/hadleywickham/status/964650890593538048), [ethics](https://twitter.com/hadleywickham/status/978712074434957313), [google sheets](https://twitter.com/hadleywickham/status/978401746182549504), [citation management](https://twitter.com/hadleywickham/status/978752525493915648).

### What the *&!% is data science? (Apr 2)

* [Data scientists mostly just do arithmetic and that’s a good thing](https://m.signalvnoise.com/data-scientists-mostly-just-do-arithmetic-and-that-s-a-good-thing-c6371885f7f6);
  Noah Lorang (2016).

* Optional: [Enterprise Data Analysis and Visualization: An Interview Study](https://idl.cs.washington.edu/papers/enterprise-analysis-interviews);
  Sean Kandel, Andreas Paepcke, Joseph Hellerstein, Jeffrey Heer (2012).

* Optional: [50 years of data science](https://www.tandfonline.com/doi/abs/10.1080/10618600.2017.1384734)
  ([OA preprint](https://courses.csail.mit.edu/18.337/2015/docs/50YearsDataScience.pdf));
  David Donoho (2017). This is discussion paper and a number of notable 
  statisticians have contributed commentary. Make sure to read some of these
  as well.

[In-class resources](week-01/)

### Data collection and collaboration (Apr 9)

* [Tidy data](https://www.jstatsoft.org/article/view/v059i10/);
  Hadley Wickham (2013).

* [Data organization in spreadsheets](https://peerj.com/preprints/3183/);
  Karl W Broman, Kara Woo (2017).
  
* [Best practices for using google sheets in your data project](https://matthewlincoln.net/2018/03/26/best-practices-for-using-google-sheets-in-your-data-project.html);
  Matthew Lincoln (2018).

* Bonus: [Modeling as a core component of structuring data](https://iase-web.org/documents/SERJ/SERJ16(2)_Konold.pdf);
  Clifford Konold, William Finzer, Kozoom Kreetong (2017)

[In-class photos](week-02/)


Spend 3-5 minutes filling out [class feedback](https://goo.gl/forms/py92VLLqodxuBU8z1).

### Software engineering (Apr 16)

* [Software development skills for data scientists](http://treycausey.com/software_dev_skills.html);
  Trey Causey (2015).

* [Excuse me, do you have a moment to talk about version control?](https://peerj.com/preprints/3159/);
  Jennifer Bryan (2017).

* [Good enough practices in scientific computing](http://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1005510);
  Greg Wilson, Jennifer Bryan, Karen Cranston, Justin Kitzes, Lex Nederbragt, Tracy K. Teal (2017).

[Collaborative google doc](week-03/google-doc.md)

### DevOps (Apr 23)

* [Opinionated analysis development](https://peerj.com/preprints/3210/);
  Hillary Parker (2017)

* [An introduction to Docker for reproducible research, with examples from the R environment](https://arxiv.org/abs/1410.0846); 
  Carl Boettiger (2014).

* [Machine Learning: The High Interest Credit Card of Technical Debt](https://research.google.com/pubs/pub43146.html);
  D. Sculley, Gary Holt, Daniel Golovin, Eugene Davydov, Todd Phillips, 
  Dietmar Ebner, Vinay Chaudhary, Michael Young (2015).

[Collaborative google doc](week-04/google-doc.md)

### Teaching (Apr 30)

* [The Introductory Statistics Course: A Ptolemaic Curriculum?](https://escholarship.org/uc/item/6hb3k0nz).
  George W Cobb (2007).

* [The democratization of data science education](https://peerj.com/preprints/3195/);
  Sean Kross, Roger D Peng, Brian S Caffo, Ira Gooding, Jeffrey T Leek (2017).

* [Teaching stats for data science](https://peerj.com/preprints/3205/);
  Danny Kaplan (2017).

* [Ten quick tips for teaching programming](http://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1006023); Neil C. C. Brown, Greg Wilson (2018).

### Reproducibility (May 7)

* [Best practices for computational science](https://openresearchsoftware.metajnl.com/articles/10.5334/jors.ay/);
  Victoria Stodden, Sheila Miguez (2014).

* [How rOpenSci uses Code review to promote reproducible science](https://ropensci.org/blog/2017/09/01/nf-softwarereview/); 
  Noam Ross, Scott Chamberlain, Karthik Ram, Maëlle Salmon (2017).

* [A practical guide for transparency in psychological science](https://psyarxiv.com/rtygm/);
  Olivier Klein, Tom Hardwicke, Frederik Aust, Johannes Breuer, Henrik Danielsson, Alicia Hofelich Mohr, Hans IJzerman, Gustav Nilsonne, Wolf Vanpaemel, Michael Frank (2018).
  
* [Lessons Learned Reproducing a Deep Reinforcement Learning Paper](http://amid.fish/reproducing-deep-rl); Matthew Rahtz (2018).

* Bonus: [The Practice of Reproducible Research](https://www.practicereproducibleresearch.org);
  Justin Kitzes, Daniel Turek, Fatma Deniz (2018).

### Ethics (May 14)

* [The Ethical Data Scientist](http://www.slate.com/articles/technology/future_tense/2016/02/how_to_bring_better_ethics_to_data_science.html);
  Cathy O'Neil (2016).

* [Big data, machine learning, and the social sciences](https://medium.com/@hannawallach/big-data-machine-learning-and-the-social-sciences-927a8e20460d);
  Hannah Wallach (2014).

* [A Code of Ethics for Data Science](https://medium.com/@dpatil/a-code-of-ethics-for-data-science-cda27d1fac1);
  DJ Patil (2018).
  
* [An ethical code can’t be about ethics](https://towardsdatascience.com/an-ethical-code-cant-be-about-ethics-66acaea6f16f);
  Schaun Wheeler (2018).

* [Ethical Guidelines for Statistical Practice](http://www.amstat.org/ASA/Your-Career/Ethical-Guidelines-for-Statistical-Practice.aspx);
  Committee on Professional Ethics of the American Statistical Association (2016).

* [Journalism as a Professional Model for Data Science](https://www.brianckeegan.com/2016/02/journalism-as-a-professional-model-for-data-science/);
  Brian C. Keegan (2016)

### Career (May 21)

* [What it's like to be on the data science job market](http://treycausey.com/data_science_interviews.html);
  Trey Causey (2015)

* [Academic job search advice](http://matt.might.net/articles/advice-for-academic-job-hunt/);
  Matt Might (????).

* [Importance of sponsorship](https://robinsones.github.io/The-Importance-of-Sponsorship/);
  Emily Robinson (2018).

* [Imposter syndrome in data science](https://caitlinhudon.com/2018/01/19/imposter-syndrome-in-data-science/);
  Caitlin Hudon (2018).

### Industry

* [Doing data science at twitter](https://medium.com/@rchang/my-two-year-journey-as-a-data-scientist-at-twitter-f0c13298aee6);
  Robert Chang (2015).

* [Engineers shouldn’t write ETL: A guide to building a high functioning data science Department](https://multithreaded.stitchfix.com/blog/2016/03/16/engineers-shouldnt-write-etl/);
  Jeff Magnusson (2016).

* [Using R packages and education to scale data science at Airbnb](https://medium.com/airbnb-engineering/using-r-packages-and-education-to-scale-data-science-at-airbnb-906faa58e12d);
  Ricardo Bion (2016).

* [Data science at Instacart](https://tech.instacart.com/data-science-at-instacart-dabbd2d3f279);
  Jeremy Stanley (2017).

* [.rprofile: Jenny Bryan](https://ropensci.org/blog/2017/12/08/rprofile-jenny-bryan/);
  Kelly O'Briant (2017)

* [Marketing for data science](https://medium.com/indeed-data-science/marketing-for-data-science-a-7-step-go-to-market-plan-for-your-next-data-product-60c034c34d55). Erik Oberg (2018).

### Workflow

* [The plain person's guide to plain text social science](http://plain-text.co);
  Kieran Healy (2016).

* [Open notebook history](http://wcm1.web.rice.edu/open-notebook-history.html);
  Caleb McDaniel (2013).

* Optional: [How to be a modern scientist](https://leanpub.com/modernscientist);
  Jeff Leek (2016).

## Grading

This is a discussion based class so the majority of your final grade will come from your preparation for discussion (weekly 1-page responses, 30%), and your in-class participation (also 30%). This class is not meant to be self-contained, so the final component of your grade will be an annotated bibliography (40%) describing other papers that you read outside of this class. The goal of these assessments is to force you to do things that are in your own best interests, and to encourage you learn helpful workflows that will stand you in good stead outside of this class.

I am not interested in policing excuses so no late responses will be accepted, and absences from class will count as a zero for participation. That said, I also don't want one bad week to affect your final grade, so your lowest two scores from each will be dropped.

### Responses

Each week (after the first week), you need to turn in a 1-2 page written response to the papers that you read that week. The goal of response is to ensure that you've read the weekly readings, thought about them, and connected them to your existing knowledge, interests, and experience. In your response, you should briefly summarise the paper (1-2 sentences to jog your memory when you re-read your notes), and then focus on _your_ response to the paper: How did it make you feel? What questions were you left with? What do you think it got wrong? If you found one of the readings to be particularly thought provoking, feel free to devote your entire response to that paper.

Each response will be graded on the check/plus/minus system. You will get a check if you briefly summarise the readings and add your own commentary. You will get a check-plus if you synthesize the readings, and combine them with outside knowledge/experience. You will get a check-minus if you only summarise the paper. (I will likely evolve these guidelines to be more concrete once I've read a few responses.)

If you're not familiar with reading academic papers (or you want to polish your skills), you might want to read these guidelines from [Jeff Leek](https://github.com/jtleek/readingpapers). I'd also highly recommend that you learn and use a citation management system. Having a system for managing citations is crucial if you plan to write a thesis. If you don't have an existing system, start by reading the advice of [Caleb McDaniel](http://wcm1.web.rice.edu/plain-text-citations.html). 

### Participation

This is a discussion class so your classroom participation is essential. But don't worry if you're an introvert, shy, or English is your second language: there will be plenty of opportunities to participate that don't require verbal agility. In this class, I'll be drawing on the techniques described in [The Discussion Book](http://a.co/dar4MT1) by Stephen D. Brookfield and Stephen Preskill to make sure that everyone gets a chance to participate. I'll also collect regular feedback to make sure that everything is going well.

### Annotated bibliography.

Your final project will be an annotated bibliography containing at least 20 papers or blog posts related to data science that we did not cover in this course. (See [citation tracing](http://www.raulpacheco.org/2018/02/forward-citation-tracing-and-backwards-citation-tracing-in-literature-reviews/))

Due June 6 (electronically)

There are three components to the bibliography:

* Executive summary (25%). Introduce the overall theme of your bibliography in 1-2 
  paragraphs. Then use 1-2 pages to synthesise the most important or interesting 
  from your annotated bibliography.

* Top 3 (25%). List the three papers that you would most highly recommend and
  describe briefly why.
  
* Bibliography (50%). List all the papers you have read with a proper reference
  and any notes you find helpful.
  
Each component will be graded 1 (C), 2 (B), or 3 (A):

* Executive summary: 
  * 3: 
  * 2:
  * 1:

* Top 3:
  * 3: Your description of the top 3 papers makes me want to run out and
    read them immediately, and you make that easy with impeccable citations
    and links to pdfs
  
  * 2: 
  
  * 1: You have listed 3 papers and briefly described why they are interesting.

* Bibliography:
  * 1: 6-10 papers
  * 2: 11-16 papers
  * 3: >25 papers

## License

<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.
