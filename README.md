# Course Report Git Post

## What is git and what are its origins?

Have you ever seen a document named something like
`report_final_draft_final(3).doc`?  Keeping track of the changes to a file over
time is difficult but important.

Git is a Version Control System (VCS) -- a tool that helps us to keep track of
differences in a file or collection of files over time. You've likely
experienced less sophisticated version control like features such as Microsoft
Word's undo or 'go back' features that allows you to return to a previously
saved version of a file. Maybe you've created your own version control by saving
drafts of a file with different numbered filenames. Git takes it to the next
level by allowing us to decide exactly when we save a version of a project, and
also provide annotations when doing so. 

You can create versions of a project by making it a **repository** (also called
a 'repo'). A repo is a folder with git tracking turned on, which may contain
files and subfolders ie. a codebase) through a series of **intentional**
snapshots called **commits**. One thing to keep in mind is that Git is most
often used 'locally', which just means on your computer. That is in contrast to
GitHub, which is a website that hosts Git repositories.

[Git](https://github.com/git/git) was originally developed by Linus Torvalds,
while maintaining the Linux kernel (An operating system that runs the majority
of smartphones, tablets, servers, and supercomputers across the globe) in 2005. 

## What is git used for? Can you give some examples?

Git is used for managing the changes to a project over time. A project might be
just a single file, a handful of files, or thousands of files. Those files can
be anything from plain text to images or videos.

Because Git is focused on managing changes, it is often used as a collaboration
tool allowing people to work on the same project at the same time. By tracking
their individual changes, Git can bring everything together to the final
version.

Imagine that you're writing a blog post that has multiple files associated with
it. You may have one main text file which is the actual post, an additional file
for references, as well as some other files that are diagrams and other images.

Without Git, you may have these various files stored in a folder on your
computer, but there is no way to tell where all of the files are at a given
point in time. Imagine you send your post to two friends to copyedit.  How do
you merge their changes back together? Maybe another friend does color
adjustments on a photo in the article. Which file is the original, which is
edited?

With Git you can track the whole repo at various points in time using commits
and provide annotations on why you decided to save the project at that point in
time.  Later, we can browse this history of commits to see a clear history of
our project, and also a means to travel back in that history, if necessary.

A software codebase works just like that blog post. At their most basic level
they are a collection of files that are linked to one another. When a developer
is working on a certain feature, Git provides a means to save a snapshot of the
entire repo via a commit. This is usually done when incremental progress has
been made and a feature is bug-free. In making the commit, the developer can
provide annotations explaining what was changed and why it was changed. This
message adds to the history of the project and can make it easy to determine
when a certain feature -- or even a bug -- was introduced.

## What is Github and what are its origins? How did its creation change the way people collaborate?

GitHub, developed in 2008, is a web application that hosts Git repositories.  
The team that started GitHub saw that Git could solve important problems for
many teams -- but Git itself is often difficult to use. GitHub adds bunch
of collaboration and exploration tools on top of Git to help you (and your team) be more productive.

For instance, GitHub makes it easy to share code
between multiple computers and developers. It's become the centralized organizing
tool of the open source community and, in turn, is used by thousands of companies
and teams. Some GitHub users have one repo they work with every day, some have thousands.

Some of the most important tools GitHub layers on top of Git include:

1. *Pull Requests* which are a way for developers to propose changes and solicit feedback/discussion from other developers (called Code Review).
2. *Issues* which developers use to track bugs, enhancements, or other requests that
   are associated with a given repository.

## How do most developers use Git and Github in their workflow? Can you give some examples?

Imagine I'm working on a project on my laptop at work, once I get to a place
where I'm happy with my progress. I can make a commit and then **push** my repo
up to GitHub. When I get home, if I want to continue adding changes to the blog
post on my desktop computer, I can **pull** it down and continue working where I
left off. I can continue to make commits and push them to GitHub so that my
project is readily available on any computer I choose to work on. Here's a
diagram of what that workflow might look like:

![git and github diagram for commits, pushing, and
pulling](./images/git-and-github.png)

I can repeat the above process with few issues if I'm working on my own.
However, if I decide to pull in a teammate to work with me on a project, we'll
need to incorporate **branching** into our workflow. Branching makes it easier
for us to update the same project simultaneously with limited headaches. If you
want to go down that rabbit hole, [The GitHub
Flow](https://guides.github.com/introduction/flow/) is a good explanation of
what a basic branching workflow looks like. At Turing, we have our students
incorporate a branching workflow starting in module 1, so that they're really
comfortable using that workflow by the time they graduate.

## What sort of companies use Github for their development process?  
### Can you give some examples?  
### How widely used is it?

Both major corporations and small open source organizations use GitHub for their
development process. GitHub makes their revenue on paid subscriptions for
private repositories, which are usually proprietory products. Public
repositories are free for everyone.

Many companies have a mix of both public and private repos as there is a
precedent of open source altruism in software development. For instance,
Facebook has a ton of open source software on GitHub, including the super
popular JavaScript framework, react.

Netflix, Amazon, Airbnb, Google, and IBM are some other popular companies that
use Git and GitHub for source code hosting.

GitHub is by far the most popular Git repository hosting service. As of October
2018, there were 31 million users across the globe with over 96 million
repositories. As of October 2017, GitHub had almost 5x as many users as the next
most popular source code hosting site, Bitbucket.

## What are some alternatives to git and Github?

Some alternatives to Git include Mercurial and Subversion (also referred to as
SVN). Mercurial had a similar catalyst to Git in that it was created by another
member of the Linux Kernel team when they lost access to the proprietary VCS
they were using at the time. SVN used to be super popular, but has lost
momementum in recent years as it's a centralized VCS, meaning that
users must be connected to a central server in order to use it (unlike Git and
Mercurial which are distributed VCSs that require no internet connection, and
most work can be done locally).

## What are advantages and disadvantages of git and Github?

Reiterating the above, one of the major advantages of Git is that it is a
distributed VCS that can be used offline. Another major advantage is that it's
so ubiquitous most other developers have familiarity with it and a lot of open
source projects are hosted on GitHub, so it's a great place to find and
contribute to those projects. GitHub also incorporates 3rd party integrations to
make workflows easier.

The main disadvantage I can think of with both Git and GitHub is that they both
have a fairly steep learning curve.

## Do all developers need to know how to use git or another version control system?

I know some developers that work on teams that don't use version control and it
sounds like a nightmare. Bugs that could be caught using version control sneak
into production and there's no place to conduct code reviews or see
history on the project. I personally can't imagine working on a codebase without
version control and would argue that some VCS competency is a must for any
developer.

## What kind of jobs require knowledge of git and Github? Examples?

Most software development jobs are going to require some knowledge of Git and
GitHub. Other job areas that might require some Git and GitHub knowledge are data
science, technical documentation, project manager, and product manager roles.

## How important is it for beginner coders to learn how to use git?  
### Is this something you learn in a CS degree?

Learning Git will provide beginners with another tool that they'll likely use on
the job so I think it's a great idea. GitHub is also a place where many
prospective employers look at applicants. In being an active Git and GitHub
user, you make it easy for potential employers to see your competency at Git,
programming, and writing technical documentation simultaneously. If I want to
see how someone writes code, the first thing I'll do is check their GitHub
profile. It's going to be a much more honest indicator than Linkedin to see how
someone works as a developer.

Not all CS programs teach Git, but it does seem to be something that more and
more programs are incorporating. I've also been told that it's something that's
never explicity taught but that its expected to be used in some programs.

## How are git and Github incorporated into the Turing curriculum?  
### Why teach Github over another service like Bitbucket?

Git and GitHub are incorporated into the Turing curriculum from day one.
Students are given a lesson during their first module to go over basic
commands and workflow. In later modules they're graded on their ability to
conduct proper pull requests and code reviews during feature development. We
also introduce more complex worflows they may use in their future jobs.

We've taught GitHub from the beginning beacuse GitHub was the first Git repo
hosting service and is also the most commonly used. It has also been fundamental
in making Git more approachable for folks learning it. On a more personal
organizational level, it was built in ruby (the first language that we taught at
Turing) and has been really supportive to the ruby community. The organization
has also been super supportive of us as a non-profit organization by providing unlimited free public and private repositories, and it just so happens that we
have 10 or so alums and/or former teachers who work there.

## How can a beginner get started on learning how to use git and Github?

There are ton of great resources out there for learning Git and GitHub. 

Here's some of my favorites below:
* If you like video tutorials, this is a great one on Git basics: [Git
  Real](https://app.pluralsight.com/player?name=6eec00f4-f910-4efc-9698-936948026502&mode=live&clip=0&course=code-school-git-real&author=gregg-pollack)
* If you have a more kinesthetic learning style, you can check out a code
  academy course that we use as supplementary homework
[here](https://www.codecademy.com/pt-BR/learn/learn-git)
* And for all things GitHub related, check out their [Learning
  Lab](https://lab.github.com) 

## Can you give us a brief bio about yourself, your background, and your experience in tech/teaching?

After doing manual data entry and calculations using excel in previous jobs, I
decided to learn how to program to streamline those processes. I attended the
Turing back end engineering program in 2015 as a student, and quickly realized
that not only could I solve these problems with programming, but I also really
enjoy it.  Before joining Turing as an instructor, I worked at Points of Light
as a full-stack web developer engineering web applications to help people both
organize and find volunteer opportunities in their communities. As an
instructor, I pull from my previous experience and try to never speak in
absolutes. In programming there are few truths and many opinions. When I'm not
at Turing, I enjoy hanging out with my wife and our dog. I also enjoy cooking,
eating, snowboarding, backpacking, hiking, and traveling. 

