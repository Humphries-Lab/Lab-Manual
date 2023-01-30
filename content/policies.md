
# Policies

## Scientific conduct

Thanks to the replication and reproducibility crises, and the
ever-growing awareness of the mis(use) of statistics, the scientific
conduct of researchers is more scrutinised than ever. These are our
basic policies for conducting science:

### Experimental data are sacrosanct
We do not alter the content of experimental data. There should
always be a complete, untouched set of any data files we obtain.
Never load the only copy of any data set. Any changes to the
formatting of data (e.g. changing from arrays to tables) are saved
as copies.

### Simulations should be replicable
Every simulation in a paper should be replicable in principle: the
same code run again with the same parameters should produce the same
results. Hint: always save parameters from any simulation code that
will be used for a paper. That includes the random number generator
seed.

### Document your work
Use whatever works for you, but document your work. That could be a
lab book, whether paper or tablet, with notes on each analysis or
each simulation. Or typing notes. Or exporting key plots to
Powerpoint, Google Docs etc. Or using a Jupyter notebook or
RMarkdown to encapsulate what you've done, if you're comfortable
with those things. Do something, so that you can give *accurate*
answers to: what have you been working on? And: what have you found?

### Every file is duplicated
Your computer will die. All working files on your computer should be
replicated elsewhere, at all times. At minimum, use an automated
program to back up to an external hard-drive. Better, use
cloud-based storage - this will also let you sync work across
machines.

### A Just Culture
As scientists we are always learning: about new ways of analysing
data, about our own findings, about new models, about new published
research. And learning is inherently about making mistakes and
errors, in order to correct our skills and knowledge. So the lab
operates a "Just Culture", not a blame culture: mistakes and errors
are expected; mistakes are not blamed on the individual; and
mistakes are used as opportunities for learning by the lab: how to
adjust our approaches to catch errors in the future.

!!! note "An example of Mark's mistakes"

    Chapters 4 and 5 of my PhD thesis contain a spiking neuron model of the
    feedback loop between the globus pallidus (GP) and the subthalamic
    nucleus (STN). As thrilling as it sounds. This is a negative feedback
    loop: the GP inhibits the STN; the STN excites the GP. However, in the
    midst of writing up Chapter 4, I discovered my code had a tiny but
    crucial error: the STN input to the GP had a minus sign in front of it.
    It was inhibiting, not exciting, GP. Already past the end of my funding,
    I had to ditch all the simulations that were to make up Chapters 4 and
    5, and ran them all again from scratch. The lesson for the future: when
    coding connections between neurons, don't write the sign of the
    connection into the arithmetic (`Input = A – w.B`); always write the sign
    into the weights: (e.g. `Input = A + w.B`, and `w = –1`). That way, a quick
    glance down the parameter values at the top of the code will show up any
    errors.


## Authorship

Until we reach that bright future where papers are no longer the de
facto currency of academia, and/or where author names are solely linked
to contributions like film credits, authorship will remain a tricky
subject. Who gets their name on the paper, and where it goes on the list
of authors, can cause problems. Our criteria are simple, and similar in
spirit to the criteria of the [ICMJE] guidelines:

1.  Substantial intellectual contribution to the content of the paper,
    AND

2.  Contribute to the written content of the manuscript in a meaningful
    way \[by contributing text and/or substantial editing; and approving
    the final manuscript\]

[ICMJE]: http://www.icmje.org/recommendations/browse/roles-and-responsibilities/defining-the-role-of-authors-and-contributors.html

The usual model is that the postdoc or PhD student leading the research
project will be first author on publications from that project; and Mark
will be listed as the senior author.

Authorship is open to discussion. Especially when we co-author with
collaborators outside the lab, there will be discussions based on the
balance of contributions, from e.g. the collection of data versus the
analysis of data.

The badge of "corresponding author" can carry weight: it is the author
taking ultimate responsibility for all the content of the paper, on
behalf of all other authors. Typically this will be Mark. But this will
be discussed if it is clear the intellectual contribution of the lead
author merits being the corresponding author.


## Work/life balance

### Working hours
Scientific research is target-based, not hour based. If you are
producing a constant, evident stream of work - dead-ends and all -
then you're doing it right. Core hours for the lab are 10am - 4pm.
All lab meetings will be within those hours.

### Email policy
Turn it off. Keep your focus. We use Slack precisely so that you do
not have to check email to keep intra-lab communications going.
Check your email when you need to use it yourself; or when you have
time to execute on whatever is there. Strongly advise that you do
not have work email on your phone.

### Slack policy
Set notifications to only arrive during core work hours (10am -
4pm). Mark will occasionally send out of hours, as I sometimes have
to shuffle email/Slack around other commitments; and when I remember
stuff that needs sorting. There is no expectation to respond until
the core work hours.

### Holidays
Take some. Take a day off to recharge after intense bouts of work.
Take a week or two off to get away from research. Mark takes a
non-negotiable two weeks off at Christmas, and turns down all
requests for work, reviews, grants etc to do so. It's awesome.


## Behavioural conduct

All lab members are expected to abide by the University of Nottingham's
policies for behavioural conduct. Briefly, these are:

-   [The Dignity at Nottingham policy][1].
    That everyone has a right to work in a positive, supportive
    environment, where harassment and bullying are unacceptable.

-   [Equality and Diversity policies][2].
    That diversity across age, gender, race, culture, physical and
    mental ability, religion are to be celebrated.

[1]: https://www.nottingham.ac.uk/hr/guidesandsupport/complaintsgrievanceanddignity/dignity/dignity-at-nottingham.aspx
[2]: https://www.nottingham.ac.uk/hr/guidesandsupport/equalityanddiversitypolicies/index.aspx
