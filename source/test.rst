
Indices and tables
==================

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`

.. figure:: /images/nport.png
   :width: 20%

.. Note::

  This function is not suitable for sending spam e-mails.

.. glossary::

 environment
    A structure where information about all documents under the root is
    saved, and used for cross-referencing.  The environment is pickled
    after the parsing stage, so that successive runs only need to read
    and parse new and changed documents.

 source directory
    The directory which, including its subdirectories, contains all
    source files for one Sphinx project.

.. productionlist::
   try_stmt: try1_stmt | try2_stmt
   try1_stmt: "try" ":" `suite`
            : ("except" [`expression` ["," `target`]] ":" `suite`)+
            : ["else" ":" `suite`]
            : ["finally" ":" `suite`]
   try2_stmt: "try" ":" `suite`
            : "finally" ":" `suite`

.. index::
   single: execution; context
   module: __main__
   module: sys
   triple: module; search; path

The execution context
---------------------

...


This is a normal reST :index:`paragraph` that contains several
:index:`index entries <pair: index; entry>`.