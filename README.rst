=================
`faker-file-wasm`
=================
.. _faker-file: https://github.com/barseghyanartur/faker-file
.. _online-demo: https://faker-file-wasm.vercel.app/
.. _Pyodide: https://pyodide.org/en/stable/

`Pyodide`_ based WASM frontend for `faker-file`_ Python package. Check the `online-demo`_.

Running locally
===============
Open the index.html file in your favourite browser.

Usage examples
==============

.. code-block:: python

    from faker import Faker
    from faker_file.providers.txt_file import TxtFileProvider
    from faker_file.providers.zip_file import ZipFileProvider

    FAKER = Faker()
    FAKER.add_provider(TxtFileProvider)
    FAKER.add_provider(ZipFileProvider)

    txt_file = FAKER.txt_file()
    zip_file = FAKER.zip_file()
    
    print(txt_file.data)
    print(zip_file.data)

Writing documentation
=====================

Keep the following hierarchy.

.. code-block:: text

    =====
    title
    =====

    header
    ======

    sub-header
    ----------

    sub-sub-header
    ~~~~~~~~~~~~~~

    sub-sub-sub-header
    ^^^^^^^^^^^^^^^^^^

    sub-sub-sub-sub-header
    ++++++++++++++++++++++

    sub-sub-sub-sub-sub-header
    **************************

License
=======
MIT

Support
=======
For security issues contact me at the e-mail given in the `Author`_ section.

For overall issues, go to `GitHub <https://github.com/barseghyanartur/faker-file-wasm/issues>`_.

Author
======
Artur Barseghyan <artur.barseghyan@gmail.com>
