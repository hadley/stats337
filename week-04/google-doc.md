---
title: 'Stats337: DevOps'
---

# Questions

How can we map the idea of 'technical debt' onto statistical analyses? (++++++)

-   Run time can be one way?
-   A related question could be: how do we think about quality control in the context of statistical analysis?
-   Can't it also be in terms of how much work you're going to have to put in later?
-   Possible definition: if the input data changes slightly, how long would it take to re-do the original analysis? (+)
-   HW: Another possible definition (more DevOps-y): if your computer was destroyed, how long would it take you to recreate the analysis?

What is DevOps, and how is it different from software engineering? (++++++)

-   Basically same: Is there an agreed upon/decisive definition of DevOps philosophy? (++)
-   I would argue that DevOps is a subset of software engineering. Basically, DevOps engineers are folks who support the infrastructure and systems for the software developers to do their work. For instance, if you need to deploy a piece of software into Amazon Web Services, DevOps engineers are usually the ones who will set up the permissions, databases, etc. for the developers.

<!-- -->

-   So DevOps sets up the architecture / structure within which (or on top of which?) software engineers build things? (the distinction is still not clear to me)

<!-- -->

-   HW: I'd say the philosophy of DevOps is to automate everything. "If something is worth doing, it's worth automating"

<!-- -->

-   I think there's also a piece of efficiency too

<!-- -->

-   This series of posts cleared things up for me: <https://blogs.msdn.microsoft.com/buckwoody/2017/11/02/devops-for-data-science-who-needs-it/> 

Do you know of any examples (e.g., repos, live videos) of great data analyses? Preferably something where you could see a bit of someone's workflow (+++++)

-   Basically same Q: Is there something like [this](https://www.practicereproducibleresearch.org/) for data science generally? Case studies or process bios would be really helpful to make DevOps thinking more tangible.
-   Examples:

1.  <https://towardsdatascience.com/napoleon-was-the-best-general-ever-and-the-math-proves-it-86efed303eeb>
2.

-   HW: I made this youtube video of me doing a basic data analysis: <https://www.youtube.com/watch?v=go5Au01Jrvs> 
-   HW: More historical, and more focussed on visualisation (rather than data science): <http://stat-graphics.org/movies/>. But neat to see state of the art in (e.g.) 1970s (+)
-   Data and replication code of a researcher here in stanford: <http://www.equality-of-opportunity.org/data/>

How can one develop unit tests to catch statistical bugs rather than programming bugs? (+++++)

-   In the ML technical debt paper, the author recommends checking that the average of the predicted values matches the population average value. (This is somewhat specific to prediction settings.)
-   HW: I think there's no analogy to lab experiments where you might have positive and negative controls for every experiment.
-   You can generate synthetic data and do basic sanity checks.

How is 'technical debt' measured in CS? Lines of code? (+++)

-   HW: I'm not aware of any precise measures; it's more of a metaphor than a specific analysis technique.
-   Code run-time is one way in which technical debt is measured in CS. If you install bunch of packages that are not useful / have codes that are not used, then you'd have higher run time than if your code were efficient.
-   Other general things to look for:

<!-- -->

-   indentation counts (high levels of indentation might indicate overly nested loops which make the code very complicated)
-    file churn (how often some files are changed)\--if some files are changed a lot by many people, that might signal that the files should be refactored into more modularized components with more specific functionality
-   function/method lengths/number of lines (degree of decomposition)

For people who have used Docker \-- what were your original use cases specifically and did you ultimately find Docker to be the best solution for your problem? (trying to figure out if it's worth learning) (++) What created the impetus for you to learn Docker? (++) For people who have tried to use Docker, what did you decide to go with instead? (+)

-   HW: I used it to recreate a package build failure that I had on travis. The only way I got it working was carefully following the instructions in <http://www.jimhester.com/2017/10/13/docker/> 
-   I tried to use it on order to play around with a neuroimaging analysis pipeline w/o having to install all of the dependencies, but ran into some snag setting it up, and didn't find it worth the time to troubleshoot.

DevOps thinking seems most helpful for large-scale collaborative analysis projects. Is it that necessary for much smaller-scale or short-term projects? (+)

-   I think automated testing and infrastructure as code are just as important for ensuring accuracy and reproducibility in small-scale projects. Continuous integration and deployment, performance monitoring, load testing... probably not.

Do you generally read research articles like this or do something else (e.g., read the docs / tutorials) to learn new technologies like Docker? (+)

-   HW: papers are often good if you can find them because they'll survey a bunch of the field, and give cohesive recommendations; but very new technologies will not have papers yet

<!-- -->

-   I search for tutorials
-   I generally search for tutorials or check out blogs that I like (I find tutorials more useful than academic papers to learn a new skill).
-   Generally prefer tutorials
-   I think a better way of thinking about Docker is that it's an implementation of what's called containers. You can just read up on containers instead. AWS has a good background on this stuff.

What is a good source to explain modular code and how to use it in social sciences? (+)

-   <https://www.datacamp.com/courses/writing-functions-in-r>

<!-- -->

-   Not that. I mean, something like to use that in the workflow of your data analysis.

Are there any best practices related to software engineering/DevOps that haven't been in the readings that anyone thinks are important to keep in mind? (++)

-   Comment generously to communicate what the code is doing
-   This is kind of besides the point but a big part of what DevOps folks do is to keep down the spend on servers, etc. so there's almost an implicit cost-saving aspect to DevOps work -\> perhaps this relates to the concept of debt (though it's literal in this sense).

How do you implement code review in your current setting? Are there lightweight versions you could recommend? (++)

-   I use it in a teaching setting every day as people learn new packages / software in R. I've found it useful to have a set curriculum (e.g., practice problems from a book), and use code review to debug problems that everyone has worked on in a weekly meeting or something like that

<!-- -->

-   Is this done in github?

Have you tried reproducing someone else's analysis before? What were the obstacles you faced? (+)

-   Didn't have the pipelines they used to produce their dataset

<!-- -->

-   Similar: didn't have script showing what manipulations they did to the data before running analysis and couldn't reproduce analysis even with analysis code (+) (same)

<!-- -->

-   Didn't have their code (just had results) and wasn't sure exactly what analysis was run
-   Tried reproducing someone's analysis and found that their experimental display code wasn't close to functional, so lost faith in the published paper. Probably should have contacted the authors, but didn't care enough. Did model my analysis of the reproduction with their code though. Lots of hacky manual bits with no explanation.
-   No idea what the columns in the dataset were
-   Related to this question, has anyone been able to find a GitHub repo that has data + code for a project? Kind of creepy but might be an interesting idea to download everything and see if you get the same results

POLL. Let's assume that researchers made their code and data available.

What percent of studies do you think would contain errors in the code?

-   Probs high (+++)

What percent of errors would change the analytical outcome (small or large)?

-   Probs somewhat less high, since manual testing and convergent results are common. But depends how upstream the error is. Simulating synthetic data FTW.

What percent of errors would change the direction of the analytical outcome? \[do we think that people's willingness to support process changes in their field correlates to their predictions?\]

-I think that if transparency and reproducibility were required, there probably would be far fewer errors in published studies. 😶

# Glossary

Virtual Machine: Software to run one operating system on top of another, such as running Windows on a Mac. Can be used to distribute configured software.

eta(?)-Features from the Sculley piece

Provisioning tools
