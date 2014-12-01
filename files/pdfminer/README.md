ferguson-grand-jury-transcripts/pdfminer
========================================

This is a script that parses the XML files created by running [pdf2txt.py](http://www.unixuser.org/~euske/python/pdfminer/index.html#pdf2txt) (PDFMiner) on the [OCR Transcripts](https://www.dropbox.com/s/67unqhdrb8jhgr0/Ferguson%20Grand%20Jury%20Testimony.pdf?dl=0).

The XML files generated by PDFMiner preserve formatting information which we can use to more accurately identify text attributed to individuals whose names have been redacted from the transcript, by examining text indentations.

The XML file of the full transcript can be generated with the command:

`pdf2txt.py -o ferguson_grand_jury_testimony.xml Ferguson\ Grand\ Jury\ Testimony.pdf`