Stats 337, Applied Readings in Data Science (Spring 2018)
================

# Annotated bibliography

-----

### Theme: Blameless postmortems for data science?

### Executive summary

The idea of postmortems to evaluate failure events has long been
considered an important practice for effective risk management. The idea
of blameless postmortems goes further to emphasize the need to create
and facilitate a postmortem process where participants are incentivized
to provide detailed accounts and analyses of what happened without fear
of punishment.

My readings for this annotated bibliography were guided by a desire to
learn more about the idea of blameless postmortems, with particular
attention to how they might be implemented for data analysis errors and
data science issues. I’ve outlined a number of potential reasons that
blameless postmortems may have not yet been widely adopted within data
science practices, as well as some potential suggestions for trying to
encourage this practice.

### Barriers & Interventions to blameless postmortems for data science

While the idea of blameless postmortems have been adopted by many
software engineering and devop teams (with many referring to Etsy’s
process as a model), it seems that blameless postmortems have not yet
infiltrated standard data science practices.

This may be because of a number of reasons, such as the following:

  - Data science is a relatively new field and there are not yet set
    “standard” data science practices
  - The definition of a data analysis success or failure may be more
    nebulous, such that the errors or failures due to data science may
    be less clearly identifiable - contrast this with some of the
    obvious software engineering failures (e.g. cloud service is
    disrupted).
  - There may be less incentives for small data science teams or data
    scientists spread across an organization to prioritize postmortem
    processes and learning over efficiency, and/or they may be in a
    weaker position to establish a culture of blameless postmortems.
  - There are a lack of examples or case studies about blameless
    postmortems as applied to data analysis errors – and likewise, there
    are a lack of templates for conducting these kinds of postmortems.
  - Data scientists may underestimate the degree to which decisions made
    as part of data science practices are subject to human bias and
    error.
  - Changing organizational culture is hard work\! And managing
    blameless postmortem processes effectively may sometimes be
    delicate, and/or require specific training and practice. These
    skills likely lie outside the typical scope of what a data scientist
    thinks their job constitutes.

From this list and from the readings, some thoughts about potential
interventions to accelerate the adoption of blameless postmortems in
data science are the following:

  - Have data scientists create a blameless post-mortem template for
    data science failures within their own organization. Doing so would
    likely catalyze thoughtful and explicit discussions on what data
    science success and failure looks like, as well as help establish
    group norms about what a blameless post-mortem process looks like
    before a crisis forces the issue.
  - If they already exist elsewhere in the organization, communicate and
    learn about the postmortem processes already in-place within
    software engineering groups, etc – and use these resources as
    potential templates for data science postmortems, or if appropriate,
    see if data science postmortems would belong within existing
    processes.
  - Consider when it would be appropriate and/or beneficial to the
    community to make a data science post-mortem public
  - Consider conducting systematic and internally reviewed premortems to
    identify potential risks and human biases before embarking on a data
    science project; revisit and iterate as necessary as the project
    unfolds

Any feedback, thoughts, critiques, additions, welcome\!

### Top 3 articles

