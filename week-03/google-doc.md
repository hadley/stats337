---
title: 'Stats337: Software engineering'
---

# Working well with others

## How do I get senior advisors on board with using these tools / best practices? (SZ)

-   Investigate existing practices and identify areas that can be benefited from automation
-   Then create some sort of quantitative metric for time and resources saved by adopting version control tools
-   -   Maybe show them the results... (For example, showing them the output of profvis when you talk about how you went about optimizing your code.)
-   Show them the article?
-   Organize a meeting/skillshare to make team transition seamless(ish)
-   Seems like there is room for "transition" tools... i.e. which allow you to use these tools + in parallel generate more traditional formats to share (natural gas as a transition fuel out of fossil fuels)
-   There's a good paper by Adam Grant on how to get organizations to collaborate on quasi-experiments. Maybe this can be applied to version control too:

<!-- -->

-   <http://journals.sagepub.com/doi/pdf/10.1177/1094428108320737> 
-   (Page 674-678)

## How do you get collaborators on board with tools like Github?

In cases where there are significant barriers to collaborator buy in (e.g., working with government, where individuals might not even be authorized to use platforms like Github), is it worth using these kinds of tools for collaboration? (Autumn)

-   Frame it as time saving / cost cutting / in terms that your superiors will understand.
-   Often not worth the effort (if it is just for document editing, much easier to just use emails -Aaron)
-   If I'm the project statistician, then I think it could be relatively straightforward, because my collaborators will care more about the output I'm producing than the tools and code I'm writing. So if they can see the output on GitHub, they'll probably be happy.

# Teaching/learning

## What is the best way to learn best practices in a classroom setting? (Emily)

-   Team teaching / small groups work well.
-   Forcing yourself to use it on a project, perhaps one of smaller or medium stakes, has been the best way for me.
-   Seeing other student's work and asking those who did something you admire.
-   Beyond the basic, coaching small teams
-   Seeing other people\'s code makes people comfortable and opens up new approaches

## 

## How to move an existing course to GitHub

