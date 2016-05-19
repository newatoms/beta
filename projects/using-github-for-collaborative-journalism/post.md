# Using GitHub for Collaborative Journalism
Inspired by how coders work together and the beautiful ecosystem of GitHub, we’ve created a workflow we believe could help any team that creates content together.

In these beginning times of New Atoms, our new editorial startup that is currently experimenting with new ways to create journalistic and research products, we are largely working with GitHub to track progress and collaborate.

As you have probably found out by now, Google Docs is kind of frustrating for larger complex journalistic projects. It lacks an adequate workflow built into the system, discouraging good collaboration between journalists. Managing changes and versions has not really developed beyond where Microsoft Word was when we all used it for collaboration.

Along with that comes a lot of anxiety. Because all the other collaborators are looking at what you are doing, it can be hard to try out radical changes or make big edits without feeling like you might be bothering your collaborators, or worse, making yourself look stupid.

Even if you are used to using ‘Suggesting’ mode (which you should always use), this often leads to collaborators copying a version, editing and then suggesting their final product.

## GitHub’s editorial flow
In opposition to the system used by things like Google Docs and Microsoft Word, GitHub works with a version control system based on *commits* and *branching*.

This means every collaborator has her or his own version – or *branch* – that they work on, which is explicitly merged with those of her or his collaborators. Every change is added to a *branch* with a *commit*, in which the contributor explains what she or he has added in a short message.

The explicit merging of your contributions with those of others creates a natural moment for everyone to look at the things that have changed, give feedback and review.

In most of our projects we have the following branches. This is a practice borrowed from teams of programmers that need to make sure that everyone works with code that is of the highest quality, and that when the code is published it is guaranteed to work.

(image)

### The branches we create
* There is a ***master*** branch, which should be all information that is fit for publishing.

* There is a ***develop*** branch that shows the current shared state of everything.

* For every new thing that is added to the whole or any specific task given to a contributor, a special ***feature*** branch is created with a clear name according to its intention. In this feature branch, one user or multiple users can work on something that needs to be added to the product.

(image)

### It’s all in the Pull Request
When someone or a group of collaborators is happy with what they have done, they create a *Pull Request* from the *feature* branch to the *develop* branch. This is, as the name suggests, a request to *pull* whatever is in the *feature* branch into the *develop* branch.

This *Pull Request* creates a special GitHub page that lists all the *commits* that have been made — with their messages — and allows other users to edit the files and comment on specific lines.

>A Pull Request is like a forum for reviewing each others' work; it’s a social network for peer or editor review.

## Using Markdown to separate content from its formatting
GitHub’s native text format is something called *Markdown*. A format that is quickly gaining more and more ground in journalism as it has a few advantages. A *Markdown* file is a plain text file in which special characters, typed by the collaborator, give structure and allow for the insertion of images e.g. without losing it’s readability.

* *Markdown* allows the writer to focus on the structure of their text, this is why the file format is the default of apps like iA Writer.
* *Markdown* can be edited in any text editor such as Notepad and the like.
* *Markdown* allows developers to ingest the files and convert them to the right structure for different outputs.

## Using GitHub issues to keep track of what you want and need to do
There is a built-in task manager in GitHub that works great for planning your project, getting an overview of what still needs to be done and flagging what needs to be done right now.

The *Issues* functionality of GitHub is quite simple and resembles a lot of other task management apps. You can create tasks, assign them to team members and associate them with certain milestones that have been planned for the future.

One of the special features of GitHub *Issues* is that you can specify which tasks have been completed by a specific *commit* or *pull request*. Every task has a number (eg #42) and can be easily resolved by mentioning `resolves #42`.

This way of managing issues makes it effortless to solve a greater number of tasks more quickly and easily, plus allows you to track tasks and their proposed solutions.

## The Shortcomings of GitHub
One of the major drawbacks of using GitHub is the dreaded *Merge Conflict* that occurs when two users have edited the same file. As of yet, there is no clear and good way to resolve these conflicts in the browser and thus requires some figuring out to solve.

## Learn more
GitHub has a great introduction to Markdown that you should most definitely check out, as well as a collection of beginner guides on GitHub Guides.

>We love working with GitHub and its Pull Requests for our editorial projects!

If you have any suggestions for the article, please, much obliged! And we’d also love to help you, so if you have any questions don’t hesitate to shoot us a mail at helpdesk@newatoms.com.
