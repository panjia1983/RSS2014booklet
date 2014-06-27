

There are 3 different versions you can compile the booklet into: print, usbstick and online. To select the version, comment out the defines in the beginning of booklet.tex

===Print version===
Dont color links,  in some places (workshop homepages), links are printed as footnotes, and file names are used for papers instead
Rephrases some sentences to use reference to conference homepage instead of links

Before printing, load file into Adobe Pro and convert everything to cmyk color model 

===USB stick edition===
Papers and eduroam configuration is linked locally to the fiels on the usb stick

===Online edition===
links to online resources.
To make this file nice and small, execute ghostscript: 

gs -dNOPAUSE -dBATCH -sDEVICE=pdfwrite -dCompatibilityLevel=1.4 -dPDFSETTINGS=/ebook -sOutputFile=booklet.online.pdf booklet.pdf


