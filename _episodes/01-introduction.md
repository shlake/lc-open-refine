---
title: "Introduction to OpenRefine"
teaching: 10
exercises: 0
questions:
- "What is OpenRefine? What can it do?"
objectives:
- "Explain what the OpenRefine software does"
- "Explain how the OpenRefine software can help work with data files"
keypoints:
- "OpenRefine is 'a tool for working with messy data'"
- "OpenRefine works best with data in a simple tabular format"
- "OpenRefine can help you split data up into more granular parts"
- "OpenRefine can help you match local data up to other data sets"
- "OpenRefine can help you enhance a data set with data from other sources"
---

## What is OpenRefine?
What is OpenRefine?

- OpenRefine is a Java program that runs on your machine (not in the cloud): it is a desktop application that uses your web browser as a graphical interface. No internet connection is needed, and none of the data or commands you enter in OpenRefine are sent to a remote server.
  - OpenRefine does not modify your original dataset. All actions are easily reversed in OpenRefine and you can capture all the actions applied to your data and share this documentation with your publication as supplemental material.OpenRefine saves as you go. You can return to the project at any time to pick up where you left off, or export your data to a new file.
 - OpenRefine can be used to standardise and clean data across your file.

It can help you:

* Get an overview of a data set
* Resolve inconsistencies in a data set, for example standardizing date formatting
* Help you split data up into more granular parts, for example splitting up cells with multiple authors into separate cells
* Match local data up to other data sets, for example in matching local subjects against the Library of Congress Subject Headings
* Enhance a data set with data from other sources

Some common scenarios might be:

* Where you want to know how many times a particular value (name, publisher, subject) appears in a column in your data
* Where you want to know how values are distributed across your whole data set
* Where you have a list of dates which are formatted in different ways, and want to change all the dates in the list to a single common date format. For example:

| Data you have   | Desired data |
|-----------------|:-------------|
| 1st January 2014| 2014-01-01   |
| 01/01/2014      | 2014-01-01   |
| Jan 1 2014      | 2014-01-01   |
| 2014-01-01      | 2014-01-01   |

* Where you have a list of names or terms that differ from each other but refer to the same people, places or concepts. For example:

| Data you have   | Desired data |
|-----------------|:-------------|
| London          | London       |
| London]         | London       |
| London,]        | London       |
| london          | London       |

* Where you have several bits of data combined together in a single column, and you want to separate them out into individual bits of data with one column for each bit of the data. For example going from a single address field (in the first column), to each part of the address in a separate field:

| Address in single field | Institution  | Library name  | Address 1 | Address 2 | Town/City | Region | Country | Postcode |
|-------------------------|:-------------|:-------------|:-------------|:-------------|:-------------|:-------------|:-------------|:-------------|
| University of Wales, Llyfrgell Thomas Parry Library, Llanbadarn Fawr, ABERYSTWYTH, Ceredigion, SY23 3AS, United Kingdom | University of Wales | Llyfrgell Thomas Parry Library | Llanbadarn Fawr | | Aberystwyth | Ceredigion | United Kingdom | SY23 3AS |
| University of Aberdeen, Queen Mother Library, Meston Walk, ABERDEEN, AB24 3UE, United Kingdom | University of Abderdeen | Queen Mother Library | Meston Walk | | Aberdeen | | United Kingdom | AB24 3UE |
| University of Birmingham, Barnes Library, Medical School, Edgbaston, BIRMINGHAM, West Midlands, B15 2TT, United Kingdom | University of Birmingham | Barnes Library | Medical School | Edgbaston | Birmingham | West Midlands | United Kingdom | B15 2TT |
| University of Warwick, Library, Gibbett Hill Road, COVENTRY, CV4 7AL, United Kingdom | University of Warwick | Library | Gibbett Hill Road | | Coventry | | United Kingdom | CV4 7AL |

* Where you want to add to your data from an external data source:

| Data you have   | Date of Birth from VIAF (Virtual International Authority File) | Date of Death from VIAF (Virtual International Authority File) |
|-----------------|:-------------|:-------------|
| Braddon, M. E. (Mary Elizabeth) | 1835 | 1915 |
| Rossetti, William Michael       | 1829 | 1919 |
| Prest, Thomas Peckett           | 1810 | 1879 |

## Basics of OpenRefine

You can find out a lot more about OpenRefine at [http://openrefine.org](http://openrefine.org) and check out some great [introductory videos](https://www.youtube.com/channel/UCqwSVsJ8CWD9pQUZDbJC1ew). There is a [Google Group](https://groups.google.com/forum/?hl=en#!forum/openrefine) that can answer a lot of beginner questions and problems. There is also an [OpenRefine Google Plus community](https://plus.google.com/communities/117280693504889048168) where you can find a lot of help, especially from community members from the life sciences. OpenRefine [recipes](https://github.com/OpenRefine/OpenRefine/wiki/Recipes), scripts, projects, and extensions are available too, where you can find and copy them into your OpenRefine instance to run on your dataset.

The OpenRefine GitHub wiki page has a [reference](https://github.com/OpenRefine/OpenRefine/wiki/GREL-Functions) of the General Refine Expression Language (GREL).

## Features

* Open source ([source on GitHub](https://github.com/OpenRefine/OpenRefine)).
* A large growing community, from novice to expert, ready to help.
* Works with large-ish datasets (100,000 rows). Does not scale to many millions. (yet).

