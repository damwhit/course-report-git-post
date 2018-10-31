# Course Report Git Post

## What is git and what are its origins?

Git is a Version Control System (VCS). That may sound super fancy and technical,
but it's really just a tracking tool that allows us to keep track of differences
in a file or files over time. You've likely experienced less sophisticated
version control like features such as Microsoft Word's undo or 'go back'
features that allows you to return to a previously saved version of a file.  Git
takes it to the next level by allowing us to decide exactly when we save a
version of a project and it allows us to provide annotations when doing so. We
create versions of a project by making it a **repository** also commonly
referred to as a 'repo' (A folder with git tracking turned on, which may contain
files and subfolders ie. a codebase) through a series of **intentional**
snapshots called **commits**. One thing to keep in mind is that Git is most
often used 'locally', which just means on your computer. That is in contrast to
GitHub, which is a website that hosts Git repositories.

Git was originally developed by Linus Torvalds, while maintaining the Linux
kernel (An operating system that runs the majority of smartphones, tablets,
servers, and supercomputers across the globe) in April of 2005, because his team
lost free access to the proprietary VCS they were using at the time. It is an
actively maintained open source project that can be found on GitHub
[here](https://github.com/git/git).

## What is git used for? Can you give some examples?

Git is used for logging the history of a project over time. It provides a way to
save multiple files and folders associated with the same project all at once,
instead of individually. It also provides a way for people to work on the same
project and files at once with minimal issues.

Imagine that you're writing a blog post that has multiple files associated with
it. You may have one main text file which is the actual post, an additional file
for references, as well as some other files that are diagrams and other images.

Without Git, you may have all of these various files stored in a folder on your
computer, but there is no way to tell the status of all of these moving pieces
at different points in time. With Git we can track the entire repo at various
points in time using commits. When we get our blog post to a good place, we are
able to save every file at once by making a commit, and provide annotations on
why we decided to save the folder at that point in time. Having all of these
commits provides a clear history of our project, and also a means to travel back
in that history, if necessary.

You may think that a blog post is a bad example, however codebases are really
aren't that different. They are at their most basic level, a series of text and
image files that are linked to one another. When a developer is working on a
certain feature, Git provides a means to save a snapshot of the entire repo via
a commit. This is usually done when incremental progress has been made and a
feature is roughly bug free. In making the commit, the developer can provide
annotations around the what and the why the feature was built. This message adds
to the history of the project and can make it easy to determine when a certain
feature or bug was introduced.

## What is Github and what are its origins? How did its creation change the way people collaborate?

GitHub, developed in 2008, is a website that allows us to host Git repositories
on the internet.  This is super useful in that it allows us to share code
between our own computers seemlessy as well as with other developers. It's
exponentially easier to contribute to open source software as most open source
projects are hosted on GitHub.  For example, if you want to propose changes to
some source code or add documentation for react js, today, you can do so.

It has also added features to Git through it's interface that are an essential
in most team workflows. Features include, but are not limited to:
1. pull requests, which are a place where developers can propose changes to a
   codebase and where most code discussion and review happens.
2. issues, which allow people to list bugs, enhancements, or other requests that
   are associated with a given repository.

## How do most developers use Git and Github in their workflow? Can you give some examples?

Imagine I'm working on a project on my laptop at work, once I get to a place
where I'm happy with my progress. I can make a commit and then **push* my repo
up to GitHub. When I get home, if I want to continue adding changes to the blog
post on my desktop computer, I can *pull* it down and continue working where I
left off.

I can repeat the above process with few issues if I'm working on my own.
However, if I decide to pull in one of my team members to work with me on the
project, we need to incorporate ****branching** into our workflow. **Branching**
makes it easier for us to update the same project simultaneously with limited
headaches.  The master branch is typically the one that should remain bug free
throughout the duration of a project. Therefore, most of the time developers
work on feature branches and use pull requests to update the master branch with
their changes.

Most developers follow a similar workflow to:

1. Create local branch
2. Write some commits within local branch
3. Push to Github
4. Create Pull Request explaining changes that branch contains and have team
   members conduct a code review
5. Merge to master once changes are approved
6. Pull down new master commits locally
7. Repeat

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
momementum in recent years as it is a centralized VCS, which means that it's
users must be connected to a central server in order to use it (unlike Git and
Mercurial which are distributed VCSs that require no internet connection, and
most work can be done locally).

## What are advantages and disadvantages of git and Github?

Reiterating the above, one of the major advantages of Git is that it is a
distributed VCS that can be used offline. Another major advantage is that it's
so ubiquitous most other developers have familiarity with it and a lot of open
source projects are hosted on GitHub, so it's a great place to find and
contribute to those projects. GitHub also incorporates tooling to make it easier
for teams to incorporate things like kanban tracking or continuous integration.

The main disadvantage I can think of with both Git and GitHub is that they both
have a fairly steep learning curve, where some command and features are not
super intuitive.

## Do all developers need to know how to use git or another version control system?

I know some developers that work on teams that don't use version control and it
sounds like a nightmare. Bugs that could be caught using version control sneak
through to production and there is no place to conduct code reviews or see the
history of the project. I personally can't imagine working on a codebase without
version control and would argue that some VCS competency is a must for any
developer.

## What kind of jobs require knowledge of git and Github? Examples?

Most software development jobs are going to require some knowledge of Git and
GitHub. Other jobs that might require some Git and GitHub knowledge are data
science, technical documentation, project manager, and product manager roles.

## How important is it for beginner coders to learn how to use git?  
### Is this something you learn in a CS degree?

Learning Git will provide beginners with another tool that they'll likely use on
the job so I think it's a great idea. GitHub is also a place where many
prospective employers look at applicants. In being an active Git and GitHub
user, you make it easy for potential employers to see your competency at Git,
programming, and writing technical documentation simultaneously. If I want to
see how someone writes code, the first thing I'll do is check their GitHub
profile.

Not all CS programs teach Git, but it does seem to be something that more and
more programs are incorporating. I've also been told that it's something that's
never explicity taught but that its expected to be used in some programs.

## How are git and Github incorporated into the Turing curriculum?  
### Why teach Github over another service like Bitbucket?

Git and GitHub are incorporated into the Turing curriculum from day one.
Students are given a lesson on both during their first module to go over basic
commands and basic workflow. In later modules they're graded on their ability to
conduct proper pull requests and code reviews during feature development. We
also introduce more complex worflows they may use in their future jobs.

We've taught GitHub from the beginning beacuse GitHub was the first Git repo
hosting service and is also the most commonly used. It has also been fundamental
in making Git more approachable for folks learning it. On a more personal
organizational level, it was built in ruby (the first language that we taught at
Turing) and has been really supportive to the ruby community. The organization
has also been super supportive of us as a non profit organization by providing
free unlimited public and private repositories, and it just so happens that we
have 10 or so alums and/or former teachers that work there.

## How can a beginner get started on learning how to use git and Github?

There are ton of great resources out there for learning Git and GitHub. 

Some of my favorites are:
* If you like video tutorials, here is a great one on Git basics: [Git
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
not only could I solve those problems, but I also really enjoy programming.
Before joining Turing as an instructor, I worked at Points of Light as a
full-stack web developer building web applications to help people both organize
and find volunteer opportunities in their communities. As an instructor, I pull
from my previous experience and try to never speak in absolutes. In programming
there are few truths and many opinions. When I'm not at Turing, I enjoy hanging
out with my wife and our dog. I also enjoy cooking, eating, snowboarding,
backpacking, hiking, and traveling. 

