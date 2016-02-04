This Project will produce a set of classes and utilities for inputting and outputting various forms of land survey data from various equipment manufacturers for the purpose of manipulating that data in whatever manner is required by an end user.

Since the original author had immediate access to Leica Total Station and GPS data, as well as Lowrance Sonar data, this is where the project began.

The original inspiration for this project grew out of need to transform some Leica data into the form required for WOLFPACK least squares adjustment.

Another need grew from processing Lowrance sonar data files to determine to depths of a pond filled with something similar to water.

Since this project is primarily concerned with the nuts and bolts of the data, it will lack any kind of Graphical User Interface. As exe's are produced, they are to be simple command line programs suitable for a DOS prompt or a UNIX shell session.  GUI's, etc., belong in the realm of some other project based, in part, on this one.  In Carpentry terms, our job here is nail up very solid, pre-fab'd, wall frames; let someone else slap 'em together, dry wall/plaster/panel 'em, and then paint 'em however they like.

In general, for each type of survey data we will create a class. (Hopefully, one day, we will know enough to develop a generic base class suitable for all types of survey data.)  We will then implement the fundamental operations of reading the data from a file (or some other source) into the member variables of this class, and then outputting the member variables back to a file which is identical to the original file / source. This, unto itself, is sufficient.

As time goes on, we can implement useful operations on the data in the member variables of the objects of the class -- just as soon as we can agree on what is 'useful.'

This library contains an RFC 4180 compliant CSV reader/writer which can be used to output binary files into something human-readable and/or processable by another program (like WOLFPACK)

Very conscientious, but not Herculean, efforts have been made to keep the code platform independent. In cases where this was not possible, the offending lines were isolated to modules with the word "implementation" in their file names so that anyone developing for a non-ix86/windows/msys/mingw environment would be able to port the program with less difficulty.

As always, I hope that some or all of this might be useful to someone else, too.

If you have classes and/or utilities and/or exe's that sound like they belong in this project, and you're O.K. with GPL V3, please let me know, and I'll add them.


RK