# Your first static web site: Hello, World!

In this lesson, we'll walk through the workflow that we'll be using throughout the course to set up projects, write some code, run the code, and grade our work.

[Here is a very brief video demonstration](https://share.descript.com/view/aSOPQUdgU9G). You should not rely entirely on the video to complete this lesson, but I wanted to give you a quick, visual overview of the process. But then PLEASE READ the below lesson as you are going through the steps, since there is much more detail in the text than in the video.

## Get a GitHub account

GitHub.com is the center of the software development universe, these days.

At its core, it's like Dropbox for code — a way to store your code in the cloud so that you never lose it, even if the computer where you are writing it is lost.

Over time, GitHub has added tons of other features, such that nearly every company and open-source project uses it for collaboration, quality assurance, and other things. Becoming familiar with GitHub is one of our key learning objectives.

- Sign up for a free GitHub account at [github.com/join](https://github.com/join). (Be sure to select the "Free" plan; you don't need to pay for your account.)
- Remember to verify your email address after signing up, before you continue on with the lesson.

We'll talk a lot more about GitHub and its features as we go along.

## Set up grades.firstdraft.com

In order to check our work and receive instant feedback, we'll be using a system called Grades (grades.firstdraft.com). Let's do some one-time setup to get it configured properly.

- First, click the button below to load the Grades project in a new browser tab. Then come back to this page and follow the remaining steps.

LTI{Load Hello, World! assignment}(https://grades.firstdraft.com/launch)[S9ymPy6WCsn18gLbByVbZQ7k]{vfdtzJb5bLYqYwuqgeRKpc5d}(2)[Hello, World Project]

### First time loading a project

The very first time you load the Grades interface, you will be asked to sign in to your GitHub account if you're not already:

<!-- ![](/assets/launch-grades-project-signin-to-github.png) -->
![](https://res.cloudinary.com/dmxgp9oq2/image/upload/v1685996960/launch-grades-project-signin-to-github_yxmtvk.png)

You will then be asked to "Authorize Grades"; click the green button to proceed:

<!-- ![](/assets/launch-grades-project-authorize-grades.png) -->
![](https://res.cloudinary.com/dmxgp9oq2/image/upload/v1685997353/launch-grades-project-authorize-grades_tgxaqr.png)

When you reach the "Project Setup" page, wait for approximately 15 seconds and then refresh the page. You should see a blue banner appear at the top of the page saying that you have been invited to the organization: "appdev-projects". This is the organization that we use to share all of the projects for the course.

Do not proceed until you see the notice. Refresh the page a few times; it should appear within 1 minute.  Click on the "accept invite" link, and then press the green button to join the organization.

<!-- ![](/assets/launch-grades-project-accept-invite-1.png) -->
![](https://res.cloudinary.com/dmxgp9oq2/image/upload/v1685997960/launch-grades-project-accept-invite-1_gz93li.png)

<!-- ![](/assets/launch-grades-project-accept-invite-2.png) -->
![](https://res.cloudinary.com/dmxgp9oq2/image/upload/v1685997950/launch-grades-project-accept-invite-2_iylajb.png)

Once you've accepted the organization invitation, you can close that tab.

Phew! Fortunately, we only needed to do this setup once.

## Fork the project repository

When you load a Grades project, you'll arrive at a page with several links.

Your first step will be to open the link that looks like `appdev-projects/<project-name>` in a new tab:

<!-- ![](/assets/launch-hello-world-fork.png) -->
![](https://res.cloudinary.com/dmxgp9oq2/image/upload/v1689100920/launch-hello-world-fork_c8kapv.png)

This will take you to my copy of the project, containing any starter code, on GitHub.com. "Repository" is Git's term for "a folder containing code". We also often say "repo", for short.

The next step is to create your own copy of the starter code, so that you can save your work and have it forever. GitHub calls these copies "forks".

On my repo's page, click on the "Fork" button in the top-right:

<!-- ![](/assets/launch-grades-project-2.png) -->
![](https://res.cloudinary.com/dmxgp9oq2/image/upload/v1686701065/launch-grades-project-2_hduxmk.png)

On the "Create a new fork" page, make sure that your personal GitHub username is set as the "Owner" and that your copy's name is the same as mine. 

Now click "Create fork":

<!-- ![](/assets/launch-grades-project-3.png) -->
![](https://res.cloudinary.com/dmxgp9oq2/image/upload/v1686701280/launch-grades-project-3_tnau3z.png)

It will take a few seconds to make a copy, and then you should end up on a page for your own fork of the repository.

If all went well, you should see `github.com/<your-username>/<project-name>` in your address bar, and a note "forked from `appdev-projects/<project-name>`":

<!-- ![](/assets/launch-grades-project-4.png) -->
![](https://res.cloudinary.com/dmxgp9oq2/image/upload/v1686701561/launch-grades-project-4_zpnslw.png)

## GitHub Codespaces

We have loaded the assignment and made our own personal copy of the code. It's time to start building on it!

One of the most painful parts of learning how to program, in the old days, was simply setting up your computer to be able to write and run code. At a minimum, we needed to install:

  - An application to write your code with.

  - The programming language itself (e.g. Ruby). Writing code is not useful on its own if we don't have something to run it with.

There are so many different combinations of hardware, operating systems, previously installed software, etc., that just getting these things installed would often stop you before you started writing your first program. We can't allow that!

Instead, we're going to write our code using a _cloud_ computer. "Cloud" just means that it's a computer that's sitting in someone's warehouse somewhere, and we rent it from them. It already has all of the software that we need installed on it, and we access it through our browsers. No muss, no fuss!

<aside markdown="1">
A warehouse full of computers that people rent and connect to via the internet is called a "data center". Some data centers have their own power plants, and some are even earthquake-proofed.
</aside>

Using a cloud computer to write and run our code used to take several more setup steps. However, happily for us, GitHub recently released a new product called Codespaces, which is a cloud IDE (integrated development environment) built right in to our repositories!

## Start your first Codespace

- Make sure you're on the page of your own fork (i.e. `github.com/<your-username>/hello-world`, i.e. _not_ my copy at `github.com/appdev-projects/hello-world`).
- Click the "Code" drop-down button, click the "Codespaces" tab, and click "Create codespace on main".

<!-- ![](/assets/launch-codespace.png) -->
![](https://res.cloudinary.com/dmxgp9oq2/image/upload/v1685989212/launch-codespace_dl0erj.png)
{: .bleed-full }

This will open a "Setting up your codespace page". 

**Be patient. The first time you setup a Codespace for a repository takes about two minutes. But subsequent loads of the Codespace will be much faster.**

### Sidenote: reopening a Codespace

Sidenote: You can see [a list of all of your Codespaces at github.com/codespaces](https://github.com/codespaces). Over time, you'll have dozens. It might be a good idea to bookmark that page — you'll be visiting it a lot.

If you close a workspace and then want to resume working on that project later, visit [the list](https://github.com/codespaces), locate the existing workspace, click the `...` menu, select "Open in ...", and "Open in browser":

<!-- ![](/assets/codespace-setup-9.png) -->
![](https://res.cloudinary.com/dmxgp9oq2/image/upload/v1680218038/codespace-setup-9_tddgdj.png)
{: .bleed-full }

### Codespace (VSCode) layout

Whenever you boot up a fresh Codespace, [Visual Studio Code](https://code.visualstudio.com/) (a.k.a. VSCode) is the application that you are interacting with.

The basic components of the VSCode window are the three **panes**:

* the **left pane** 
  * containing the **file explorer** and **source control tabs** (where you create and open files and visit your Git version control)
* the **top pane** 
  * containing the **code editor tabs** (where you type and edit files in your codebase)
* the **bottom pane** 
  * containing the **terminal** and **ports tabs** (where you run a live app server on a port with `rackup` and run `rake grade`)

<!-- ![](/assets/vscode-layout.png) -->
![](https://res.cloudinary.com/dmxgp9oq2/image/upload/v1686338851/vscode-layout_yh62tb.png)
{: .bleed-full }

### Reopen a pane

Sometimes you might accidentally close out of the explorer (left pane) or terminal (bottom pane).

To reopen them, there are keyboard shortcuts to close and reopen:

* <kbd>Ctrl</kbd> (Windows) or <kbd>Cmd</kbd> (Mac) + <kbd>B</kbd> for left pane, 
* <kbd>Ctrl</kbd> (Windows) or <kbd>Cmd</kbd> (Mac) + <kbd>J</kbd> for bottom pane.

But, you can always click on the top left hamburger menu to bring up the VSCode options and visit "View" to reopen:

<!-- ![](/assets/vscode-reopen-editor-or-terminal.png) -->
![](https://res.cloudinary.com/dmxgp9oq2/image/upload/v1686338878/vscode-reopen-editor-or-terminal_ekhafk.png)
{: .bleed-full }

### The terminal tab

Before we go on, take a moment to read about the all-important, but perhaps unfamiliar, terminal tab in the bottom pane.

This is a place for you to type commands ("instructions") to be run by the underlying operating system or coding environment.

In the terminal tab, we have:

<!-- ![](/assets/terminal-hello-world-layout.png) -->
![](https://res.cloudinary.com/dmxgp9oq2/image/upload/v1689097394/terminal-hello-world-layout_pin2jy.png)
{: .bleed-full }

* The GitHub repo name.
* The current git "branch", or version of the code, that you are on (usually this will be `main`).
* The `%` sign, or **bash prompt**. 
    * `bash` is a program running at the operating system level that allows you to enter instructions to the computer.
    * You may see other styles of **command prompt**, like a `$` or `>` symbol. If you see one of these symbols at the end of your terminal prompt, it means the terminal can be typed into and new commands can be run.
* A `+` button icon for opening additional fresh bash prompts in tabs.
* If you open another bash tab, you will see a navigation pane to click between them.

## `rackup`: Your live application preview

In the terminal pane, click on the `+` icon to open a second bash prompt, then click on the prompt so that your cursor is shown after the `%` bash prompt. Type this command then hit <kbd>return</kbd>:

```
rackup
```

<!-- ![](/assets/bash-vs-rackup-puma.gif) -->
![](https://res.cloudinary.com/dmxgp9oq2/image/upload/v1689098330/bash-vs-rackup-puma_pmbidx.gif)
{: .bleed-full }

A few things should have happened:

* The name of the current prompt in the navigation pane should have changed from `bash` to `puma`. This name is telling you the current program that is running in that terminal. In this case `puma`, which is the web server that we are using to view the app. In the original terminal, you will still see `bash` and if you click back to that terminal you will see the `%` bash prompt.

* In the terminal that is now running the `puma` web server, you should see a long output, which is just telling you that the **live application preview** is running. You can no longer type into this terminal tab now (you won't see the `%` sign), because it is now dedicated to running your application server.

* You may be prompted in a little pop-up message to "Open browser". 

To open the live app preview in a new browser tab, visit the "Ports" tab in the bottom pane, look for the port with a green dot 🟢 on the left side (indicating that it is active), and hover over the "Local Address" column, then click the globe 🌐 button to "Open in Browser":

![](https://res.cloudinary.com/dmxgp9oq2/image/upload/v1688656108/ports-tab_cfaa1k.png)

Clicking this icon should open a new browser tab with the live preview of your app (but there's nothing there yet, so you'll see a 404 page not found message). 

If you ever close this browser tab, you can reopen the live app preview at any time by visiting the Ports tab.

---

The live app preview has a long, complicated URL, with the structure:

```
https://USERNAME-CODESPACE-NAME-vrpqrxxrx7x2rxx-3000.preview.app.github.dev
```

This URL is tied to the mini computer you are running in your Codespace. Specifically, it's tied to the terminal that you ran `rackup` in, which is now running the `puma` web server. If that terminal tab is closed for any reason (including if you close the Codespace), your live app will no longer be running, and the URL will not be visitable. But you can always open a new terminal tab with `+` and `rackup` again.

At this point, in the live application browser tab you should see a 404 page missing message. Let's change that!

## Adding an `index.html` homepage

Right-click in the file explorer (left pane) in VSCode and let's create our first HTML file. Call it `index.html`.

In that `index.html` file that opens in a new editor tab (top pane), put the following code:

```html
<h1>Hello, world!</h1>
```

Back in your live app preview browser tab, refresh the page and make sure that your HTML message shows up.

(Technically, we should have added `/index.html` to the end of our live app domain in order to see the page, like this:

```
long-domain-name.preview.app.github.dev/index.html
```

But if there's a file with the specific name of `index.html`, then it will be displayed when someone visits the "naked", i.e. "root", domain.)

Yay! Our first web page is up and running.

## Git commit and push

GitHub's core functionality is to allow us to save our code in the cloud. To do this, we need to do two things:

- Make a **git commit**, which is a snapshot of our entire project at a given moment in time.
- **Push** the commit from our local computer to GitHub.com.

In your Codespace VSCode window, there are a few tabs on the left side bar that open in the left pane:

<!-- ![](/assets/vscode-explorer-git-tabs-hello-world.png) -->
![](https://res.cloudinary.com/dmxgp9oq2/image/upload/v1686709045/vscode-explorer-git-tabs-hello-world_swedfx.png)

Click on the "Source Control" tab, which will bring up this view in the left pane, where you can enter a **commit message** and click the "Commit" button:

<!-- ![](/assets/vscode-git-commit-hello-world.png) -->
![](https://res.cloudinary.com/dmxgp9oq2/image/upload/v1686709462/vscode-git-commit-hello-world_clmplq.png)

You will see a message pop up asking if you would like to "stage all your changes and commit them directly". Click "Yes".

The best time to commit is right after you just got something to work, before you start on your next experiment. But, in general, you can never commit and push too often.

Remember: **ABC**: *Always Be Committing (ABC)*.

Did you notice the "Commit" button change to "Sync" after you committed?

Whenever you are ready to store your changes on GitHub, click the "Sync" button, and when you get the pop-up message, select "Ok, Don't Show Again":

<aside markdown="1">
Pressing "Sync" actually does two things: it runs "git pull" to pull down any changes from the repository on github.com and then runs "git push" to publish your current commits to the repository.
</aside>

<!-- ![](/assets/vscode-sync-button.png) -->
![](https://res.cloudinary.com/dmxgp9oq2/image/upload/v1689104419/vscode-sync-button_mrbmda.png)

(You may get a message after this first sync asking if you would like to periodically run "git fetch". You can say "Yes" to this.)

You should get into the habit of committing and pushing your code to GitHub very often. If you do, then you're certain never to lose your work, among many other benefits of using GitHub to store your code.

When you push the code, each commit you made gets registered in the history of your fork of the GitHub repo. In other words, you can view any given snapshot of your code, at any time, forever. Yay!

Visit the repo at `github.com/<your-username>/hello-world` to see the published commits, stored safely forever:

<!-- ![](/assets/vscode-git-pushed-history-hello-world-1.png) -->
![](https://res.cloudinary.com/dmxgp9oq2/image/upload/v1689105281/vscode-git-pushed-history-hello-world-1_nqtupr.png)
{: .bleed-full }

<!-- ![](/assets/vscode-git-pushed-history-hello-world-2.png) -->
![](https://res.cloudinary.com/dmxgp9oq2/image/upload/v1689105276/vscode-git-pushed-history-hello-world-2_yz3has.png)
{: .bleed-full }

## Grading with `rake grade`

Once we've tested our work manually by visiting the live preview, and we think everything looks good, there's one more step we can take to be sure — run automated tests.

For most of our projects, I have included automated tests that will visit every page and click on every link and make sure the app is behaving correctly under all circumstances. If it isn't, you will get immediate feedback so you can fix it.

In the terminal tab in the bottom pane, open the bash prompt (i.e. not the terminal tab that is currently running `puma`). You can alway use the `+` icon in the terminal tab to open a fresh `%` bash prompt tab if you don't already have one open. 

<aside markdown="1">
If you want to cancel the `puma` server running with the `rackup` command (thus closing your live app preview), and return to the bash prompt to enter another command, you can just press: <kbd>Ctrl</kbd> + <kbd>c</kbd>

That's a very important command: it will cancel any currently running terminal process if your terminal gets stuck doing something and you want access to the bash prompt again to enter new commands.
</aside>

At the bash prompt, run the command:

```
rake grade
```

The first time you run it (per project), it will ask you for an access token. Click the "Load assignment" button from the beginning of this lesson to return to the grades.firstdraft.com page for this project if you have since closed or lost that browser tab.

Copy-paste the token from the Grades page into your terminal. This only needs to be done one time, and then the token will be stored in that workspace:

<!-- ![](/assets/grades-token.png) -->
![](https://res.cloudinary.com/dmxgp9oq2/image/upload/v1686005312/grades-token_vyb9cy.png)
{: .bleed-full }

You may get a pop up window in the Codespace workspace asking for permission to paste from your clipboard into the workspace, you should "Allow" this action.

<!-- ![](assets/grades-token-enter.png) -->
![](https://res.cloudinary.com/dmxgp9oq2/image/upload/v1686008287/grades-token-enter_wf7s8y.png)

You should see output that looks like:

<!-- ![](assets/grades-token-submission-url.png) -->
![](https://res.cloudinary.com/dmxgp9oq2/image/upload/v1686008310/grades-token-submission-url_lc4mpf.png)

Copy-paste the Results URL into a new tab, or <kbd>Cmd</kbd> + click (Mac) / <kbd>Ctrl</kbd> + click (Windows) on it. (Select "Trust grades.firstdraft.com" in the dialog that comes up.)

This will take you to a "build report" with the results of our automated tests for the project.

Is everything green? If so, then you have passed the tests and your grade has been registered. If you see any red, then try clicking on the test to see if there's more information that can help you fix the issue. You can close this browser tab when you are done with it. 

That's fundamentally it for grading in this project and others in this course. **You can run `rake grade` in your terminal as many times as you want**, and you will get a new updated build report each time. Make it all green and you have completed the assignment!

## Deploy your app

We can now view our app in the live preview in our Codespace, and we've published the code to GitHub.

Now let's see how we can actually deploy our app to the internet with a custom domain name so that anyone in the world can view what we created.

You have two options for deployment:

1. **Fly.io**. We recommend this option, since it works for dynamic web apps as well and we will use it later in the course. However, it does require you to enter credit card information. You will not be charged, but you must have a credit card to enter into your profile.

2. **GitHub Pages**. This option is completely free and does not require a credit card, but it will only work for static websites.

Depending on which option you choose, find the appropriate next lesson on Canvas to deploy the "Hello, World" web site.
