<h1> 👋 Introduction </h1> 

This repo is a development area for the revamped toolkit website.

The development branch `dev` is where we will make additions to the new toolkit website skeleton once they have been reviewed and approved.

These additions will be developed on separate branches (branched off of `dev`) and merged into `dev` once completed.

Once we are happy with the wesbite as it appears on `dev`, `dev` will be merged into the release branch `main`. The release branch will be public facing and used to host the Uncertainty Toolkit website via GitHub pages.

<h2>Instructions on making changes to the website</h2>

Make a copy of the repo project in your favoured IDE by typing the following into the terminal
```
git clone git@github.com:AnalystsUncertaintyToolkit/uncertainty_toolkit_govuk.git
```

Navigate to the `dev` branch:
```
git checkout dev
```

Create a new branch off dev (replacing `my_dev_branch` with a descriptive name for your branch):
```
git checkout -b my_dev_branch
```

Make your changes.

Check how your changes render on the website:
```
hugo server
```
(nb: you will need to have followed the [instructions on installing hugo](https://gohugo.io/installation/) on your machine first).

Once you are happy with your changes, you can check which files have changed using `git status`. 

Next, add files you wish to push to the remote repo with 
```
git add updated_file_1.md updated_file_2
```

Finally, commit your changes with:
```
git commit -m "Your commit message here to describe the changes"
```
and push to the remote repo:
```
git push
```
(You will need to use `git push -u origin my_dev_branch` the first time you push changes to also create a copy of your local branch on the remote repo).





