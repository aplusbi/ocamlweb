OCAMLWEB PROJECT
================
This is the source code implementing a new website for the OCaml
community. Information here is relevant only to developers and content
contributors. End-users of the website should simply visit the
website, which is currently being hosted at http://ocaml-lang.org. (It
is hoped that this site will eventually be served by the URL
ocaml.org, but that is not finalized yet.)


DEPENDENCIES
============
Building the html pages requires:

* ocaml
* [oasis](http://forge.ocamlcore.org/projects/oasis/)
* [weberizer](https://github.com/Chris00/weberizer)

Weberizer is Christophe Troestler's templating tool. It allows us to
easily provide a consistent design to multiple pages. You will only
need to understand this tool if you are contributing design
changes. Content contributors can focus on the pure html source within
src/html/.


BUILD
=====
Currently the site consists only of static html pages, and so can be
built and run entirely on a local machine without dependencies on
external file or database servers. Simply run:

    oasis setup
    make

This will generate a new folder 'www' that contains the full website.


PUBLISH
=======
Changes can be published by running:

    make publish

Of course, this is only allowed by the project administrators that
have write permission to the production server.


CONTACTS
========
You can reach the development team by posting to the [mailing
list](https://lists.forge.ocamlcore.org/cgi-bin/listinfo/ocamlweb-devel).

To begin contributing, visit the [master
repo](https://github.com/agarwal/ocamlweb) on github, click the Fork
button, make changes to your copy, and submit pull requests. It's that
easy!
