<!-- Locked by waynegramlich on 2017Sep9 to do initial development. -->

# Ubiquity Robotics Documentation Standard

This document describes the Ubutity Robotics documentation formating
and writing standards.

## Formating Standards

In general, the documentation is written in standard
[Markdown](https://daringfireball.net/projects/markdown/syntax)
format.  Period.
t
### Formatting Extensions

The current intention is to seriously consider using
[GitHub Pages](https://pages.github.com/).
This means that some of the github extensions will be endorsed as well.
In general, do not use any GitHub extensions unless they are listed below.
Github Pages provide some extensions to Markdown format.  In addition,
Github Pages uses
[Jekyll](https://jekyllrb.com/docs/home/).
We may decide to incorporate some Jekyll features into the UR formatting
standards.  Only use Markdown and Jeykll features that have been
agreed upon and incorporated into this document.  Please see the
lists below.

#### Acceptable GitHub Markdown Extensions

There are currently no agreed upon Github Markdown extensions.

#### Acceptable Jekyll Extentions

There are currently no agreed upon Jekyll extensions.

## Formatting Guidelines

Some formatting guidelines are listed immediately below:

* Directory Per Page:
  Each Markdown document should be in its own directory.
  Since markdown provides a way to include images, almost images associated
  with the page are colocated in the directory in the that has the markdown page.
  This means when the page is no longer needed, the entire directory can be deleted.

* Dirctory Names:
  If the directory is named `foo`, the markdown file should be need `foo.md`.
  Directory names should somewhat descriptive without getting overly long.
  For now directory names should be somewhere be 10 to 25 characters long.
  This is a guideline rather than a hard and fast rule.  Do not label directories
  with chapter numbers (e.g. `chapter1`, `chapter2`, et.c)
  Directory names should be all lower case with underscores ('_') between words.
  Long words like "documenatation" and "miscellaneous" can be sorted down to
  "doc" and "misc", respectively.  Do not do do vowel removal.  Thus, shortening
  "documentation"  and "miscellaneous" down to "dcmnttn" and "mscllns" is not
  acceptable.

* Images:
  Pictures are saved with a suffix of `.jpg`.  Screen snapshots are saved with
  as suffix of `.png`.  The Markdown syntax for an image is:

  >        \![Alterative Text][URL]

  Please put something in alternative text to describe the image.  URL's
  should always use relative syntax.  Most of the images are colocated in
  the same directory, so the URL's have the form of `image_name.jpg` or
  `image_name.png`.

* Global Images Directory:
  Some images are used over and over again.  This images are stored in a
  global top level directory named `assets/`.  Do not go wild stuffing images
  into the `assets` directory.  Each image that goes goes in there should
  be an obviously sharable image.  Some examples are `loki.jpg`, `magni.jpg`,
  `robots.jpg`, etc.

* Links:
  The format for a link is:

  >        ![Link Text](Link URL)

  Try to embed the link into a sentence.  Do not use the cheat of "click here"
  for link text.   If the URL is to a page local to the repository, use relative
  links.  If the URL is to another repository, use a full URL.

* Line Wrapping:
  Currently, there is no standard for line wrapping.  If you like your paragraphs
  to reside on a single line, that is quite acceptable.  Breaking a paragraph
  so that there is line wrapping is quite acceptable.  The arbitrary buffer
  width of 100 characters is assumed for line chopping.  Links and image

## Writing Style

Documentation is easier for the customer to read if everybody uses similar
writing style.  The list of writing style recommendations is listted below:

* Tense:
  The dominate tense to use is the present tense.  Only use the past tense
  to document depricated features.  Only use future tense infrequently, and
  then only to describe features that have not been implemented and are not
  likely to be implemented soon.

  If you are documenting a feature that has not been implemented yet, but will
  be implemented relatively soon, please write the documenation in the present
  tense.  Some sort of marker is needed to flag documented features that have
  not been implemented yet.  For now, just use `Not Implemented:` at the
  beginning of each paragraph or section that is not implemented.

* Pronouns:
  Documentation tends to be easier to read if it is documentation team having
  a conversation with the customers.  Thus, use "we" and "us" to refer to the
  UR development team and "you" and "your" to refer to the customers.

* Textual References:
  Sometimes you need to refer to some text elsewhere in the page.  Back references
  text earlier in the page should use the term "above".  Forward references to
  text later in the page, should use the term "below".  The term "immediately below"
  means that the text shows up within a paragraph or two.  The term "much further below"
  means that the text shows up many paragraphs below.  Do not fall into the trap
  using past/future tense to 

* Robot Names:
  Only use specific robot names when talking about a feature that is specific
  to that robot.  Thus, "Magni" and "Loki" are to be used only features that
  are specific to the Magni and Loki robot platforms.  Use the phrase "your robot"
  to refer to a generic robot (i.e. the customer's robot.)  This allows Ubiquity
  Robots to add a new platform without having to do a massive edit.

* Acronyms:
  The first time you use an acronym on a page, follow the acronym with
  a parenthetical expansion of the phase with the appropriate letters capitalizes.
  You may use the UR (Ubiquity Robotics) without having to do the expansion.

## Documentation Workflow

* Typographical and Gramatical Errors:
  Members of the UR team should fix these immediately on the GitHub site.
  Use the comment "Fixed some typos" to mark these.

* Locking:
  When somebody is going to do a massive reedit of a page, you should "lock"
  the page with a comment of the following form:

  >        \<!-- Locked by USER_NAME on YYYYMMMDD for REASON. -->

  where:

    * USER_NAME is the github user name for the person doing the locking.

    * YYYYMMMDD is date where YYYY is the year, MMM is a three character
      month (e.g. "Sep",  "May", ...) and DD is the day.
      
    * REASON is a very short reason why the page is locked.
    
  {locking needs a bit more explanation.}

## Conclusion

{conclusion goes here.}