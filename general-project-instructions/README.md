# Project Instructions

For every project you will follow the same process of:
1. Forking my project repo as a starting point
2. Clone your forked copy locally
3. Develop your code & push to github your updates
4. Create a pull request and submit a link to that pull request for your submission

## Step 1: Fork the project

To create a copy of my base code into your own repo, you
will need to `fork` this project.

In the top bar in GitHub there is a fork button. Press that,
and make sure you are logged into your GitHub account. It will
prompt you with some default settings for this new copied repo,
and you can accept and fork the project.

You now have your own repo with a copy of my starter code for this project.

**Important last repo setup step!!** Go to the Actions tab on your forked repo and click the green button that says "I understand..." to allow github actions to run. If you don't see that button after clicking Actions, then you're good to go.

## Step 2: Clone the repo

Now you will clone your repo to your local computer.

Click the green code button on your GitHub repo. Make sure HTTPS tab is selected
and copy the https URL.

Use your terminal/git bash on your computer and navigate to
wherever you save your Java projects. Once you are where you want
to copy the project, type:

`git clone https://copiedurlhere`

Where the copied URL is the one you copied from the green code button
on GitHub.

Hit enter and the project will clone to your computer.

## Step 3: Open the project in IntelliJ

Open IntelliJ and select open. Navigate to the project folder
and select open. You now have the project open in IntelliJ and ready to make changes!

## Step 4: Project requirements, make your changes and test

Follow the directions below to complete the assignment.
Test your project by running it and verifying it works as expected.

## Step 5: Push changes to GitHub

Once you have made your changes and tested that they work, you will need to
push your changes to GitHub.

In IntelliJ there's a terminal already open you can use, or you can do this in
your own terminal as long as you navigated to the project directory.

In the terminal type the following commands:<br>

`git add .`<br>

`git commit -m "summary of your changes"`<br>

`git push`<br>

At any point you can type: `git status`
This will give you the status of your changes, whether you added
or committed them already.

You will repeat this process anytime you want to push new changes.

## Step 6: Submit a pull request

When you are ready to submit you will need to submit a pull request. A pull request
is a git terminology that means you are wanting to submit your changes back to the repo
you forked from (mine). This gives us a great layout for reviewing the changes you made
and checking that the automated tests passed.

To do this you will start with **your repo** open in GitHub. You will know you are looking at your repo when it has your username in the URL. (Pull request cannot be created if you try to start it while on my repo). 

Click on the Pull Request tab located on the top bar.

Click `New pull request`.

By default, the branches will be main and will target your main branch to merge into my repo's main branch.
You can accept this and click `Create pull request`.

Give it a descriptive title and add a description of your changes. Then click `Create pull request`.

You are now taking to the pull request that was just created. The URL should end with `pull/##` where the ## is the unique number for the pull request. Copy that URL. You will use it when you turn in your project.

This will now show up on my side, and I can review your changes. It will also kick off an automated pipeline
to run tests. Give it a few minutes, and you'll see a checkmark next to the job.

## Step 7: Turn it in

I will review the code and tests through the pull request. Please submit a link to this pull request, and a zipped up copy of your project for backup to MyHills.
