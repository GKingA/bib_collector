# bib_collector

Do you have some latex files relying on one big bibtex?
Do you want to migrate some of it to a new file?
Then this little script is for you.

You just need to pass the tex files and your previous bib file 
to the bibliography.py script, specify the output bib file
and you are done. If the specified output file wasn't empty, don't worry
the script will check which are the missing elements and add them 
to the file.


Usage:

````
python bibliography.py [-h] [-t TEX [TEX ...]] [-b BIB] [-o OUT]

optional arguments:
  -h, --help            show this help message and exit
  -t TEX [TEX ...], --tex TEX [TEX ...]
                        List the latex files you want to gather the citations
                        from
  -b BIB, --bib BIB     The bib files to check for the citations
  -o OUT, --out OUT     The output bib file. The bib file can be non-empty and
                        it will be checked for existing citations.
````