**1. [Blameless PostMortems and a Just
Culture](https://codeascraft.com/2012/05/22/blameless-postmortems/).
John** **Allspaw (from Etsy). *Code as Craft* (May 2012).**

*Why you should read this*: If there was a canon of readings on
blameless postmortem, this article would be on it. The article is
relatively short, but lays out the philosophy behind blameless
postmortems in a cogent and persuasive manner and at a digestible pace –
it’s a great way to quickly get up to speed on the ideas as well as the
actions that blameless postmortems involve. As in, John not only
presents simple explanations of key principles from the literature on
risk management and safety (e.g. from Sidney Dekker), but also lays out
concrete steps that Etsy takes to implement these ideas. And it seems
like everyone writing about blameless postmortems links to this article…
so don’t be out of the loop\!

*Winning Quotations*:

  - “So technically, engineers are not at all “off the hook” with a
    blameless PostMortem process. They are very much on the hook for
    helping Etsy become safer and more resilient, in the end.”
  - “We enable and encourage people who do make mistakes to be the
    experts on educating the rest of the organization how not to make
    them in the future.”

**2. [What is a Successful Data
Analysis?](https://simplystatistics.org/2018/04/17/what-is-a-successful-data-analysis/)**
**Roger Peng. *Simplystats* (Apr 2018).**

*Why you should read this*: Maybe this article should come first,
because fundamental to the question of postmortems for data science is
the question: what does data analysis failure look like? What metrics do
we use to identify it when we see it?

This article is a great entry into these questions – you’ll inevitably
push your thinking by observing your own reactions and thoughts in
response to Roger’s proposed definition, which he suggests might be
unsettling (or not\!).

In terms of content: Roger presents a framework with which to think
about the question of success in data analysis, and contrasts his ideas
about “acceptance” and “audience” to other notions such as that of using
internal and external validity as a measure of successful data analysis.
He also brings two critical yet underappreciated points into the
conversation: 1) the importance of considering the context in which an
analysis is performed when trying to evaluate what analysis is
appropriate; and 2) that human nature plays a big role in defining the
success of data analysis.

*Winning quotations*:

  - “Success depends on human beings, unfortunately, and this is
    something analysts must be prepared to deal with.”
  - “When an audience is upset by a data analysis, and they are being
    honest, they are usually upset with the chosen narrative, not with
    the facts per se.”

**3. [Fearless shared postmortems – CRE life
lessons](https://cloudplatform.googleblog.com/2017/11/fearless-shared-postmortems-CRE-life-lessons.html).**
**Adrian Hilton, Gwendolyn Stockman. *Google Cloud Platform Blog* (Nov
2017).**

*Why you should read this*: This is a bit of an oddball reading
suggestion (so maybe that’s reason enough\!). While the motivation for
why teams for Google’s Site Reliability Engineering are thinking about
the mechanics of writing an external postmortem may be obvious, it is
less obvious why data scientists may want to think about the value of
external postmortems. So here are two reasons to read this article: 1)
As the importance and role of data science grows, the likelihood that
data science decisions and failures will affect customers more directly
and obviously may also grow (e.g. think facebook experiments that the
public has pushed back on) – and thus the value of external postmortems.
And 2) this article has a nice section at the very bottom called “A side
note on the role of luck”, which offers something both wise and unique
to most descriptions of postmortem write-ups.

*Winning quotations*:

  - “We have found that, with a combination of automation and practice,
    we can produce a shareable version of an internal postmortem with
    about 10% additional work, plus internal review.”
  - “An internal postmortem assumes the reader has basic knowledge of
    the technical and operational background; this is unlikely to be
    true for your customer. We try to write the least detailed
    explanation that still allows the reader to understand why the
    incident happened; too much detail here is more likely to be
    off-putting than helpful.”

## Bibliography

*Note about citation formats*:

  - Most citations follow the convention used in the GitHub syllabus,
    reverting to a more traditional academic citation format for
    academic publications.
  - Readings are generally grouped by topic and listed in reverse
    chronological order, except for the priority readings which are
    placed first.

