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

  * No one can change the `slug` of a file. It is set in stone (mostly).
  * Refrain from renaming files.
  * Use British English (God save the Queen)


Contributing
------------

Feel free to create pull requests for any typos or grammatical mistakes.

For more significant changes, [make an issue][issue] to discuss the change first.

[make an issue]: https://github.com/penguoir/nextstep-content/issues/new


Sponsors
--------

To sponsor this project, send an email to <contact@nextstep.sh>.


