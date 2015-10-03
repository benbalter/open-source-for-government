---
title: GitHub
---

# GitHub Generally
[GitHub](http://github.com) is a social code sharing service that allows teams to collaborate among themselves or with the general public and has quickly become the go-to social network for the open source community, much like Facebook is the primary social network among friends and classmates. Code is grouped by organizations, which consist of teams, which own repositories. Repositories can be either [private](#private_repositories) or [public](#public_repositories) (open source).

GitHub is based on, and extends the social functionality, of an open-source [distributed version control system](http://en.wikipedia.org/wiki/Revision_control) known as [Git](http://en.wikipedia.org/wiki/Git_(software)). In essence, Git keeps a running log of all changes to a software project. Each time you make a change, you describe that change (a commit message) and then push that change to GitHub. GitHub also allows members of the public to "[fork](#forks)" existing projects, improve upon them, and then submit their changes back upstream as a "[pull request](#pull_requests)."

GitHub offers free public repositories for open source projects as well as subscription-based private repositories for closed projects. Agencies should create an organization account with GitHub, which can include an unlimited number of individual developer accounts. See [Records](#Records) below for more information.

_Additional Reading: [Introduction to Git and GitHub](https://help.github.com/), [Setting up Git](https://help.github.com/articles/set-up-git)_

# Culture
Each social network has a different culture, and espouses different values from its users. While posting pictures of a family vacation may be commonplace on Facebook, the same cannot be said for Twitter or Pinterest. Likewise, while providing customer service and interacting directly with customers via Twitter is an every day occurrence, if a major corporation were to try and friend me on Facebook, I'd be a little confused.

GitHub is no different. GitHub is about sharing, but instead of sharing photos or feedback you share code. Notice the word we use here is code, not software. The expectation is not that anyone can go and get a polished piece of software as you might from a big-box retailer. Instead, the expectation is that those that produce the software would release the underlying code early and often in its raw form. Bugs and unpolished work are not only accepted, it's the norm.

Think about it this way: putting out a press release with a typo (or even an unfinished press release) is embarrassing because the point of the network is to disseminate information from agency to press and erroneous or missing content hinder that end. The point of open source on the other hand is to collaborate in the creation of software. Allowing early adopters to discover bugs, review early project roadmaps, and suggest ways to improve the software _furthers_ that end. As a result, openness, transparence and contributions and valued much more highly than refined code and polished documentation.

Put simply, the culture on this social network is not to criticize but to create, and it has [mechanisms to enforce such social norms](https://github.com/WhiteHouse/petition/issues/2).

# Public Repositories
Public repositories are the default on GitHub. Public repositories are free and are freely accessible (to read but not edit) for anyone on the internet. Public repositories are cheap (literally). Do not be afraid to use them to save and store early R&D efforts, thought experiments, or even side projects.

Whereas on a government website it may be strange to have extraneous pages with content that has not be recently updated, public repos are treated differently. They often serve as the conical archive for other efforts, and at the very least, are used to showcase development efforts and creative thinking, no matter how small. As a result, a large presumption **in favor** of creating public repositories and a large presumption **against** deleting or renaming exists.

# Private Repositories
Private repositories allow you to create proprietary / closed source software. This could be used in two ways. First, it can be used simply to facilitate in the collaboration of internal tools or other projects that don't really make sense to open source due to their specific nature. Second, it can be used as a staging environment to prepare open source projects for release one they reach a minimum viable product.

Private repos are created on a [free-based pay structure](https://github.com/plans).

# Public Footprint
GitHub provides a handful of tools to organize projects (internally) and engage with the public. Each repository has:
1. A public facing page (powered by the projects readmd.md),
2. A bug tracker (issues), and
3. A wiki.

GitHub can also be used to host blogs and micro sites using the built in Jekyll engine (and their GitHub pages feature). [More Info](http://pages.github.com/)

# Social Coding
Two things that makes GitHub a bit different from many other code sharing services are the concepts of the fork and pull request.

## Forking
A fork is an alternate or parallel copy of a piece of software. Forks are created from public repositories from often unaffiliated developers. A GitHub user may fork a repository because they simply want a snapshot of the code as a simply bookmark, or more commonly, fork the repository in hopes of improving upon it. Even a user does not have permission to write to an agencies repository (e.g., a member of the public), they can always fork the repository, and make the desired changes in their fork without affecting the original.

## Pull Requests
Pull requests allow other, unaffiliated developers to submit their improvements for consideration by the original project. The project administrators are publicly presented with the changes, along with a forum to discuss them, and can then either choose to accept or reject the proposed improvements. In most cases, once accepted, the changes are automatically merged and the contributor is given credit in the commit log.

It is [perfectly acceptable](http://ben.balter.com/2012/04/15/cfpb-accepts-first-citizen-submitted-pull-request-on-behalf-of-federal-government/) (and even encouraged) for the government to accept pull requests from the public.

# Records
When it comes to records, the good news about GitHub (and git), is that its chief purpose is to keep track of who made changes to what file when. In order to conform with the necessary records requirements, you must associate your commits with your .gov e-mail address so that notifications are properly captured by your agency's records management system. You can do this two ways:

## If you don't yet have a GitHub account
Simply register for a new GitHub account using your .gov e-mail address. Follow the normal instructions to set up Git, setting your Git e-mail address as your .gov address so that all commits are associated with your official account.

## If you already have a GitHub account
1. Navigate to the [e-mail settings page](https://github.com/settings/emails) and add and confirm your .gov e-mail address.
2. Ensure that notifications for the organization go to your .gov account on the [notifications settings page](https://github.com/settings/notifications).
3. Create a new repository, or clone and navigate to your team's repository on your computer
4. Configure the repository to use your .gov account by issuing the command `git config user.email your@email.gov` (note, this does not have the `--global` flag as many tutorials suggest, we want the setting to stay within the repository so that commits to other repositories continue to come from your personal account)
5. Repeat step 4 with each additional repository you contribute to in your official capacity

You can safely use your existing GitHub account and public key, as long as commits are associate with and notifications go to your official e-mail.

Some agency records retention office may also require more detailed records retention plans. Additional methods of ensuring no history is lost may be to use project activity RSS feeds, post-commit hooks to e-mail, or by hooking into the API directly. You can even use the Git repository itself as the formal record. Since the version control is fully distributed, it will contain a copy of each commit. It will not, however, contain GitHub social activity like comments or issues.

# Terms of Service
There is an existing gov-friendly terms of service ("TOS") which GitHub has already reviewed and signed with the White House, the General Services Administration, the Federal Communications Commission, and the Consumer Financial Protection Bureau among others. Before using the service you should double check with your agency's general counsel's office.

# Accounts
Create an organization. The organization can have an unlimited number of public projects associated with it, and an unlimited number of both public and undisclosed members with various levels of permissions.

Contractors and employees should use their individual accounts to commit code (rather than say an agency account), respond to support forums, etc., just as they would on any other project, or on any other social network, however to ensure records retention and that the commits come from an official source (e.g., to delineate commits in one's official capacity versus commits in one personal capacity), the account should be associated with a .gov e-mail address as [described above](#records).

It is arguably GitHub's secret sauce (making coding social as their slogan goes), provides a level of transparency and accountability, and is a long-standing norm in the open-source software community, not to mention, the fundamental software underlying the website. Almost without exception, all government agencies that have released open-source software, both on GitHub and otherwise have followed this model.
