---
layout:	page
root: ..
title: Get in Touch, Help and Support (draft)
---

((TODO This is boilerplate for the most part - page should reflect how to contact when ShowYourWOrking is a going concern)).

## How to get in touch

E-mail {{ site.mailing_list }} with:

* Discussions about the deployment and use of {{ site.software_name }}.
* Information, hints and tips you think would be useful for other
  {{ site.software_name }}  users to know.
* Requests for features or changes to {{ site.software_name }} and/or its
  documentation. 
* Reporting bugs in {{ site.software_name }} or issues with the
  documentation. 
* Providing updates on bugs e.g. you find a fix for a bug you
  reported. 
* Information on presentations you will give or have given, or papers
  you have published, based on research to which 
  {{ site.software_name }} contributed. 

E-mail {{ site.email }} with:

* Requests for discussions relating to collaborations.
* Confidential questions or issues that you do not wish to make public.

Use our [issue tracker]({{ site.issue_tracker }}) for:

* Seeing a list of requested features and reported bugs.
* Requests for features or changes to {{ site.software_name }} and/or its
  documentation. 
* Reporting bugs in {{ site.software_name }} or issues with the
  documentation. 
* Providing updates on bugs e.g. you find a fix for a bug you
  reported. 

---

## How to get help

If you experience a problem when using {{ site.software_name }}, then:

* Check the user documentation and release notes for your release (if
  applicable) 
* Search {{ site.mailing_list }} [archive]({{ site.mailing_list_archive }}).
* Search our [issue tracker]({{ site.issue_tracker}}) for
  known problems and bugs (both fixed and open).

If you cannot find a solution, then you can do one of:

* E-mail {{ site.mailing_list }} with your request for help.
* Create a [new issue]({{ site.issue_tracker_new_issue }}).

See [How to ask for help](#how-to-ask-for-help), below, for advice on
what information you should provide.

### What is and is not supported

The following versions are supported:

* Source code releases with a version number.
* Binary releases with a version number.
* Tagged release versions in our Git repository.

The following versions are **not** supported:

* Any version in Git that is not a tagged release version.
* Modified versions released by third-parties.

### What support we offer

The {{ site.software_name }} team consists of members in a number of
organisations who work on a number of projects, and may be very
busy. {{ site.software_name }}'s support relies on the goodwill of
these members and organisations. Our support is 'best effort' (i.e.,
we'll do the best we can, given our other commitments).

---

## How to ask for help

* Submit only one request per report.
* State your platform, operating system and version.
* State the version of {{ site.software_name }} you are using:
  - If you are using a source code release then give the version
    number of that release. 
  - If you are using a binary release then you can get the version
    number by running:

~~~
$ ./TODO-SOFTWARE-NAME --version
~~~

  - If you are using a version from Git then give the commit hash
    of the version you are using:

~~~
$ git log -1
~~~

* Provide any error messages and exceptions that you see. 
  - If providing exceptions then provide these exactly as displayed in
    a terminal window. 
  - Do **not** provide a simple textual summary like 'It threw an
    error'. 
  - If using a graphical user interface, then see the next point.
* If using any graphical user interface and, if you think
  it would help, then send a copy of your display: 
  - Under Ubuntu, use the Print Screen key to save an image of your
    display into your home directory as a .png file. 
  - Under Windows, click CTRL and Print Screen, select Start =>
    All Programs => Accessories => Paint, click CTRL and V to 
    paste the image into Paint and then Save the image as a .png
    or .jpg file.
* If possible, provide a recipe for repeating the bug.
* Provide any other information you think will help.
* Clearly separate fact from speculation.

Requests of the form "I used {{ site.software_name }} and am stuck" are
not helpful to either you or us and people may suspect that you are
just a spammer or time waster.

No bug is too trivial to report - small bugs may hide big bugs.
