# Review

What went well, what didn't
Challenges - reading all requirements

## Ambiguity

In the future we're not going to have the same level of instruction with
step by step guides.
Soon we're going to start introducing some ambiguity, ambiguity
ambiguity means inexactness, obscurity, or vagueness. It harkens back to the
sanbox way of learning, you're going to have to find out the problem
and locate the solution yourself

## Markdown making a page

Step through making a new page
Step through getting the url for that page when turning in assignments

## Git

### Collaboration
Helpful and necessary tool when working alone or when working with a large group of people
Git is one of the wyas we collaborate

Version control system, ways to maintain files and folders and maintain their system
Multiple ppl can work on the same code
you can view changes, apply new changes, remove changes, revert changers
Keep all files in a single rpository

Without version control lots of issues can arrise

say here you make a term paper, you make some changes to the paper and
perhaps you don't want to get rid of the original so you keep it

then you end up adding foot notes and you want to keep track of that as well
then you 

### Snapshots in time
Git uses a commit it represents successive version of a file or a group of files
Similar to a save as, but it does a little bit more

When I commit I'm telling Git, this is what my project looks like rn, every time you do a save
it saves the 'you are here' so you were at A, and now you're at B, but B still exists.

If you need to go back and look at the initial version, you can
Without Git, you can only ever see the final version, you don't have the previous changes.
Its all one file, but it remembers the changes that were made across that 1 file
and Git remembers every change.

So if you were to work on a file for 2 years, you can go back to the very beginning and see what it
looked like 2 years ago.

Each commit has a label that points to it the HEAD is the label meaning "You are here"
It's a good idea to commit early often. You can add messages to commits, messages are like writing
captions for your code. Be sure to 

### Git and Github are two different things
Github uses Git under the hood, but adds other functionality. Now we're already familiar with
Github. It's a place to store your code and a place to share code with others. You can also make changes to
files on your computer and upload them directly to Github.
You can keep changes seperate until you're ready to input them

### Git + Github = awesome

Multiple people can work together without messing each other up (sometimes)
there's sometimes issues with **merge conflicts** these can occur when

One project = one repository
your front end may be hosted on aws and the back end may be hosted somewhere else for whatever reason

# Demo

### Creating a new repository called hello world

Ask students how i make the new respository
Next **deploy** your website, ask them what the first step is to deploy
the website and then go through to deploying the website

### Command Line Git Setup

Now that we have the terminal properly setup let's go ahead and create a higheracy of folders

* Documents
* Projects
* Codecrew
* Code102

if we go to our github repo we have the code button, we can click on it and then get the link from github
 
we can type git clone [paste the link] not the address bar link, that's not gonna help you
it may ask for your password, now if we chek, we'll see we have a hello world folder

[the computer recognized that this is a git repo and lets me know that i'm in the main branch]

Lets use the **code** command to open our document in vscode. Let's use ACP (Add Commit Push) to push our changes
to github

* **git status** this shows what changes we've made. We've changed the README.md and github knows nothing of that
* **git add [the name of the file] **
* **git status** now it's green, it's ready to be pushed
* **git commit -m 'Message must be in quotes, added another heading' **
* **git status** We commited and moved our head ahead by one commit, our local version (git) is further ahead than what's on github
* **git push origin main** For now push the 'I believe button' on origin main

I beleive on windwos10 you'll always have to continuously put in your username and password for Github
Remember these are public so if you're saying stuff like screw this code or this sucks, people can see that

Keep it clean but also relevant

