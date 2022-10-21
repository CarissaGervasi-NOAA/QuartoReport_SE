# QmdReport.

Example of a Quarto Report with dynamically created tables

Presentation given on this Aug 11 2022: https://youtu.be/Uay6X65Ukvk. The version given in that talk is Release v2.0.

## What is this doing?

* Dynamic tables and figures where the table number, table caption, number of tables is all dynamically created based on the data set
* Table cross-refs that just work across formats
* Figures that look good across formats and it "just works"---with the caveat that I am using {flextable} for Word/html and {kableExtra} for PDF.
* A custom title page for PDF.
* Link to source code, post issue, edit source code right on the HTML for each page.
* Link to download the PDF and Word. This is auto-generated. None of this is manual.
* HTML that looks good across different sized displays (big screen and phone screen)

## How about?

* {gt} is great. Why not use that for tables? It was not playing nice with Quarto+PDF and broke all table numbering in subsequent tables (flextable or kabelExtra or markdown). I reported the bug and I think the {gt} developers have fixed for the next update.

## Can't {bookdown} do this?

Kind of. I love {bookdown} and I have written multiple on-line books with it but 

* there were a lot of hacks and tricks needed for cross-refs and it would tend to break when you needed multiple formats (PDF, HTML and Word). 
* Lack of solid cross-ref working across formats is a deal-breaker for government reports.
* The ability to use "@" to find your cross-refs that you can do with Visual mode in RStudio... I can't live without that now. 
* Quarto still has some hacks, but many many fewer. A lot of stuff seems to just work.


_____________________________________________________________________________________________________________
Disclaimer:

This repository is a scientific product and is not official communication of the National Oceanic and
Atmospheric Administration, or the United States Department of Commerce. All NOAA GitHub project code is
provided on an ‘as is’ basis and the user assumes responsibility for its use. Any claims against the Department of
Commerce or Department of Commerce bureaus stemming from the use of this GitHub project will be governed
by all applicable Federal law. Any reference to specific commercial products, processes, or services by service
mark, trademark, manufacturer, or otherwise, does not constitute or imply their endorsement, recommendation or
favoring by the Department of Commerce. The Department of Commerce seal and logo, or the seal and logo of a
DOC bureau, shall not be used in any manner to imply endorsement of any commercial product or activity by
DOC or the United States Government.
