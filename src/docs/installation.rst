******************
Installation Guide
******************

.. warning::

    Haplodon is still experimental. It may have bugs and features are subject to change.

There are multiple ways to install haplodon:

Pixi
~~~~
Haplodon can be installed globally using `pixi <https://pixi.sh/>`_:

.. code-block:: bash

    pixi global install haplodon

Bioconda
~~~~~~~~
Haplodon is available via `Bioconda <https://bioconda.github.io>`_. With Bioconda set up,
installation is as easy as:

.. code-block:: bash

    conda install haplodon -c conda-forge -c bioconda -c nodefaults

Pay attention to the correct channel ordering for the installation.

Cargo
~~~~~
If the `Rust <https://www.rust-lang.org/tools/install>`_ compiler and associated
`Cargo <https://github.com/rust-lang/cargo/>`_ are installed, haplodon may be installed via:

.. code-block:: bash

    cargo install haplodon

Source
~~~~~~
Download the source code and within the root directory of the source run:

.. code-block:: bash

    cargo install --path .
