# Scripts used in my thesis research

The enron folder contains a script to do the following:
* Extract all zips present in the defined directory.
* Convert all PST files (extracted from the zips) to individual EML files (recursively)
* Extract all attachments present in the EML files (recursively)
* Delete all not Excel related files (also leave the EML files) (recursively)
* Move the Excel sheets into one directory

This script is developed using Ubuntu 20.04. In order to execute this script, you need the
following additional packages installed:
* pst-tools (for extracting EML files from the PST)
* mpack containing the munpack executable (for extracting attachments from the EML files)

### Installation of additional packages
When using Ubuntu (or any debian based distributions), the above packages can be installed using
the following line in a terminal:

> sudo apt install pst-utils mpack
