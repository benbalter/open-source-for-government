---
permalink: /index.html
layout: home
---

* Table of Contents
{:toc}
 
What is Open Source
-------------------


GitHub for the Uninitiated
--------------------------

GitHub is a social code sharing service that allows teams to collaborate among themselves or with the general public. Code is grouped by organizations, which consist of teams, which own repositories. Repositories can be either private or public (open source). In essence, GitHub keeps a running log of all changes to a software project. Each time you make a change, you describe that change (a commit message) and then push that change to GitHub. GitHub also allows members of the public to “fork” existing projects, improve upon them, and then submit their changes back upstream as a "pull request."

*Additional Reading: [Introduction to Git and GitHub](https://help.github.com/)*

Private Repositories
--------------------

This will allow you to create proprietary / closed source software.

Public Repositories
-------------------

Public Footprint
---------------

GitHub provides a handful of tools to organize projects (internally) and engage with the public. Each repository has a public facing page (powered by the projects readmd.md), a bug tracker (issues), and a wiki. GitHub can also be used to host blogs and microsites using the built in Jekyll engine (and their GitHub pages feature). [More Info](http://pages.github.com/)

Records
-------

In order to conform with the necessary records requirements, you must associate your commits with your .gov e-mail address so that notifications are properly captured by your agency’s records management system. You can do this two ways:

### If you don’t yet have a GitHub account

Simply register for a new GitHub account using your .gov e-mail address. Follow the normal instructions to set up Git, setting your Git e-mail address as your .gov address so that all commits are associated with your official account.

### If you already have a GitHub account

1. Navigate to the [e-mail settings page](https://github.com/settings/emails) and add and confirm your .gov e-mail address.
2. Ensure that notifications for the PIF organization go to your .gov account on the [notifications settings page](https://github.com/settings/notifications).
3. Create a new repository, or clone and navigate to your team’s repository on your computer
4. Configure the repository to use your .gov account by issuing the command `git config user.email your@email.gov` (note, this does not have the `--global` flag as many tutorials suggest, we want the setting to stay within the repository so that commits to other repositories continue to come from your personal account)
5. Repeat step 4 with each additional repository you contribute to in your official capacity

You can safely use your existing GitHub account and public key, as long as commits are associate with and notifications go to your official e-mail.

Licensing
---------

Under 17 U.S.C. § 105, any code created by a government employee on government time is not subject to domestic copyright protection (essentially public domain) and would be licensed as a US Government Work. 

If a project is a derivative work of virally licensed code (e.g., the GPL, the most common open source license), it must be licensed under the same terms as the upstream project (e.g., a WordPress plugin or using a code snippet that was posted under the GPL) and the question of licensing is simple.

If a project does not use any previously licensed code, things can get a bit tricky, especially if you get a pull request from the public (e.g., do contributors surrender the rights to their work by contributing?). It is important to specify the means and terms under which the public can contribute to encourage collaboration. If possible, I would recommend including even a single line of GPL licensed code to simplify things, but you are free to require contributions be licensed under any license, including public domain (although I wouldn’t recommend it). Sample language for a GPL’d project below:

[Example Licenses](licenses/)

Contributing
------------

Federal employees and members of the public are encouraged to contribute to the project by [forking](https://help.github.com/articles/fork-a-repo) and submitting a pull request. (If you are new to GitHub, you might start with a [basic tutorial](https://help.github.com/articles/set-up-git).) 

All contributors retain the original copyright to their code, but by contributing to this project, you grant a world-wide, royalty-free, perpetual, irrevocable, non-exclusive, transferable license to all users under the terms of the [Gnu General Public License v2](http://www.gnu.org/licenses/gpl-2.0.html) or later.

