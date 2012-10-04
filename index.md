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

Open source software is a collaborative model of software development whereby the human-readable source code used to produce a given piece of software is made freely available for others to adapt or improve upon as they see fit. Most often (although not always) such development efforts occur publicly, and may involve many disperate groups of developers contributing to the project (rather than a single software firm).

Open source software (sometimes known as free, open source software or FOSS) represents a forward-thinking political philosophy, not an alternate software development workflow or business model. In this context, free refers to free as in speech, not free as in beer. In fact, there's no reason you can't sell open source software, or even make a living producing it. Many large, private sector firms (Facebook, Twitter, Microsoft, Google to name a few) are actually extremely influential members of the open source community.

### Why Open Source

There are lots of arguments in favor of adopting an existing open source project:

* Lower cost - No costly licensing, no vendor lock in
* Nimble - FOSS often is better and remaining responsive to emerging trends
* Open - Open standards encourage interoperability. You own your own data; no proprietary formats
* Fast fixes - The distributed model enables rapid detection and patching of bugs
* Custimizable - You own the code. Make it do what you want.

The argument in favor of creating an open source project, however, is slightly more nuanced:

Emperically, [open source produces better, more reliable software](http://www.coverity.com/library/pdf/coverity-scan-2011-open-source-integrity-report.pdf). Think about it logically. When you (or your organization) is the only person that's ever going to see something, you're a lot more likely to "just make it work." After all, who would ever know? [^1]

But the same logic that applies to sweeping literal dirt under the rug doesn't apply to writing code. Whereas a rug will always serve to cover the floor, applications evolve over time and code is often constantly reused and repurposed as customers' needs change. Simply put, it's impossible to predict today where your code is going to be a year from now and it's in your best interest to plan accordingly.

Open source hedges this risk by distinguishing generic logic (say posting content online) from application-specific customization (say the use-case-specific presentation of that content). Yet when you're writing with the intention of producing proprietary or one-off code, you do everything in one pass. The true challenge arises when the same problem emerges again in another department, another business unit, or more generally in an even slightly different context. You're reinventing the wheel. You're "open sourcing" (even if within your organization). The solution? Always assume your software is going to be open source, even if you know it's never going to be, and here's why:

Imagine you building a house and the contractor literally nails down all your furniture at the onset, saying you could always remove it before you sell. You'd almost certainly hire a new contractor. Even if you're never going to sell the house, you may want to get a new couch, or at the very least change a room's layout somewhere down the line. Yet software developers do it all the time. Distinguishing unrelated components encourages several coding best practices. In addition to introducing a modular design, meaning additional components could easily be added (or existing components removed) down the line, abstraction often yields objectively more stable and more readably maintainable code due to the abhorrence of the copy-and-paste effect. 

Justice Brandeis is famous for noting that "sunlight is the best disinfectant." Likewise, the transparency afforded by the open-source ethos produces more reliable software.

### Why Open Source and Government

## Open Source Community Building

Open source is referred to as a community, because that's what it is. Open source isn't a source of free labor or an avenue to sparaticly garner good will, nor is the release of open source software tantamount to the release of a press release or policy document. Open source is about fostering a space in which like-minded enthusiasts — coders, designers, user experience experts, even the users themselves — can come together and create something for their mutual benefit, a something which is almost without exception, greater than the sum of the individual parts. As such, when begining an open source project, special steps must be taken to encourage community involvement.

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

Licensing concerns itself with two things. (1) Who "owns" the code, and (2) who has the right to use it. When a coder develops code (or a painter paints, or a writer writes) he "owns" the code. Put another way, he holds the code's copyright, or is the code's copyright holder. If the coder would like to let others use his code, he would grant them a "license" to do so. Such a license would confer limited rights or guarantees (e.g., the right to use). This license is generally provided in writing along with the software.

Think about it like renting an appartment. The landlord owns the property, but via your lease, confers upon you certain rights (e.g., the right to live there), but also reserves certain rights (e.g., the right to tear down a wall). Software licensing is no different. The copyright holder holds all rights to the software, and can license out some or all of those rights as he sees fit.

### Copyright

In most open source projects (although not all), copyright is held by the individual code contributors. So, for example, while the Microsoft corporation may own the right to Microsoft Windows (and thus upon purchasing it, you receive a license for its use), the rights to the open-source content managment system, on the otherhand, are held by thousands of individual contributors scattered around the world who echo individually license to you the right to use the software free of charge. License and copyright, although related are wholy distinct.

### Types of Licenses

Although technically one could create their own license, the open source community has generally adopted a handful of standard licenses. These license are well known and well understood, and make using or contributing to the software easier.

Most licenses do three things. (1) Describe what rights the copyright holder is granting to you, (2) Disclaim that you cant sue the copyright holder if something goes wrong, (3) Require you to include the text of the license if you redistribute it to others.

#### MIT, BSD, Apache

Some licenses, such as the MIT, BSD, or the Apache license simply serve primarily to clarify that the software's recipient is getting virtually unlimited rights to the software, so long as they include the text of the license if they redistribute it or make a derrivatve work. Such licenses do not heavily restrict use of the software. For example, here's the text of the MIT license:

> Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

> The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
> THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

It is important to note that such licenses do not restrict the commercialization of software. If I produce module "foo" and release it under the MIT license, there is nothing stopping another from including that module in software "bar" and selling it under a proprietary (e.g. closed source) license.

#### GPL (Copyleft)

Another large class of licenses are called "Copyleft" licenses. They seek to use copyright law to ensure 

Releasing the project under GPL is done simply by (1) including the text of the license within the repository, (2) posting a boilerplate statement at the top of the main file that notes the licenses and releases subsequent distributors from liability, and (3) noting the license within the project's documentation.

### Derivative Works


### Government-Specific Considerations

Under 17 U.S.C. § 105, any code created by a government employee on government time is not subject to domestic copyright protection (essentially public domain) and would be licensed as a US Government Work. 

If a project is a derivative work of virally licensed code (e.g., the GPL, the most common open source license), it must be licensed under the same terms as the upstream project (e.g., a WordPress plugin or using a code snippet that was posted under the GPL) and the question of licensing is simple.

If a project does not use any previously licensed code, things can get a bit tricky, especially if you get a pull request from the public (e.g., do contributors surrender the rights to their work by contributing?). It is important to specify the means and terms under which the public can contribute to encourage collaboration. If possible, I would recommend including even a single line of GPL licensed code to simplify things, but you are free to require contributions be licensed under any license, including public domain (although I wouldn't recommend it). Sample language for a GPL'd project below:

[Example Licenses](licenses/)

#### Contractor-created code

Absent permission from the contracting officer, the US Government retains unlimited rights for all work created under contract. FAR 52.227-14(c)(1)(i). Even if the contracting officer grants such rights, they do not take effect unless the contractor includes a copyright notice, acknowledgement of government sponsorship, and the contract number along with the code at the time of delivery. See FAR 27.404(a)(5).

#### Government-created code

If a government employee contributes to a project on government time and within the scope of his employment, such code is considered a US Government Work. US Government Works are not entitled to copyright protection under US copyright law (commonly known as falling within the "Public Domain") but may receive copyright protection abroad, and thus should still be licensed accordingly. See 17 USC § 105. 

Additionally, if a derivative work under a viral license, the government is still bound by the terms of the original license, thus the project as a whole would be licensed under the original license. Put another way, if a government agency is granted limited rights by a copyright holder to use or redistribute a piece of software under the condition that any contributions to the software be redistributed under the same terms, the government does not have the right to release the software under a less restrictive or incompatable license.[^1]

#### Community-contributed Code

Generally speaking, the government may not accept volunteer services (such as software development) absent appropriate compensation for fear of running afoul of gift restrictions or the Administrative Procedures Act. *See generally* 31 U.S.C. § 1342. This has stymied public code contributions in the past. To mitigate this concern, project documentation should unambiguously declare the license under which the project is distributed (e.g, GPL, MIT) and that any code publicly posted in association with the project (e.g., pull requests, code comments) must be licensed under the same terms (not uncommon in normal open source projects as "terms of contribution"). 

Under such a model, the individual contributor will retain the copyright, and the publicly distributed code becomes legally indistinguishable from other publicly distributed code already used regularly by the government under the same type of open-source license (e.g., Drupal, WordPress, Apache), thus giving us legal authority to accept pull requests and other citizen-generated code.

Contributing
------------

Federal employees and members of the public are encouraged to contribute to the project by [forking](https://help.github.com/articles/fork-a-repo) and submitting a pull request. (If you are new to GitHub, you might start with a [basic tutorial](https://help.github.com/articles/set-up-git).) 

All contributors retain the original copyright to their code, but by contributing to this project, you grant a world-wide, royalty-free, perpetual, irrevocable, non-exclusive, transferable license to all users under the terms of the [Gnu General Public License v2](http://www.gnu.org/licenses/gpl-2.0.html) or later.

## Procurement

\[ This is a place holder. Please [feel free to contribute](how-to-contribute/). \]

## Additional Resources

1. Producing Open Source Software – Karl Fogel (Practical)
2. The Cathedral and the Bazar – Eric S. Raymond (Theoretical)
3. Understanding Open Source and Free Software Licensing – Andrew M St. Laurent (O'Reily)


# Todo

Free as in beer vs. free as in speech

[^1]: Theoretically, even though the government's contributed code, as a whole, would be bound by the copyleft license, individual blocks of code intirely independent from the parent work, may be removed by the public and used in another project free of restriction. This is an edge case and would only arise in the event of conflict.