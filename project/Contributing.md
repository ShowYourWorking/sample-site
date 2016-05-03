---
layout:	page
root: ..
title: How to Contribute (draft)
---

((TODO - Make this reflect best practice for how to contribute when ShowYourWorking becomes a going concern - mailing lists etc))

Anyone can contribute to {{ site.software_name }}, regardless of their
skills, as there are many ways to contribute. There follows a summary
of what contributions can be made, how they are made, any conditions
the contributions must conform to, and the process followed by the
project in accepting the contribution.  

All contributions are under the terms of the Contributor Licence
Agreement and Certificate of Origin detailed below.

---

## Information on how our software has helped you

E-mail us at {{ site.mailing_list }} or {{ site.email }}.

If you are praising any aspect of {{ site.software_name }} we will
thank you profusely and ask if we can quote you on our web site.

If you have published a paper, based on research to which 
{{ site.software_name }} contributed, we will add an entry for
this to our [Research](../research/index.html) page.

We may ask if you'd like to write a case study for our web site.

---

## Tutorials on using or developing our software for research

E-mail us at {{ site.mailing_list }} or {{ site.email }}.

Provide any source code or data files that are needed by your
tutorial.

We will work through your tutorial and check it for readability and
correctness. If there are issues, we'll work with you to resolve
these.

We will add your tutorial to the documentation. Your name will be kept
on its pages. We will also add you to our
[Contributors](#contributors).

---

## Changes to the web site or documentation

EITHER e-mail us at {{ site.mailing_list }} or {{ site.email }}

OR submit a pull request against the *gh-pages* branch of 
[{{ site.doc_repository }}]({{ site.doc_repository }}).

We will review your proposed changes. If there are issues, we'll work
with you to resolve these. 

We will update the web site or documentation. For case studies, your
name will be kept on its pages. We will also add you to our
[Contributors](#contributors).

---

## Feature or enhancement requests or bug reports

EITHER e-mail us at {{ site.email }} or use the GitHub issue tracker at ((TODO fork and rename chembiohub_helpdesk)) and create a  [new ticket]({{ site.issue_tracker_new_issue}}).

See [Get in Touch, Help and Support](./HelpAndSupport.html) for what
information to provide.

We will check that the feature has not been requested or the bug has
not been reported, implemented or fixed, already. If it has been
reported, implemented or fixed already, we'll let you know.

---

## Features, enhancements or bug fixes

Before you submit a feature, enhancement or bug fix, make sure that:

* Your code confirms to the {{ site.software_name }} [coding
  standards](../developer/CodingStandards.html). 
* You have written automated tests (either new tests, or updates to
  existing tests) to test your feature or bug fix.
* You have list of steps required to test your feature.
* You have a list of changes to required to the documentation that are
  incurred by your feature or bug fix.

EITHER e-mail us at {{ site.mailing_list }} or {{ site.email }}. Include:

* EITHER a `.tar.gz` file or `.zip file` with your code.
* OR a patch file created using the Linux/UNIX `diff` command.  
* If you modified a source code release then give the version
  number of that release. 
* If you are using a version from Git then give the commit hash
of the version you modified (if you have commited any local
changes to your Git repository then give the commit hash for
the commit prior to your local changes):

~~~
$ git log
~~~

OR submit a pull request against the *gh-pages* branch of 
{{ site.code_repository }}.

We will check that your code compiles, that your code conforms to the 
{{ site.software_name }} coding standards, and that your tests
pass. We will also review your code. We will run though the list of
steps to test your feature and validate any documentation you
provide. If there are issues, we'll work with you to resolve these.

Once complete, we will merge your code into the 
{{ site.software_name }} trunk and add you to our
[Contributors](#contributors).
 
---

## Contributors

The following people have contributed to this code under the terms of
the Contributor Licence Agreement and Certificate of Origin detailed
below:

* NAME, EMAIL, AFFILIATION, WHAT WAS CONTRIBUTED
* NAME, EMAIL, AFFILIATION, WHAT WAS CONTRIBUTED
* NAME, EMAIL, AFFILIATION, WHAT WAS CONTRIBUTED
* ...

---

## Contributor Licence Agreement and Certificate of Origin

By making a contribution to this project, I certify that:

(a) The contribution was created in whole or in part by me and I have
    the right to submit it, either on my behalf or on behalf of my
    employer, under the terms and conditions as described by this file;
    or

(b) The contribution is based upon previous work that, to the best of
    my knowledge, is covered under an appropriate licence and I have
    the right or permission from the copyright owner under that licence
    to submit that work with modifications, whether created in whole or
    in part by me, under the terms and conditions as described by
    this file; or

(c) The contribution was provided directly to me by some other person
    who certified (a) or (b) and I have not modified it.

(d) I understand and agree that this project and the contribution
    are public and that a record of the contribution (including my
    name and email address) is maintained indefinitely and may be
    redistributed consistent with this project or the licence(s)
    involved.

(e) I, or my employer, grant all recipients of this software a
    perpetual, worldwide, non-exclusive, no-charge, royalty-free,
    irrevocable copyright licence to reproduce, modify, prepare
    derivative works of, publicly display, publicly perform,
    sub-licence, and distribute this contribution and such
    modifications and derivative works consistent with this project or 
    the licence(s) involved or other appropriate open source
    licence(s) specified by the project and approved by the 
    [Open Source Initiative (OSI)](http://www.opensource.org/), for
    code, or other appropriate [Creative
    Commons](http://creativecommons.org/) licence(s) specified by the
    project, for documentation.

(f) If I become aware of anything that would make any of the above
    inaccurate, in any way, I will let {{ site.email }} know as soon
    as I become aware.

(The {{ site.software_name }} Contributor Licence Agreement and
Certificate of Origin is inspired by the UK Met Office FCM Contributor
Licence Agreement and Certificate of Origin which was, in turn,
inspired by the Certificate of Origin used by Enyo and the Linux
Kernel.)
