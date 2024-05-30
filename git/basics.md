# Getting started with Git

This short guide will get you up and running with what Git is and how to use it.

## What is Git?

Git is a version control system. It's main goal: to track different versions of files. It records what changes were made, like new files, deleted files, or altered lines in a file. It also tracks who made the change, and when they made the change. 

While Git isn't the only source code version control software used, it is by far the most popular. It's free and open source, fast, and extremely powerful. It's also the technology used to power popular cloud source code control services like GitHub, GitLab, BitBucket and more.

As a fun tidbit, the creator of Git is none other than Linus Torvalds, the creator of the Linux operating system.

## What problems does Git solve?

Complex coding requires thousands, tens of thousands, or even [millions of lines of code.](https://informationisbeautiful.net/visualizations/million-lines-of-code/). At one of my jobs I worked on a single Java file with 20,000 lines of code! The rest of the Java program had 10's of millions of lines of code in total. Yeah, it's a lot.

Imagine a developer making a small, single character change to one of those millions of lines of code. Months, or even years later, a critical bug is discovered in the application. How would you know what change caused the bug? And how would you know who made it, and when? If you were using a version control system, this becomes much simpler. 

Beyond bugs, version control helps developers on a day-to-day basis. Imagine working on a team of developers to add new features to a company webpage. You add the text boxes and form inputs, and simultaneously your co-worker adds the logic to perform a filter on the page based on those UI inputs. When it comes time to connect the two changes together, how do you ensure you don't overwrite some of each others changes? Once again, version control systems take care of this.

Here's an example that might feel familiar to your own experiences. Have you ever worked on a group project in school that utilized Google Docs? Google Docs is a web-based word processing tool that allows multiple users to edit the same document in real time. This can be really handy for collaboration. You can add a paragraph to the project, and your buddy can edit or remove that paragraph all together at the same time, later that day, or months later. 

What happens if multiple classmates edit the same paragraph? Which version becomes the final version? What if you wrote something you really like, but your classmate overwrote it (even unintentionally) with their own words? Google docs has a version history system (sound familiar?) that takes snapshots of the document at a given time when an edit is made. This takes who made the change, what the document looked like at the time, and when it was made. You can even easily revert back to a previous version and get back to your erased essay. 

Git works like this, and so much more. It's precise - you can't sneak even a spare space in a file without it tracking it, and forcing a reconciliation with a conflicting version. 

## Who uses Git?

Short answer: pretty much every company that develops code. 

This is in-part because of how well designed and feature rich Git itself is, but also because of the popularity of enterprise cloud-based Git solutions like GitHub and GitLab. 

So, it'll pay to get to know it well. You'll use it everyday. And the companies I talk to that hire students like you want you to be good at it.

## How do I get started using Git?

The basic steps to getting started using Git are:
1. Install Git locally on your computer. [download git here](https://git-scm.com/downloads)
2. Create an account on [GitHub](https://github.com/) to remotely track your code (we're using GitHub, on the job it might be another service by under the scenes its still Git)
3. Create a repository and start tracking changes!


### Step 1: Install Git locally

[Download git here](https://git-scm.com/downloads)

Windows users will install Git through a tool called Git Bash. This is a helpful terminal environment that helps you interact with Git and your computer more similar to unix based systems (Linux and Mac) so the commands will look more similar. I recommmend checking the boxes during the installation to add Git Bash to context menu shortcuts. That'll come in handy later.

Mac users have a few options to install Git. I recommend installing `Homebrew` and using it install git, which will behind the scenes install `xcode`. It's a long download and a more involved process, but well documented and it'll run great once setup. 

### Step 2: Create a GitHub account

We are using GitHub in all our classes. It's free, and offers some great enterprise level features free for us instructors. 

### Step 3: Create your first repo

After you create an account, create a new `Repository` by [following this guide](https://docs.github.com/en/repositories/creating-and-managing-repositories/quickstart-for-repositories)

Next, you'll want to `Clone` your repository to your computer. This means that you will have a local version of the repo, and a remote version, and they will be linked together where you can send changes from your computer to GitHub, and vice versa. [Follow this guide to clone your repo](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository)

The first time you try to connect to your GitHub account locally you will be asked to sign in. 

Windows users will receive a pop-up window that signs you in through the browser. After signing in, return to your Git Bash window and the clone should have completed successfully. 

Mac users will need to setup an access token for this to work. [Here's a good guide to do that](https://gist.github.com/jonjack/bf295d4170edeb00e96fb158f9b1ba3c)

Once your repo is cloned to your computer, you can create whatever type of coding project you want in that folder or even just copy existing project files into that folder. 

Anytime changes are made to those project files and you want those reflected on your remote repo on GitHub, you'll need to `push` those changes. You'll follow these three steps. In fact, you'll do these so often in your life you might want to get them tattoed on your arm (don't really do that, I don't want to be responsible for that, but do write them down on a sticky)

In a git bash or terminal window inside the repo directory on your computer, type:

`git add .`

The period is necessary. This adds all changes to the files staged and ready for a commit. If you ever want to add some files and not others, you can always type `git add filename`. If you ever add something accidentally and don't intend to push it, you can type `git rm filename`

Next type:

`git commit -m "a summary of your changes inside these quotes"`

The commit grabs all tracked changes since the last time a commit was made and bundles them together, ready to be sent over. Along with these changes you add a short summary of the changes you made. For example, if I added some code to calculate sales tax I might say write: `git commit -m "added sales tax calculations"`. There's different standards for how to write good commit messages, but for now just be specific and detailed in your documentation and that will be good.

Finally, type:

`git push`

This will send the committed changes to your remote repo on that branch. Oh, we haven't even talked about branching yet. That will be another lesson :)

Anytime you make new changes, rinse and repeat those three commands:<br>

`git add .`<br>

`git commit -m "summary of your changes"`<br>

`git push`<br>
