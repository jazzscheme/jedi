Jedi
====

Jedi is a fully programmable IDE for the Lisp family of languages.


License
-------

JazzScheme is released under a dual Mozilla Public License Version 1.1 or
GNU General Public License v2 or later. Choose whichever license you prefer.


Platforms
---------

Windows, Mac OS X / X11, Linux / X11


Distribution
------------

```
README                   :  Readme file
INSTALL                  :  Installation instructions

.git                     :  Git repository
.gitignore               :  File patterns ignored by Git
.gitmodules              :  Used by Git to manage submodules

jam                      :  JazzScheme Management System
configure                :  Placeholder for configure
make                     :  Placeholder for make

bin                      :  Default configuration binaries
build                    :  Custom configurations binaries
jazz                     :  Jazz repository as a Git submodule
lib                      :  Pre-installed packages
```


Building
--------

Please see INSTALL for details and examples on building Jedi.


Launching
---------

Launch
  Once you have built Jedi you can launch it using the jedi executable.

Debugging
  If you get an error before the IDE is fully functional, you will end up in
  the Gambit debugger. This is not as painful as would appear as JazzScheme
  code is very close to the generated Scheme code so that inspecting a Jazz
  stack inside the Gambit debugger is very easy. Having access to a lower level
  debugger is even a very nice feature as it is virtually impossible to crash
  the IDE even when modifying a critical piece of code (like inserting a bug in
  the view system for instance) as the Gambit debugger is completely self
  contained.

  If you get an error that brings you to the Gambit debugger, the console will
  automatically open. You can then use all of Gambit's debugging command to
  debug your code and when you are done, simply execute the (resume) command.
  This will resume the IDE's message loop making it again functional.


Documentation
-------------

Jedi documentation is available online at www.jazzscheme.org


------------------------------------------
Send comments, suggestions, bugs,... to:
gcartier@jazzscheme.org
