This is a small Bash script to remove empty pages from a PDF document.

I use it after scanning many pages with a paper feed scanner to a single PDF file. I usually scan in duplex mode though many pages are only used on one side. To get rid of the resulting empty pages in the PDF this script has been useful.

To run it `ghostscript` and `pdftk` are needed. Both programs can be easily installed in Linux using your package manager (e.g. `apt` in Debian and Ubuntu or `dnf` in Fedora). I've tried the script only in Linux.

The script is run by
```
./remove-blank-pages input-with-blank-pages.pdf output-without-blank-pages.pdf 
```

You can play with the ink coverage threshold determining if a page is considered blank or not in line 7 of the script.
