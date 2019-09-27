

This case study examimes the role of "style" in the analysis of citations for Tardis.  **It is not complete or vetted**

Tardis is <introduction about the Tardis aggregation of research objects>. 

A tabulation of all the mentions of "tardis" in the literature since September 2018 is given below. 
The list is a join of two ADS queries:
1) a full text search for "tardis" that removes non-supernova related papers;
2) a reference search for the Proxy 2014 paper.

Each paper was read and the mention of tardis extracted. 

| BibCode mentioning tardis | Mention type                                       | Reference Processing
|     :---                  | :----                                              | :----
|     2018ApJ...865L...3P   | cited Software DOI (v2.0.2)                        |   Sent to broker
|     2018MNRAS.480.3609B   | dropped Software DOI inline to the text (footnote) | 
|     2018A&A...620A.156E   | mentioned but did not use the software             |
|     2019A&A...621A..29V   | failed to cite the software DOI                    |
|     2019Natur.565..324I   | cited the ASCL record                              |    
|     2019A&A...622A.102M   | cited the software DOI (v2.0.2)                    | Not sent to broker
|     2019ApJ...871..250H   | cited the software DOI (v2.0.2)                    | Sent to broker as 2019arXiv190201904H
|     2019MNRAS.484.4785M   | dropped the software DOI inline to the text (ackno)|
|     2019ApJ...876..148C   | mentioned but did not use the software             | 
|     2019AstL...45..276P   | mentioned but did not use the software             |
|     2019arXiv190611206P   | mentioned but did not use the software             |
|     2019arXiv190604205B   | mention code by proxy; did not use software        |
|     2019LRCA....5....1N   | cited the software DOI (v2.0.2)                    | Sent to broker
|     2019PrPNP.107..109K   | mention code by proxy; did not use software        |
|     2019arXiv190803001K   | cited the software DOI  (v3.0-alpha2)              | v 3.0-alpha.2 DOI; Not indexed; not sent to broker
|     2019MNRAS.487.2538J   | mentioned but did not use the software             | 
|     2019arXiv190904545M   | has not yet cited the code. ;-)                    |

We draw attention to three specific mentions of tardis and their outcome with respect to detection of the citations. 





### bibliographic style

The bibliographic style used by an author to prepare a preprint can result in the stripping of the DOI from the metadata the author collected to write a manuscript.
In the instance of 2019arXiv190803001K the author utilized LaTeX packages that resulted in the stripping of the DOI from their bibtex source file.
Specifically the authors used the outdated `apj.bst` style file, which treats `@misc` (or any non-article type) in such a way that the DOI is not included in the string version of the reference that appears in the PDF of the manuscript. 
Without the DOI in the string reference, a bibliographic index such as ADS will find it difficult to match the reference string uniquely to a registered record (there's more to this than that). 

The AAS Journals updated their bibtex style file in 2016 to support DOIs for `@misc` objects. This new style file, `aasjournal.bst` is avaiable . I has a number of other changes, including providing inline anchored strings for DOIs, arXiv, and ASCL identifiers. 
Stylistically it chooses to render these are fully expressed strings -- in otherwords, we made a choice to add the PID string **in full** in the text rather than anchoring it to related identifying material. 
This is to ensure that preprints created with our tools had unambigious identifiers. 

### production style

An author submitted manuscript is converted to a final PDF/XML/HTML research paper through automated parsing of the original manuscript.
Here we mean that the original form of a manuscript could have many formats: PDF, TeX, XML (or subsets such as DOCX), or HTML. 
Whatever means is necessary to 
In other words, as with the compilation of a LaTeX document, the conversion process by a vendor requires a style that may or may not be updated with an awareness of the new style (for software citations).

We think an example is this arXiv preprint for 2019A&A...622A.102M. The preprint (arXiv:) has the DOI for the software citation of tardis (v2.0.2). It is present in all forms of the preprint. It was/was not encoded as bibtex by the authors. 

However the final production version of this article, the DOI for the zenodo citation has been stripped away in the metadata for the article XML as submitted to ADS. Without the ADS in the XML, ADS cannot index the citation and pass it to the Asclepias broker. 

We speculate that the removal of this DOI during the production of this article is a function of **production style** used by the vendors related to EDP Sciences.
We make this speculation based on the fact that most production vendors transform author manuscripts to XML via . 
We note that although the entry in the preprint is typed as an article, the final type is "book"

### transmutation style

To submit data to CrossRef a fully self contained JATS/XML document is transformed into a metadata version through the use of an XLST style sheet. 

If that style sheet is unaware of upstream changes to the production style then it will behave unexpectedly.

For the AAS/IOP journals we found that the metadata transmitted to CrossRef had at least three types of identifiers stripped from the bibliographic: arXiv identifiers, ASCL identifiers and software DOIs. 

There may be any of a number of other identifiers that are not submitted to CrossRef and thus are not made available to 


### summary

Style acts as a filter against information transmitted in scholarly manuscripts. 
Sometimes this filter has a net positive effect, rendering unclear language or grammar usage normative.
Yet for the adoption of new styles in published manuscript this style can be destructive, removing important bits of information that were in the original text written by the author.

This document describes instances of three such style filters and their impact on software citation. 
