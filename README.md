My Transition
=============

The starting point of this discussion is how to achieve a society where the below statements would be true (see Resource Based Economy [[RBE](http://www.thevenusproject.com/the-venus-project/resource-based-economy)]):

1. resources must be equally distributed among all people
2. free access to those resources
3. no political system as we know it
4. the political system is replace by a technical one that keeps the balance
5. this system is maintained by everyone that would like to contribute, but it needs no human input to run
6. people strive to accumulate, share, develop knowledge (to be able to contribute)
7. there are no need for laws, except technical ones

If when reading some of the article here you get the feeling that this is impossible, try to ask yourself what should I add to make it possible.
It is all on you.
I know you will not let us down.
You can use your life experience and a [thought experiment](http://en.wikipedia.org/wiki/Thought_experiment) to show that a current socio-economic problem could not work and then propose a different solution. 

#Goals

We would like to use Git as a platform on top of witch we could build a new society.
We are going to build a new society with the use of Latex documents.
Each of them is a transition proposals.
As it is clear now that our socio-economic system is not capable to care for us (the people), we are going to build a new one.
As far as this repository is concern the destination of this transition should be some kind of a system based on a Resource Based Economy [[RBE](http://www.thevenusproject.com/the-venus-project/resource-based-economy)]

### Long term

The best way to use our intelligence is to solve problems.
One of the biggest problem ever seems to be: What we need to do to become a civilized society on a planetary level?
With more fancy words: How to start the process that will lead us to a type 1 civilization [[Kardashev_scale](http://en.wikipedia.org/wiki/Kardashev_scale)]?
But this problem was already solved.
The solution is a RBA.
The true challenge is to synthesize the transition.
The long term goal is to use a distributed version control system the allow the community to express it's own creativity.
Each document (proposal) is a piece of legislation that could/should be considered by politician and one day be passed a law. 

### Medium term

Create and collaborate on proposals that tackle specific socio-economic problems.
Along the way verify if a version control system is the right platform.
We certainly need an uncentralized way of writing law.
There are a lot of similarities between writing laws and software.
The best practice in unsentralized software development is Git.
I believe Git could be the right way to allow millions of people to collaborate in the design of our society.

### Short term

Convince anybody to follow :)

# Collaboration

Politician an politics has deviated so much from reality in the past years that it need a complete overhaul.
Politician are just too few to tackle the complexity of the real world.
We need to drastically increase the number of people involved if we want real change.
At the same time more people could mean endless discussion.
To prevent it we have to realize the we are working for the community and not for our personal gain.
Politician are limited by the small communities they represent.
If we are building it together we would have a greater respect for this new entity the we created.

### Rules

As I do not have control over what people do this should be seen as guidelines:

1. all files are released under licence CC0
1. except rule 1 and 2 everything can be changed
2. keep in mind RBE's philosophy
3. if you think a line of thought is wrong propose a change to make it right
4. currently only two file types are allowed i.e. `*.tex` and `*.bib`
5. when you type text each sentence goes in its own line
6. when you first commit a document you can use your name in the author section.
When you amend a document you should change the author to "The People" (or somthing similar that describes us all).

### File Structure

1. folder `approvals` - here you can put your articles that could be considered as a peace of law that implements the transition.
Something that one day could be turn into law.
2. folder `articles` - an argumented discussion that tries to convince others to participate to this vision.
3. folder `goodies` - solution to some environment issues

### Git

If you are not sure about what are you doing use GitHub pull request to share your work.
If you are sure everything is fine use a direct SSH connection to push your changes (see `goodies/user`)
The remote branches are:

1. `master` - official version
2. `dev` - current public development, to be merged into master at the end of current development iteration after formal collective approval
3. `backdoor` - new document and/or minor (spelling) changes that can be pushed to master  without a formal collective approval
4. `dev-backdoor` - fixes to dev branch needed to get a formal approval.

Each approval folder (e.g. p101) has two extra collaboration files.
They are `approved.tex` and `release.tex`.
In the first one people that did not contribute can leave their approval.
We do that by adding one line to the document and then commit it.
The second one is a document meant to support the release cycle.
The release cycle moves commits form dev to master branch.
File `release.tex` it is wiped out after each release.
The release to master should contain all the approvals (squashed into one commit), the `release.tex` file and all the improvements relevant for that release.

### Environment
What to install on Windows before starting:

1. MikTex (compiles a tex file to a pdf)
2. TexMaker (it provides spell checking, if you do not it just use MikTex for editing documents)
3. Git
