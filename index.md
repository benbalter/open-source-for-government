---
permalink: /index.html
layout: home
---

{% comment %}Trick Maruku into rendering the table of contents which requires an H1 tag within the markdown{% endcomment %}# &nbsp;{.hidden}

### Contents

* Table of Contents
{:toc}
 
## Open Source Generally

### What is Open Source

foo

### Why Open Source

Bar

## Open Source Community Building

### Encouraging Community Involvement

Simply making the code public is not enough. Open source developers want to get behind a cause. Think of it as analogous to volunteering for a political campaign. They want to know what the project stands for, and where it is going. If they contribute, what will their code be used for in a six months or a year?  As a result, open source project documentation commonly includes three primary pieces of information: 

1. A project mission statement, philosophy, or goal,
2. A features and requirements list, or long-term project roadmap, and most importantly 
3. The status of the project (active development, beta, etc.)

### Mechanics

1. Version control, 
2. Bug tracking ("issues" in GitHub parlance),
3. Packaging for downloading, and
4. Documentation hosting (in GitHub's case, a wiki).

### Communications

Beyond the obvious initial announcement, there are several forms of ongoing communication that may require a bit of planning prior to release. Most successful, large-scale projects have a two-way (note: not announcement only) mailing list, to facilitate interaction among developers, as well as an official IRC channel or other real-time chat forum. 

### Upkeep

Beyond the code itself, best practices dictate that maintaining an open-source project requires significant day-to-day upkeep and may entail both policy and technical decisions. Agencies should empower a team of trusted developers with decision-making authority to: 

1. Individually respond to any issues opened by users ("tickets"),
2. Accept or reject pull requests on behalf of the project, and 
3. Coordinate future releases. 

**Formal governmance is bad, etc. It's about agility, stoopid. Link to GitHub post on pushing 150+ times a day.**

### Governance

Most government projects are governed by a model known by its tongue-and-cheek name "benevolent dictatorship" (as opposed to democratic consensus building). This is not a bad thing. Almost all projects begin this way, and many major projects (including popular projects like Drupal and WordPress) remain this way. 

The term simply means that ultimate decision-making authority rests in a single individual or groups of individuals, rather than by vote of the community as a whole. To be successful, this model will require significant management and delegation of development efforts around:

1. Patching, 
2. Translations, 
3. Documentation and FAQs, 
4. Issue tracking, and 
5. Support

## Delegation

Such a model is arguably the norm for open-source software development, but it must be noted that organization and delegation of such efforts fall squarely on the agency's shoulders. You would be hard-pressed to find a successful open source project that does not have at least one full-time developer or community organizer.

## Commiter Status

In the long term, individual contributors will emerge as key project stakeholders based on the quality and quantity of code contributions and involvement in day-to-day discussions. It is common to grant such contributors committer status (the ability to commit code to the project, accept pull requests, etc.). This is arguably a necessary step for the project's continued evolution.

## Github

### GitHub for the Uninitiated

GitHub is a social code sharing service that allows teams to collaborate among themselves or with the general public. Code is grouped by organizations, which consist of teams, which own repositories. Repositories can be either private or public (open source). In essence, GitHub keeps a running log of all changes to a software project. Each time you make a change, you describe that change (a commit message) and then push that change to GitHub. GitHub also allows members of the public to "fork" existing projects, improve upon them, and then submit their changes back upstream as a "pull request."

*Additional Reading: [Introduction to Git and GitHub](https://help.github.com/)*

### Private Repositories

This will allow you to create proprietary / closed source software.

### Public Repositories

### Public Footprint

GitHub provides a handful of tools to organize projects (internally) and engage with the public. Each repository has a public facing page (powered by the projects readmd.md), a bug tracker (issues), and a wiki. GitHub can also be used to host blogs and microsites using the built in Jekyll engine (and their GitHub pages feature). [More Info](http://pages.github.com/)

### Records

In order to conform with the necessary records requirements, you must associate your commits with your .gov e-mail address so that notifications are properly captured by your agency's records management system. You can do this two ways:

#### If you don't yet have a GitHub account

Simply register for a new GitHub account using your .gov e-mail address. Follow the normal instructions to set up Git, setting your Git e-mail address as your .gov address so that all commits are associated with your official account.

#### If you already have a GitHub account

1. Navigate to the [e-mail settings page](https://github.com/settings/emails) and add and confirm your .gov e-mail address.
2. Ensure that notifications for the PIF organization go to your .gov account on the [notifications settings page](https://github.com/settings/notifications).
3. Create a new repository, or clone and navigate to your team's repository on your computer
4. Configure the repository to use your .gov account by issuing the command `git config user.email your@email.gov` (note, this does not have the `--global` flag as many tutorials suggest, we want the setting to stay within the repository so that commits to other repositories continue to come from your personal account)
5. Repeat step 4 with each additional repository you contribute to in your official capacity

You can safely use your existing GitHub account and public key, as long as commits are associate with and notifications go to your official e-mail.

### Terms of Service

There is an existing gov-friendly terms of service ("TOS") which GitHub has already reviewed and signed with the White House, the General Services Administration, the Federal Communications Commission, and the Conusmer Financial Protection Bureau. Before using the service you should...

F. Accounts
Create an organization. The organization can have an unlimited number of public projects associated with it, and an unlimited number of both public and undisclosed members with various levels of permissions. Contractors and employees should use their individual accounts to commit code, respond to support forums, etc., just as they would on any other project, or on any other social network. It is arguably GitHub's secret sauce (making coding social as their slogan goes), provides a level of transparency and accountability, and is a long-standing norm in the open-source software community, not to mention, the fundamental software underlying the website. Almost without exception, all government agencies that have released open-source software, both on GitHub and otherwise have followed this model.

## Licensing

### Licensing Generally

### Types of Licenses

#### MIT, BSD, Apache

#### GPL

Releasing the project under GPL is done simply by (1) including the text of the license within the repository, (2) posting a boilerplate statement at the top of the main file that notes the licenses and releases subsequent distributors from liability, and (3) noting the license within the project's documentation.

### Government-Specific Considerations

Under 17 U.S.C. § 105, any code created by a government employee on government time is not subject to domestic copyright protection (essentially public domain) and would be licensed as a US Government Work. 

If a project is a derivative work of virally licensed code (e.g., the GPL, the most common open source license), it must be licensed under the same terms as the upstream project (e.g., a WordPress plugin or using a code snippet that was posted under the GPL) and the question of licensing is simple.

If a project does not use any previously licensed code, things can get a bit tricky, especially if you get a pull request from the public (e.g., do contributors surrender the rights to their work by contributing?). It is important to specify the means and terms under which the public can contribute to encourage collaboration. If possible, I would recommend including even a single line of GPL licensed code to simplify things, but you are free to require contributions be licensed under any license, including public domain (although I wouldn't recommend it). Sample language for a GPL'd project below:

[Example Licenses](licenses/)

i. Contractor-created code


Contributing
------------

Federal employees and members of the public are encouraged to contribute to the project by [forking](https://help.github.com/articles/fork-a-repo) and submitting a pull request. (If you are new to GitHub, you might start with a [basic tutorial](https://help.github.com/articles/set-up-git).) 

All contributors retain the original copyright to their code, but by contributing to this project, you grant a world-wide, royalty-free, perpetual, irrevocable, non-exclusive, transferable license to all users under the terms of the [Gnu General Public License v2](http://www.gnu.org/licenses/gpl-2.0.html) or later.

## Additional Resources

1. Producing Open Source Software – Karl Fogel (Practical)
2. The Cathedral and the Bazar – Eric S. Raymond (Theoretical)
3. Understanding Open Source and Free Software Licensing – Andrew M St. Laurent (O'Reily)


