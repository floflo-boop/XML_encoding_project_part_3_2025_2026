# XML_encoding_project_part_3_

In this repository, you will find two folders.

The first one contains my custom ODD, RNG, and HTML files derived from this custom ODD, as well as the XSL document used to create the ODD from my previous XML file.

The second folder contains three XML documents that validate against my RNG file, along with two documents used as external lists in those three files.

No files have been modified, except for the necessary changes required to match the new RNG.

<br>

# AI use statement

AI was used on this occasion in an “emergency case.” Despite many attempts, I encountered significant difficulties with the Schematron part. Most of these issues were resolved by myself.

When I first tried to validate the files, the Schematron rule concerning the use of `@xml:lang` appeared to work only partially and not on all the specified elements. After many attempts and extensive research, I was unable to identify the cause of the problem and so unable to find solutions.

At that point, I used generative AI to help resolve the issue. It turned out that the problem was related to namespaces: the TEI namespace was not declared in my Schematron rules nor referenced in my XPath expressions. This caused the rule to behave incorrectly. The AI identified this issue; I then made the necessary changes, and the validation worked as expected.