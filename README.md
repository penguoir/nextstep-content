nextstep-content
================

The content for [nextstep.sh][nextstep]. Changes are pushed automatically to
the staging site, which is promoted to master once a contributor checks the
changes.

[nextstep]: https://nextstep-prod.herokuapp.com


File structure
--------------

  * Syllabuses are saved in the root as directories.
  
  * Each syllabus has an `index.md` file which holds the following:

    * `title`: Title of the syllabus
    * `slug`: slug of the syllabus
    * `parts`: an array of folder names

  * Parts are saved as directories alongside the `index.md` file. The `parts`
  array specifies the name of the directory.

  * Each part has an `index.md` file which holds the following:
  
    * `title`: Title of the part
    * `slug`: Slug of the part
    * `chapters`: an array of filenames
    * `content` (as markdown): Introduction to that part

  * Chapters are saved as markdown files. They are saved alongside the part's
  `index.md` file. The `chapters` array references the file name of the chapter.

  * Each chapter has the following:
  
    * `title`: Title of the chapter
    * `slug`: Slug of the chapter
    * `content` (as markdown): Content of the chapter


### Rules

  * Don't change the `slug` of a file. It is set in stone.
  * Refrain from renaming files.
  * Use British English (God save the Queen)


Contributing
------------

Feel free to create pull requests for any typos or grammatical mistakes.

For more significant changes, [make an issue][issue] to discuss the change first.

[issue]: https://github.com/penguoir/nextstep-content/issues/new

### The source files

Keep the source files neat. They should be readable without needing any
external software. Users should not be required to use the Blue Paper website.

Make link text long so mobile users can click it easily.


### Key words

- **Read through**: Read the text, and understand the main concepts. If
  something doesn't make sense, re-read, searh online, or ask your tutor for
  help.

- **Skim through**: Read the text, understanding the main concepts, but don't
  worry if something doesn't make sense.

- **Work through**: The next link is a tutorial. Follow the steps in the
  tutorial making sure to understand why everything works. Play around with
  what you're doing as well, trying to push your knowledge.

- **Make**: Build, using any references you'd like, your ideal version of the
  following.

- **Try out**: Follow the steps shown in this guide, but don't worry about
  understanding how everything works.


Sponsors
--------

To sponsor this project, send an email to <contact@nextstep.sh>.


