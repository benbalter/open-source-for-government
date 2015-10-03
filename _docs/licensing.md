---
title: Licensing
---

# Licensing Generally
Licensing concerns itself with two things. (1) Who "owns" the code, and (2) who has the right to use it. When a coder develops code (or a painter paints, or a writer writes) he "owns" the code. Put another way, he holds the code's copyright, or is the code's copyright holder. If the coder would like to let others use his code, he would grant them a "license" to do so. Such a license would confer limited rights or guarantees (e.g., the right to use). This license is generally provided in writing along with the software.

Think about it like renting an apartment. The landlord owns the property, but via your lease, confers upon you certain rights (e.g., the right to live there), but also reserves certain rights (e.g., the right to tear down a wall). Software licensing is no different. The copyright holder holds all rights to the software, and can license out some or all of those rights as he sees fit.

# Copyright
In most open source projects (although not all), copyright is held by the individual code contributors. So, for example, while the Microsoft corporation may own the right to Microsoft Windows (and thus upon purchasing it, you receive a license for its use), the rights to the open-source content management system, on the other hand, are held by thousands of individual contributors scattered around the world who echo individually license to you the right to use the software free of charge. License and copyright, although related are wholly distinct.

# Types of Licenses
Although technically one could create their own license, the open source community has generally adopted a handful of standard licenses. These license are well known and well understood, and make using or contributing to the software easier.

Most licenses do three things. (1) Describe what rights the copyright holder is granting to you, (2) Disclaim that you cant sue the copyright holder if something goes wrong, (3) Require you to include the text of the license if you redistribute it to others.

## MIT, BSD, Apache
Some licenses, such as the MIT, BSD, or the Apache license simply serve primarily to clarify that the software's recipient is getting virtually unlimited rights to the software, so long as they include the text of the license if they redistribute it or make a derivative work. Such licenses do not heavily restrict use of the software. For example, here's the text of the MIT license:

> Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

> The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

> THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

It is important to note that such licenses do not restrict the commercialization of software. If I produce module "foo" and release it under the MIT license, there is nothing stopping another from including that module in software "bar" and selling it under a proprietary (e.g. closed source) license.

## GPL (Copyleft)
Another large class of licenses are called "Copyleft" licenses. They seek to use copyright law to ensure that source code remains in the public domain by requiring that derivative works of a copyleft licensed project be released under the same (or compatible) conditions.

Releasing the project under GPL is done simply by:
1. Including the text of the license within the repository,
2. Posting a boilerplate statement at the top of the main file that notes the licenses and releases subsequent distributors from liability, and
3. Noting the license within the project's documentation.

### Derivative Works
Any derivative work of a copyleft licensed projects must be released under the same or similar terms. Some popular copyleft licensed projects are WordPress and Drupal, two popular content management systems, both of which are licensed under the GPL.

A derivative work is a legal term of art, but in layman's terms, is any work that requires the former to function. So, in the above example a Drupal or Wordpress theme, plugin or module, which theoretically could not stand alone from the original, would be considered a derivative work if it uses the CMS's API. A stand alone CMS inspired by, but completely unrelated to (say written in a different language), however, would most likely not be considered derivative and could be licensed under any license.

The term derivative work also applies, more traditionally to forks and improvements upon the original codebase for which the above logic still applies. If I take the WordPress core files, change one line, and then distribute it, I am still bound by the terms of the GPL.

### Distribution Requirement
Note however, the terms of the GPL don't kick into affect until the software is _distributed_. In that sense, an agency can take a GPL'd piece of software (say Drupal), expand upon it (e.g., by writing a module to produce custom functionality), and are not required to distribute it (e.g., the module may remain closed source).

Once the module is distributed however (e.g., posted online, shared with others outside the organization), the GPL requirements kick in and it must be licensed under the term so of the GPL.

# Dual Licensing
Some projects may be dual licensed. This is most often the case when something is offered to the public under the terms of both the GPL **and** and another license such as MIT. In this sense, most developers would chose the less restrictive MIT flavor for their project. However, if I have an existing GPL'd project and am looking to include the software, having the option to use the project under the GPL is attractive and simplifies under what terms I provide my software to others. It also resolves potential incompatibility between your license and the GPL.

To dual license software, simply note in the project's readme that the file is available under both licenses. No additional steps are necessary. When downstream developers use the software, they will chose what license they use it under (again, without taking any additional steps). This is most often the case with add-on frameworks such as jQuery which are likely to be incorporated in existing projects down stream.

# Government-Specific Considerations
There is [a strong presumption](http://ben.balter.com/2012/07/26/government-release-of-source-code-public-domain-or-open-source/) toward open source in government-produced software.

Under 17 U.S.C. § 105, any code created by a government employee on government time is not subject to domestic copyright protection (essentially public domain) and would be licensed as a US Government Work.

If a project is a derivative work of virally licensed code (e.g., the GPL, the most common open source license), it must be licensed under the same terms as the upstream project (e.g., a WordPress plugin or using a code snippet that was posted under the GPL) and the question of licensing is simple.

If a project does not use any previously licensed code, things can get a bit tricky, especially if you get a pull request from the public (e.g., do contributors surrender the rights to their work by contributing?). It is important to specify the means and terms under which the public can contribute to encourage collaboration. If possible, I would recommend including even a single line of GPL licensed code to simplify things, but you are free to require contributions be licensed under any license, including public domain (although I wouldn't recommend it). Sample language for a GPL'd project below:

[Example Licenses](licenses/)

## Contractor-created code
Absent permission from the contracting officer, the US Government retains unlimited rights for all work created under contract. FAR 52.227-14(c)(1)(i). Even if the contracting officer grants such rights, they do not take effect unless the contractor includes a copyright notice, acknowledgement of government sponsorship, and the contract number along with the code at the time of delivery. See FAR 27.404(a)(5).

## Government-created code
If a government employee contributes to a project on government time and within the scope of his employment, such code is considered a US Government Work. US Government Works are not entitled to copyright protection under US copyright law (commonly known as falling within the "Public Domain") but may receive copyright protection abroad, and thus should still be licensed accordingly. See 17 USC § 105.

Additionally, if a derivative work under a viral license, the government is still bound by the terms of the original license, thus the project as a whole would be licensed under the original license. Put another way, if a government agency is granted limited rights by a copyright holder to use or redistribute a piece of software under the condition that any contributions to the software be redistributed under the same terms, the government does not have the right to release the software under a less restrictive or incompatable license.[^1]

## Community-contributed Code
Generally speaking, the government may not accept volunteer services (such as software development) absent appropriate compensation for fear of running afoul of gift restrictions or the Administrative Procedures Act. _See generally_ 31 U.S.C. § 1342. This has stymied public code contributions in the past. To mitigate this concern, project documentation should unambiguously declare the license under which the project is distributed (e.g, GPL, MIT) and that any code publicly posted in association with the project (e.g., pull requests, code comments) must be licensed under the same terms (not uncommon in normal open source projects as "terms of contribution").

Under such a model, the individual contributor will retain the copyright, and the publicly distributed code becomes legally indistinguishable from other publicly distributed code already used regularly by the government under the same type of open-source license (e.g., Drupal, WordPress, Apache), thus giving us legal authority to accept pull requests and other citizen-generated code.

[^1]: Theoretically, even though the government's contributed code, as a whole, would be bound by the copyleft license, individual blocks of code entirely independent from the parent work, may be removed by the public and used in another project free of restriction. This is an edge case and would only arise in the event of conflict.
