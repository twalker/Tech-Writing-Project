# Tech-Writing-Project
Class repository
Getting started!


----

## How to work on the site on your machine

This site was created from a [11ty](https://www.11ty.dev/) starter project which uses Node.js to build static web pages from markdown, html and a variety of templates. See the [./11ty-starter-readme.md](./11ty-starter-readme.md) for more information about how the project works.

The site runs on your local machine so you can verify changes. 

## Install

1. [Install git](https://git-scm.com/downloads) if it is not already installed.
2. Download and install Node v16 from [https://nodejs.org/en/](Node.js).
4. Open a terminal and clone the repository:

```bash
git clone git@github.com:cmneal26/Tech-Writing-Project.git
```

5. Using a terminal, navigate into the root folder of the repository, and install 11ty's npm dependencies:

```bash
npm ci 
```

## Running the site locally 

From a terminal in the root directory of the project, run:

```bash
npm start
```

This will start a server on your machine and can be browsed:
[http://localhost:8080/](http://localhost:8080/)
The server can be stopped with the `Control + c` keyboard shortcut.

Updates to pages should automatically be loaded  in your browser (aka Hot reloading). If changes are not appearing, stop and restart the sereve.

## Buiding the site

The `docs/` folder is generated by 11ty and that is the folder that is served in GitHub pages. Running this command to build the site into the `docs/` folder:



```bash
npm run build
```

## Workflow for making page updates

1. Check out a branch to make your changes.  

The branch name can be any name, my-changes is used as an example.


```bash
git checkout -b my-changes
```
2. Start the server

```bash
npm start
```

3. Make changes to files and preview the changes at [http://localhost:8080/](http://localhost:8080/)

When you're happy with the changes to the page(s):

```bash
# build the site into the docs directory
npm run build
# add the changes to your branch
git add . 
git commit -m "My delightful changes"
# Upload (aka push) your changes to GitHub
git push -u origin my-changes
```

Create a pull request in GitHub by either:

A) Opening the link included in the output.

For example:

```bash 
remote: Create a pull request for 'my-changes' on GitHub by visiting:
remote:  https://github.com/cmneal26/Tech-Writing-Project/pull/new/my-changes
```

Or, 

B) Go to GitHub and [create a pull request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request) for your branch.

Your changes are now ready for review by your teammates.

About 5 minutes after your pull request is merged, the changes will appear on:

[https://cmneal26.github.io/Tech-Writing-Project/](https://cmneal26.github.io/Tech-Writing-Project/)

:^)

