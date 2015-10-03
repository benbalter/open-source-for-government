---
title: Open source community building
---

Open source is referred to as a community, because that's what it is. Open source isn't a source of free labor or an avenue to sporadically garner goodwill from Silicon Valley, nor is the release of open source software tantamount to the release of a press release or policy document. Open source is about fostering a space in which like-minded enthusiasts -- coders, designers, user experience experts, even the users themselves -- can come together and create something for their mutual benefit, a something that is almost without exception, greater than the sum of the individual parts. As such, when beginning an open source project, special steps must be taken to encourage community involvement.

#### Encouraging Community Involvement
Simply [making the code public is not enough](http://ben.balter.com/2012/04/10/whats-missing-from-cfpbs-awesome-new-source-code-policy/). Open source developers want to get behind a cause. Think of it as analogous to volunteering for a political campaign. They want to know what the project stands for, and where it is going. If they contribute, what will their code be used for in a six months or a year?  As a result, open source project documentation (readme) commonly includes four primary pieces of information:
1. A project mission statement, philosophy, or goal,
2. A features and requirements list, or long-term project roadmap, and most importantly
3. The status of the project (active development, beta, etc.)
4. How to submit an issue/feature request or contribute a fix/enhancement

For help getting started, including other common sections, please see the [example readme](example-readme/).

#### Mechanics
Creating an open-source project requires the project finder to stand up several pieces of critical infrastructure. It's not enough to simply make the code available, for example, as a zip file. Steps must be taken to ensure transparency and conversational, rather than announcement-driven communications. The goal here should be to make it as easy as possible for developers to find the project, grab the code, use it, and potentially contribute back. Most commonly, this infrastructure consists of:
1. Version control,
2. Bug tracking ("issues" in GitHub parlance),
3. Packaging for downloading, and
4. Documentation hosting (in GitHub's case, a wiki).

#### Communications
Beyond the obvious initial announcement publicizing the release, there are several forms of ongoing communication that may require a bit of planning prior to release. Most successful, large-scale projects have a two-way (note: not announcement only) mailing list, to facilitate interaction among developers, as well as an official IRC channel or other real-time chat forum. Alternatively, many projects use the open-source collaboration tool [P2](http://p2theme.com) to coordinate development efforts. The goal here is to provide a means by which developers can communicate with one another (rather than with the agency); to make a web rather than a hub and spoke. If two like-minded developers would like to contribute to a project, they shouldn't have to go through an intermediary (e.g. the agency) to do so.

#### Have the discussion in public
No matter how trivial the issue, make the discussion open. Even if issues are hashed out in-person, memorialize the conversation on the project's official communications channels. This does a few things: First, it creates a record of the decision, so that down the road, you (or more likely other contributors) can understand your reasoning. Second, it helps break down the us/them mentality, by showing the community respect and broadening the decision-making process. Last, and most helpful, engaging the community has the potential to generate more discourse, and thus more ideas and better decision.

#### Upkeep
Beyond the code itself, best practices dictate that maintaining an open-source project requires significant day-to-day upkeep and may entail both policy and technical decisions. Agencies should empower a team of trusted developers with decision-making authority to:
1. Individually respond to any issues opened by users ("tickets"),
2. Accept or reject [pull requests](#pull_requests) on behalf of the project, and
3. Coordinate future releases.

The key here, however, is not to institute a traditional governance structure. Informality is the cornerstone of open source and collaborative development and is the key to its agility. Code commits should be early, often, and public (as apposed to say, committing privately and "open sourcing" once a week). If such a policy were to be overlaid, most if not all the benefits of open source outlined above would be offset by the added overhead.

_See also, [GitHub as a Social Network](#culture)._

#### Governance
Most government projects are governed by a model known by its tongue-and-cheek name "benevolent dictatorship" (as opposed to democratic consensus building). This is not a bad thing. Almost all projects begin this way, and many major projects (including popular projects like Drupal and WordPress) remain this way today.

The term simply means that ultimate decision-making authority rests in a single individual or groups of individuals, rather than by vote of the community as a whole. To be successful, this model will require significant management and delegation of development efforts around:
1. Patching,
2. Translations,
3. Documentation and FAQs,
4. Issue tracking, and
5. Support

#### Delegation
The benevolent dictatorship model is arguably the norm for open-source software development, but it must be noted that organization and delegation of such efforts fall squarely on the agency's shoulders. You would be hard-pressed to find a successful open source project that does not have at least one full-time developer or community organizer.

#### Committer Status
In the long term, individual contributors will emerge as key project stakeholders based on the quality and quantity of code contributions and involvement in day-to-day discussions. It is common to grant such contributors committer status (the ability to commit code to the project, accept pull requests, etc.). This is arguably a necessary step for the project's continued evolution.
