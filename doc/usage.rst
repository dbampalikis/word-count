

Usage
=====


How to clone the code
---------------------

In order to fork the repository visit the `link <https://github.com/dbampalikis/word-count>`_


Make
----

Generate all results:

::

  $ make -f Makefile_all


Snakemake
---------

Define the rules for the workflow in the file Snakemake, located in the root folder. To run the workflow use the snakemake command.
A rule can be define as following
::

  rule alldata:
	input:
		'processed_data/isles.dat',
		'processed_data/abyss.dat',
		'processed_data/last.dat',
		'results/results.txt'

The included rules are the following:
	1. runall
	2. zipf_test
	#. count_words
	#. clean

Where to find the results
-------------------------

The results are located in the /results folder
