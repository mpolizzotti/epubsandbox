# EPUB 3 Sandbox
* * *
The EPUB 3 Sandbox repository houses a basic implementation of the EPUB 3 specification. This repository is a sandbox for learning and understanding the EPUB 3 specification.

# What's Inside
This sandbox currently houses an example eBook entitled, **Do Horses Wear Socks?**. This is just a sample implementation of the EPUB 3 specification.

    META-INF
        - container.xml
    OEBPS
        images                      // Houses images
            - cover.jpg
            - preface-image.jpg
        text                        // Houses chapter content
            - 1-preface.xhtml
            - 2-chapter-1.xhtml
            - 3-chapter-2.xhtml
            - 4-chapter-3.xhtml
            - 5-chapter-4.xhtml
        - package.opf               // Package manifest
        - toc.ncx                   // Table of contents for older EPUB versions
        - toc.xhtml                 // Table of contents for latest EPUB versions
    - mimetype                      // application/epub+zip

# Create the EPUB Document
To create the EPUB document, navigate to the root eBook folder (i.e., do-horses-wear-socks) and execute the *zip* command on the directory. Running these commands will render the **do-horses-wear-socks.epub** package.

    cd ../epubsandbox/do-horses-wear-socks
    zip -0Xq ../do-horses-wear-socks.epub mimetype
    zip -Xr9Dq ../do-horses-wear-socks.epub * -x *.DS_Store

# Validate the EPUB Document
To validate the EPUB document, you can leverage the [Browser-based EPUB Validator Tool](http://validator.idpf.org/application/validate) or use the [Stand-alone EPUB Validator Tool](https://github.com/idpf/epubcheck)

# Viewing the EPUB Document
If your on an Apple Computer, double-click the **do-horses-wear-socks.epub** package. The EPUB document will automatically open with **iBooks** application.