**General**

  - [What is a Successful Data
    Analysis?](https://simplystatistics.org/2018/04/17/what-is-a-successful-data-analysis/)
    Roger Peng. *Simplystats* (Apr 2018).
  - Parker H. (2017) Opinionated analysis development. PeerJ Preprints
    5:e3210v1 <https://doi.org/10.7287/peerj.preprints.3210v1>
  - [Why ‘Blameless’ ‘Postmortems’ Can Feel
    Wrong](https://medium.com/@jpaulreed/why-blameless-postmortems-might-feel-wrong-cbeee00d51b2).
    Paul Reed. *Medium* (Aug 2016)
  - [It’s Not Your Fault Blameless
    post-mortems](https://www.slideshare.net/jhand2/its-not-your-fault-blameless-post-mortems).
    Jason Hand. (Jul 2014)
  - Dekker, S., Paul, C., & Hofmeyr, J-H. (2011) [The complexity of
    failure: Implications of complexity theory for safety
    investigations](https://www.sciencedirect.com/science/article/pii/S0925753511000105).
    Safety Science, 49: 939-945.
  - Dekker, S. (2002) [Reconstructing human contributions to accidents:
    the new view on error and
    performance](https://ac.els-cdn.com/S0022437502000324/1-s2.0-S0022437502000324-main.pdf?_tid=a5bf53cb-4092-4a%20be-bbfd-ec56bac96588&acdnat=1528328624_9f90fafde4c783a8175f94bce923aced).
    Journal of Safety Research, 33: 371-385.

**Company case studies**

  - [Fearless shared postmortems – CRE life
    lessons](https://cloudplatform.googleblog.com/2017/11/fearless-shared-postmortems-CRE-life-lessons.html).
    Adrian Hilton, Gwendolyn Stockman. *Google Cloud Platform Blog* (Nov
    2017).
      - This blog posts also points to other great examples of public
        postmortems by [Google Cloud
        Platform](https://status.cloud.google.com/incident/compute/16007),
        [Gitlab](https://about.gitlab.com/2017/02/10/postmortem-of-database-outage-of-january-31/),
        [CloudFlare](https://blog.cloudflare.com/incident-report-on-memory-leak-caused-by-cloudflare-parser-bug/),
        and
        [Honeycomb.io](https://www.honeycomb.io/blog/2017/10/bitten-by-a-kafka-bug-postmortem/)
  - [5 Whys – how we conduct blameless post-mortems after something goes
    wrong](http://code.hootsuite.com/blameless-post-mortems/). Noel
    Pullen. *Hootsuite Development* (2017)
  - [Chapter 15: Postmortem Culture: Learning from
    Failure](https://landing.google.com/sre/book/chapters/postmortem-culture.html).
    John Lunney, Sue Lueder, edited by Gary O’Connor. (2017)
      - [Postmortem culture: how you can learn from
        failure](https://rework.withgoogle.com/blog/postmortem-culture-how-you-can-learn-from-failure/).
        John Lunney, Sue Lueder, Gary O’Connor. *Re: Work* (Apr 2018).
      - Provides an [example
        postmortem](https://landing.google.com/sre/book/chapters/postmortem.html)
        and this [postmortem exercise
        template](https://docs.google.com/document/d/1ob0dfG_gefr_gQ8kbKr0kS4XpaKbc0oVAk4Te9tbDqM/edit)
      - [Google: Engineering excellence requires a “blameless
        post-mortem culture” for fault
        fixing](https://www.v3.co.uk/v3-uk/news/3013962/google-engineering-excellence-requires-a-blameless-post-mortem-culture-fo%20r-fault-fixing).
        Stuart Sumner. V3 (July 2017).
  - [Postmortems at
    Airbnb](https://medium.com/airbnb-engineering/postmortems-at-airbnb-dde936fd7877).
    Ben Hughes. Medium (Oct 2013).
  - [Blameless PostMortems and a Just
    Culture](https://codeascraft.com/2012/05/22/blameless-postmortems/).
    John Allspaw (from Etsy). Code as Craft (May 2012).
      - Dekker, S. & Breakey, H. (2016) [‘Just culture:’ Improving
        safety by achieving substantive, procedural and restorative
        justice](https://www.sciencedirect.com/science/article/pii/S0925753516000321).
        Safety Science. 85: 187-193.
      - [What blameless really
        means](http://www.jessicaharllee.com/notes/what-blameless-really-means/).
        Jessica Harlee (Mar 2014)

**How to run a postmortem debrief and other postmortem resources**

  - [A collection of postmortem
    templates](https://github.com/dastergon/postmortem-templates).
    Dastergon GitHub repo.
  - [What Etsy Does When Things Go Wrong: A 7-Step
    Guide](https://www.fastcodesign.com/3064726/what-etsy-does-when-things-go-wrong-a-7-step-guide).
    John Allspaw, Morgan Evans, Daniel Schauenberg. *Co.Design* (Nov
    2016).
      - [Etsy github Morgue](https://github.com/etsy/morgue)
      - [Practical Postmortems at
        Etsy](https://www.infoq.com/articles/postmortems-etsy). Daniel
        Schauenberg. *InfoQ* (Aug 2015)
  - [A Project Postmortem Toolkit: Apps and Approaches that Help You
    Learn More from
    Retrospectives](https://zapier.com/blog/project-retrospective-postmortem/).
    Genevieve Conti. *Zapier* (Nov 2015).
  - [A Leader’s Guide to After-Action
    Reviews](http://www.au.af.mil/au/awc/awcgate/army/tc_25-20/tc25-20.pdf).
    Headquarters, Department of the Army (Sep 1993).

**Other**

  - [After a Major Cyberattack, Does the Public Deserve an
    Explanation?](https://www.nextgov.com/cybersecurity/2018/06/after-major-cyber-attack-does-public-deserve-explanation/148692/)
    Mitch Herckis. Nextgov (Jun 4, 2018).
      - [The City of Atlanta should publish a blameless post-mortem of
        the ransomware
        attack](https://www.change.org/p/mayor-keisha-lance-bottoms-the-city-of-atlanta-should-publish-a-blameless-post-mortem-of-the-ransomware-attack?recruiter=867558611&utm_source=share_petition&utm_medium=twitter&utm_campaign=share_petition).
        *Change.org petition*. (Mar 2018)
  - [Tool: Foster psychological
    safety](https://rework.withgoogle.com/guides/understanding-team-effectiveness/steps/foster-psychological-safety/).
    *Re:Work*
      - [The Head of “X” Explains How To Make Audacity the Path of Least
        Resistance](https://www.wired.com/2016/04/the-head-of-x-explains-how-to-make-audacity-the-path-of-least-resistance/#.aeio3w645).
        Astro Teller. *Wired* (Apr 2016).
  - [Upserve – Software
    Engineer](https://jobs.lever.co/upserve/ad9b5e26-3118-430c-aeae-d5331c41a5d3)
    – mentioned in the job posting directly as part of what a day might
    look like

-----

#### Articles about “a case for data literacy”

I didn’t go with this topic, but in case this is helpful to anyone…\!

**General:**

  - [Why companies must close the data literacy
    divide](https://www.forbes.com/sites/brentdykes/2017/03/09/why-companies-must-close-the-data-literacy-divide/#75639da369d9).
    Brent Dykes. *Forbes* (March 9, 2017).
  - [Beyond Data Literacy: Reinventing Community Engagement and
    Empowerment in the Age of
    Data](http://datapopalliance.org/wp-content/uploads/2015/11/Beyond-Data-Literacy-2015.pdf).
    *Data-Pop Alliance* (Oct 2015).
  - [Facebook Spawned a Data Crisis. Here’s What We Do
    Next](https://magenta.as/thank-you-facebook-now-suffer-the-consequences-beee86038439).
    Michael Horn. *Magenta* (Apr 4, 2018).
  - Matthews, P. (2016) [Data literacy conceptions, community
    capabilities](http://eprints.uwe.ac.uk/30506/1/ci-journal-datalit-matthews-preprintep16.pdf).
    The Journal of Community Informatics, 12 (3). ISSN 1712-4441
    Available from: <http://eprints.uwe.ac.uk/30506>
      - Helpful framing: four varieties of data competencies including
        research (academic), classroom (secondary education), carpentry
        (practical training), and inclusion (community development).
  - [Becoming Data Literate in 3 Simple
    Steps](http://datajournalismhandbook.org/1.0/en/understanding_data_0.html).
    Nicolas Kayser-Bril. *Data Journalism Handbook 1.0 Beta*
  - [Data Literacy – Quantitative Research
    Part 2](https://uxknowledgebase.com/data-literacy-quantitative-research-part-2-de07607f1127).
    Krisztina Szerovay. *Medium* (May 16, 2018).
  - [Where if Your Organization on the Marketing Data Literacy
    Spectrum?](https://medium.com/aimarketingassociation/where-is-your-organization-on-the-marketing-data-literacy-spectrum-b0988740b9e2)
    Jim Sterne. *Medium* (Apr 9, 2018).
  - [Why Data Science and UX Research Teams are Better
    Together](https://www.mindtheproduct.com/2018/02/data-science-ux-research-teams-better-together/).
    Julie Stanescu. (Feb 7, 2018).
  - [Data literacy: Your data-driven advantage starts with your
    people](https://www.bdcnetwork.com/blog/data-literacy-your-data-driven-advantage-starts-your-people).
    Nathan Miller. *Building Design + Construction* (May 24, 2017).
  - [Why Data Literacy
    Matters](https://data36.com/why-data-literacy-matters/). Gabor Papp.
    *Data36* (Oct 17, 2016).
  - [Why We Should All Be Data
    Literate](http://alistapart.com/article/why-we-should-all-be-data-literate).
    Dan Turner. *A List Apart* (Sep 20, 2016).
  - [Is Design Metrically
    Opposed?](https://www.uie.com/jared-live/transcripts/Is_Design_Metrically_Opposed.html)
    Jared Spool. *Transcript of talk, UXIM Salt Lake City* (Apr 2015)
  - Martin, Elaine R. (2014). [What is Data
    Literacy?](https://escholarship.umassmed.edu/cgi/viewcontent.cgi?article=1069&context=jeslib)
    Journal of eScience Librarianship 3(1): e1069.
    <http://dx.doi.org/10.7191/> jeslib.2014.1069
  - [Data Literacy: Definition, Importance and
    scope](http://epgp.inflibnet.ac.in/epgpdata/uploads/epgp_content/S000021LI/P001449/M021913/ET/1503055537ModuleID-MIL-10-etext-DataLiteracyDefinition,Importanceandscope.pdf).
    Anubhuti Yadav.

**In higher ed:**

  - [Strategies and Best Practices for Data Literacy Education,
    Knowledge Synthesis
    Report](http://www.mikesmit.com/wp-content/papercite-data/pdf/data_literacy.pdf).
    Chantel Ridsdale, James Rothwell, Mike Smit, Hossam Ali-Hassan,
    Michael Bliemel, Dean Irvine, Daniel Kelley, Stan Matwin, and Brad
    Wuetherick. *Dalhousie University* (2015). \* [The Data Literacy
    Disruption: It’s Time to Change the Education
    Mindset](https://medium.com/@sarah_32155/the-data-literacy-disruption-its-time-to-change-the-education-mindset-d0dfcaa0782c).
    Sarah Nell. *Medium* (April 30, 2018).
  - [The importance of data literacy in secondary
    education](https://edexec.co.uk/the-importance-of-data-literacy-in-secondary-education/).
    Executive Education. (Mar 14, 2018).
  - [The importance of data literacy in higher
    education](http://edquarter.com/Article/the-importance-of-data-literacy-in-higher-education).
    Charley Rogers. *edquarter* (Jan 5, 2018).

**For educators:**

  - [Why data literacy training is important, and how I-TECH
    helps](https://edscoop.com/why-training-and-data-literacy-are-important-and-how-i-tech-helps).
    Paige Kowalski. *edscoop* (Oct 30, 2015).
      - [State Progress, Data Quality
        Campaign](https://dataqualitycampaign.org/why-education-data/state-progress).
        *Data Quality Campaign* (2015).
  - [Ethical and appropriate data use requires data
    literacy](https://datafordecisions.wested.org/wp-content/uploads/2015/03/Kappan-Ethical-and-Appropriate-Data-Use-Requires-Data-Literacy.pdf).
    Ellen Mandinach, Brennan Parton, Edith Gummer, Rachel Anderson.
    *Data for Decisions, WestEd* (March 2015)
