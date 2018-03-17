## Resources for Modern 61A in Python

- [Course website for Spring 2018](https://cs61a.org/)
- [Course website for Spring 2017](http://www-inst.eecs.berkeley.edu/~cs61a/sp17/)
- [Course website for Summer 2017](http://www-inst.eecs.berkeley.edu/~cs61a/su17/)
- [Textbook for Modern 61A in Python](http://www.composingprograms.com/projects.html)

## Resources for classic 61A & revised 61AS in Racket & Scheme

### SICP Textbooks

- [Better Looking Online SICP Textbook](http://sarabander.github.io/sicp/)
Online SICP Textbook
- [Equivalent Online Textbook provided freely by MIT Press](https://mitpress.mit.edu/sicp/full-text/book/book.html)
- [SICP translated to Python](https://www.gitbook.com/book/wizardforcel/sicp-in-python/details)
- [SICP translated to Javascript](https://www.comp.nus.edu.sg/~cs1101s/sicp/)

### Simply Scheme Textbook
- A well-written gradual introduction to CS.
- Serves as a handy introduction if it is your first time programming.
- Reading this textbook is a lesson 0 pre-work for classic 61.
- [Simply Scheme Textbook](https://people.eecs.berkeley.edu/~bh/ss-toc2.html#variables)

### Classic 61A Lecture
- Note that the last lecture was given in Spring 2011.
- [Course Webpage](https://inst.eecs.berkeley.edu/~cs61a/sp11/)
- [Course Outline](https://inst.eecs.berkeley.edu/~cs61a/sp11/0.pdf)
- [Video Lectures](https://archive.org/details/ucberkeley-webcast-PL3E89002AA9B9879E)
- [Lecture Notes](https://inst.eecs.berkeley.edu/~cs61a/reader/notes.pdf)

### Modern 61AS

- [Course Archives](https://inst.eecs.berkeley.edu/~cs61as/archives.html)
- [61AS (Self-Paced) in Racket & Scheme (in the spirit of classic 61A) - 2013 Course](https://edge.edx.org/courses/uc-berkeley/cs61as-1x/SICP/about)
- [Spring 2013 Course Resources](https://inst.eecs.berkeley.edu/~cs61as/sp13/)
- [Spring 2016 Course Resources (Latest)](http://berkeley-cs61as.github.io/textbook.html)
- Enrol and you’ll get access to a course outline that is  useful for providing you with some structure.

### Additional Useful Notes

#### About Racket

- The language Racket, a dialect of Lisp, is used in the modern 61AS course.
- It is a general-purpose programming language as well as the world’s first ecosystem for developing and deploying new languages.

#### Installing Racket

- [Racket's Mac Installation Guide
(Using Homebrew)](http://brewformulas.org/racket)

```bash
# Starts Racket REPL (Read-Eval-Print Loop)
> racket
# Starts DrRacket IDE (a cooler env for running racket program)
> drracket
```
- [Downloading Racket from website](http://racket-lang.org/download/)

#### Installing Racket Libraries (Important)
- Downloading Racket itself if not sufficient to follow the online 61AS textbook. The textbook uses procedures that the language does not natively provide. You will need to install some additional libraries to follow along. Instructions on how to install these libraries can be found below.
- Do note that following the classic SICP text in Scheme also requires additional libraries. The additional library provided below for Racket is also useful for following Scheme.
- [This library adds a Simply Scheme teaching language into DrRacket; the language that is used in the online textbook:](http://planet.racket-lang.org/package-source/dyoo/simply-scheme.plt/2/1/planet-docs/manual/index.html)

```clojure
#lang planet dyoo/simply-scheme:2

#Add the above line at the top of DrRacket's IDE to get access to useful helper procedures defined by Simply Scheme.
```

#### Documentation for Racket

- [Documentation](https://racket-lang.org/)
- [Other Reference Materials for Lisp](https://www.tutorialspoint.com/lisp/lisp_program_structure.htm)