(I've got my R Markdown files, homework assignments in Latex, and some data sets in Excel, csv, and txt)? Where do I best start transitioning stuff?

-   Bill mentioned that Hadley might have some good resources on this

## 

## What are people's best practices for how you stay on top of new developments? (can I second this?)  - specific examples / recs?

-   RStudio newsletter
-   Twitter

<!-- -->

-   Any good accounts to follow?

<!-- -->

-   \@rstudiotips
-   \@hadleywickham (+1)
-   \@treycausey
-   \@vsbuffalo
-   \@jakevdp
-   \@randal\_olson
-   \@jeremystan
-   \@luispedrocoelho
-   \@seantaylor
-   \@dataandme

<!-- -->

-   How to prune?

<!-- -->

-   code mentors (+4)

<!-- -->

-   How active is this mentorship?

<!-- -->

-   Stanford Stats 337
-   Reading the scientific computing literature/blogs/news websites
-   <http://rweekly.org/> --- particularly the weekly highlights
-   [Rbloggers](https://www.r-bloggers.com)

## How to learn new features of git incrementally?

-   https://www.atlassian.com/git/tutorials

<!-- -->

-   Maybe as they come up?

I've heard Make mentioned a few times - any resources on learning this?

## \^Relatedly how do you implement widespread education of best practices for data science across disciplines (not just establishing opportunities but convincing people to take advantage of them). (Autumn)

-   I think it always has to start with showing people how much value it can bring to them (cost, time savings, etc.).

## How and when did you all learn e.g. version control?  (community poll... might be interesting to see years too)

-   Learned subversion doing research in undergrad. Learned git working in industry.

<!-- -->

-   +1 to undergrad research project
-   What is subversion? Hadley: it's one of the precursors to git

<!-- -->

-   Learned version control (git) in undergraduate coursework
-   Got much much better at git from being the only person on a team who knew anything about git (turns out when you have to step up, you can learn a lot from the interwebs!)
-   Grad school (first quarter), in an intro grad programming course (x3)
-   Final projects in undergraduate class
-   On my own, probably through a MOOC
-   Internship
-   In conjunction with back-ups of my computer files (also learned subversion first, then Git)
-   DCL- 2017 (+1)
-   CS107 (+1)
-   Data Science course in undergrad, and then just reading blogs/tutorials online out of self interest
-   On my own in \~2015, got much better at it while working with a team in an internship in 2016

# Investment

## 

## How do you decide when it's worth it to use higher cost tools like writing tests or github etc?

At a topline level - the benefits of implementing these tools should outweigh the costs.

Here are some ways to think about answering this question:

-   Do you care about version control? If you don't care... probably not worth it.
-   How long are you spending on the project, vs. how long are you spending on overhead?
-   How long did it take to diagnose this problem? How likely is it to come up again?
-   Does future you want to collaborate with past you?

<!-- -->

-   Will you be grateful later on that you documented process?
-   Will you need to leave and come back to it?
-   Are these valuable thinking processes or reasonings that aren't captured in the final output?

<!-- -->

-   Are you working with other people on the project?  If you are...

When shouldn't you take these up? Or why isn't my grocery list on github?

-   Fixed costs and maintenance costs.
-   How long will you be spending on the project?
-   Don't have any knowledge of how to use version control, or someone you want to work with doesn't have any knowledge of version control

## What are the benefits to implementing best practices?

-   General

<!-- -->

-   If your project is becoming sufficiently complicated that you're having trouble staying organized
-   I think I might start using it more for projects/studies I aim to publish: just seems like it can save me time and headaches when the reviewer comments are coming in and I need to go back to the analyses and do more/change things
-   If I think that I'll have the opportunity (or will create the opportunities) to share the results with people who appreciate these practices - generating opportunities for recognition is helpful motivation
-   I think even for your "future self" GitHub seems like a worthwhile upfront investment in terms of saving time and reducing confusion.

<!-- -->

-   GitHub

<!-- -->

-   GitHub for a project seems almost always worthwhile (if format is compatible)

<!-- -->

-   Doesn't have to be a collaborative project for it to be useful

<!-- -->

-   Github seems worthwhile when people you may collaborate with have existing workflows for processing/wrangling data that you also want to leverage. This can help ensure data consistency across analyses where multiple people want to work with the same data.
-   BitBucket is another option, especially if you would rather use mercurial

<!-- -->

-   Writing tests / documentation

<!-- -->

-   Documenting: when the thinking isn't clear from the output
-   In terms of tests: if you think it's possible you could break your code when you're working on it, once something works and you spent more than a bit getting it to work (ex. hours vs. minutes)
-   Tests are useful to make your code "fail fast" in the sense that you can catch errors at their source, which makes debugging a lot easier. If you find yourself looking at your log and not knowing where down the pipeline errors occur, you might find testing useful
-   Assertions

## A lot of my work is (essentially) solo, or just collaboration with my advisor. Should I still use git? I don't personally find it that beneficial in non-collaborative projects.

-   \^I've had this same experience working in industry as the only data scientist on a team. There are sometimes unanticipated collaborative efforts that need my prior analyses for other teams, but this is hard to anticipate
-   Yes! (or some other VC system - no real benefits over subversion for solo work) It is hugely advantageous in ways you don't realize until you start using it. It gives you a lot more flexibility in working with your code, and making changes that could potentially break things without having to worry about getting the system back to a working state.
-   I have found it very helpful for small-scale projects for self-documentation, versioning/the ability to rollback changes, and the ability to test out new direction on branches without committing to that direction.
-   Can be more easily transitioned into a portfolio if you need to demonstrate your work or skills in/for future settings
-   I think it is extremely helpful solo! I use it solo most of the time for the version control aspect!

## How do you build your utility library? How do you distribute? (Aaron)

-   Docker!!!

# Patterns, smells and refactorings

Pattern = identify what is wrong (smell) and then fix it (with a refactoring).

Having written a lot of code, how can I extract the common patterns?

How to identify when it worthwhile to do the right thing?

What are common problems?

-   systematically exploring hyperparameter tuning
-   managing 100s of files
-   copying and pasting code --- time to write a function?

## There are a set of standard design patterns for software engineering. Is there something analogous for data science? (Alex) +1

-   Exploration versus fixed question
-   Single data set versus multi data set

## What are data science "code smells"? What are common data science refactorings? (Hadley)

-   Smell: Repeated code (Aaron)
-   Refactor: vectorization of loops in R (Aaron)
-   Smell: Hard-coded elements within functions
-   Smell: Significant varied table shaping --- "letting the horse win"
-   Smell: Long (100+ line) functions
-   Smell: Places in the code with many nested indents and loops (\~4+ levels deep) refactor by taking some of these blocks into their own function.
-   Smell: Variables that do not have clear meaning from their name
-   Smell: long files  (or all code in one long file)

# Other

-   

<!-- -->

-   

## What is the best way to manage modeling workflows & versioning?

This is different from just software versioning since you need to version input and output data, and may need to be running multiple models at the same time to do parameter sweeps or try out different options. I've seen systems built on Make, and built my own, but it seems like there should be more about best practices here. (Aaron)

## Out of all the best practices listed, are there criteria that we can use to assess which is best suited for particular situations?

-   Does it make your life or your collaborator's life easier?
-   If hard to assess the above, was it recommended by someone doing something similar to you?

## Related to the previous question, what tools exist to manage data and analyses that are proprietary (e.g., company-owned in a consulting setting) or otherwise subject to sharing and identifiability restrictions?

-   I think git can work on local servers as well? \<\--Yes (Yup! Have done this, you install git locally and don't link it to GitHub)

## How do you write word documents for projects with collaborators?

-   [Overleaf](https://www.overleaf.com/) (like Google Docs for Latex) (X3)

<!-- -->

-   It has lightweight version control options too!
-   And preformatted templates for lots and lots of journals!
-   And rich-text/WYSIWYG editor for those unfamiliar with Latex

<!-- -->

-   Sharelatex
-   Google Docs...?
-   Word + dropbox
-   TexMacs is a great WYSIWYG for solo latex work

## How to handle backwards compatibility with your personal utilities library? (Nick)

-   I think someone mentioned Make
-   I use something called Docker...
-   What is in your personal utilities library? I want to hear more about this!

## There are lots of mentions of Docker. It seemed like it was a bit much for most analysis workflows. Maybe I'm wrong? What are people's use cases for this? Are people using it in academics on a regular basis? (Aaron)

-   Looks like we actually have readings on Docker next week... \*angel emoji\*

## Who should be responsible for teaching data scientists how to use best practices? Schools? Industry? The individual? \[Eli\]

-   If there are data science courses at schools, they should at least try to teach best practices.
-   I think it should always be the individual.... Every organization is different\...

# GLOSSARY

## Code Smell

Any symptom in the source code of a program that possibly indicates a deeper problem

Pattern

## 

## Docker

![](https://lh6.googleusercontent.com/BjD4Plk7dE3WBne1xPzgCzdZuv0bodItOGTR0AvCa38EqxDxTmUlEPRy1uMG7MnCWrD3kybrm0DcrMa0pR6jGN06Gkzt1DUP8yPBs8ENmUVfSx5jvPfoqbIrolXGs07PehqUZt7T)\<- That is not helpful :( (+1 even though it's really cute!)

## 

## Make

A Unix utility to automate processes. You specify dependencies, and when something become out of date, a specified action is taken, such as compiling code or running a script.

## Unit test

Contained code that is used to test whether your "production" code is working as intended. It is primarily used in the world of software engineering, where functions should have deterministic outputs based on the inputs, but is less well-defined in data science, where there may not be deterministic outputs, due to randomness in the algorithm, changing data, etc.

## Utility library

A collection of functions that you find yourself using across many projects.

## \~\~ this is fun and oddly soothing \~\

![](https://lh4.googleusercontent.com/cI4GH1qfUs9QZ8msgTSm8GXJpsgwRXW0RyC0JW7zwup0ixyXCcoelBwh-V8v0JYSlLJt-1pY_7qfcwQQ59M1szIiptd1-xWI7_e6DAITNCxOjbVWEeEejyXUDVUZyyVx3vWzhdfo)
