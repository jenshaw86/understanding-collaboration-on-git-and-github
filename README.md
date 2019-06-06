## Recounting My Experiences With Git and GitHub
Git and Github are so misunderstood, and I’ve decided I’d like get to know them better. 

My inital experiences with them were rough, and I want to share that story as well a collaborative GitHub workflow I think might work for me. 

### First Date Impressions
Here were my initial impressions of them before I actually jumped into using them. 

Github’s website says Git and Github are easy to learn. They even say you can learn it without any code! What a *relief*!

Git reveals its greatest potential on the comand line, which is itself seemingly straightforward and unassuming. Sounds *powerful*!

GitHub has a simple website even more intuitive to navigate because of its graphical user interface. That seems *manageable*!

Git itself is a simple name made up of three simple letters. And Github has an adorable mascot, the Octocat.

![Cute Octocat](Octocat.jpg)

__Git__ is a *Version Control System* and __GitHub__ is like Git with social networking. They’re there to help you build and collaborate on projects with peace of mind, and so naturally you’d get the impression that it’s supposed to be simple and easy to use. 

Looking into Octocat's adorable eyes, I honestly believed that Git and GitHub were a cute-appreciating, harmless pair that existed genuinely and only to make my life easy. 

But if that were the case, why do people panic when it's time to use them?

<iframe src="https://giphy.com/embed/p9bj7nrUPAypq" width="480" height="480" frameBorder="0" class="giphy-embed" allowFullScreen></iframe><p><a href="https://giphy.com/gifs/muppets-p9bj7nrUPAypq">via GIPHY</a></p>

### I Just Don't Git You
For many reasons, I've had lots of internal freakouts whenever I've had to approach Git. The command line is simple, but obscure, not only for me but for many inexperienced users. When things go wrong, it screams at you with long lines of complex words. And when things go right, very, very little happens, if anything at all, and you don’t always get validation. The command line just accepts whatever you last entered and then wordlessly and apathetically moves on to the next line leaving you wondering whether you did the right thing or not! I don't know about you, but to me, that's reminiscent of a bad relationship.

Then we add Git and some people into the mix. Although the experience is not all that much different, it’s far more high-risk and terrifying.

### Why It Was Worth Working On My Relationship With Git and GitHub
Several of my bootcamp classmates and I learned the hard way after from our very first collaborative project experience last week that without trying to understand how Git works and establishing a good workflow on Git and Github, you will not only ruin your own efforts, projects, and experiences, but your relationships too.

Even though my project experience suffered, it was an arguably necessary experience because now I'm highly motivated to not repeat my mistakes. Because I now know what it’s like to collaborate on a project, I have a better idea about how to research solutions for my problems and I can read Git documentation with more clarity. I have a stronger sense (I think!) of how Git and Github can help me work more harmoniously with my team, and I think it's only right to share what I've learned so we can all better maintain and preserve our relationships. 

## Collaborative Workflow
So, after a lot of googling, I've concluded that this is a collaborative workflow I can understand and work with. I'm excited to try this approach during my next project and take in and appreciate every moment of peace and no-stress.

If you're not familiar or rusty with Git basics, you can take a look at GitHub's own guide, which is pretty clear. In this section, I'm going to skip over explaining basic stuff like stage, commit, and push, but spend more time explaining what extra steps might be involved in collaborating on GitHub.  


### Setting Your Team Up for Collaboration
So let's assume that we're working a team consisting of multiple people, and we're all working on a brand new project. 

#### Project Setup
##### Creating a Master Branch
First, we need to appoint just one person, and let's name her Abby, and ask Abby to create a new repository for our project. Or in the case that we're starting from a template of another repository, she can fork the repository. Whether a brand new repository or a fork of one, Abby has created a new master branch for all of us to work with! Good job, Abby!

##### Adding Collaborators
But wait! Before we jump into the code, Abby still has to add us all as collaborators to the project!

Click on your repository's Settings on the top tab, and then Collaborators on the left menu. Then using the search bar, search for your team members by name or GitHub name, and click on Add Collaborator to add them to your project. Easily done!

Now that that's done, everyone can clone / download a copy of the repository into their local directories and work on it independently.

##### Having a Game Plan

Well before this stage and certainly by this point we should have a clear plan of how we're going to tackle this project, not leap in already typing away. We really shouldn't ever be working on the same files, and we especially shouldn't be working on the same code. We need establish expectations first.

Let's assign each of us a feature of the project to work on and create feature branches off the master branch for each of us to work on. Very similar to rules of the road, stay in your lane, stay on your own branch. 

##### Creating a Feature Branch
Each of us can create our own branch using the terminal. Type 'git checkout -b ' and the hypenated name of your branch. Now we're working off our own branches and we can start making changes to our feature! Just remember not to work on anyone else's code!

##### I'm Done with my feature! Now What?
Once we've finished working on our feature, it's time to push it up to our remote repository on GitHub. In your terminal, type 'git push origin ' and the name of the branch you've been working on.

Then hop over to your remote repository on Github, and click on the button that says New pull request. 

On the new pull request page, you want to first compare 'base: master' to your changes on your feature branch 'compare: your-feature-branch-name' of the same repository. 

If you get that green light that you're able to merge, you're good to go! Create your pull request by clicking on the green button on the bottom right corner of the form.

##### Time to Merge! 
There are many ways to go about doing this. By default, any contributor can approve a pull request and merge changes into the master branch. But that could be problematic if they're not carefully reviewing the code. 

I like a more democratic approach. We can also either choose one person to review and approve all the pull requests, or we can require that at least one other collaborator outside of ourselves look it over and approve it. That's a pretty neat feature and I think more people should use it. 