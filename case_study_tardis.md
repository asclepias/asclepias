

This case study examimes the role of "style" in the analysis of citations for Tardis.  **It is not complete or vetted**

Tardis refers in this case study to an aggregation of a software proxy article, software identifiers, and versioned software DOIs about `tardis`, a tool that creates synthetic observations (spectra) for exploding stars (supernovae). 
In the literature the most frequently cited work for mentions of this tool is a software proxy article published in **MNRAS** in 2014 (Kerzendorf & Sim 2014); there are 43 citations as of today for this software proxy in [NASA ADS](https://ui.adsabs.harvard.edu/abs/2014MNRAS.440..387K/abstract).
The first ADS indexed entry for Tardis is the corresponding "accepted" **arXiv** preprint of this MNRAS article (January 2014).
Tardis appears to have been on **GitHub** since January 2012 and has 17 tags and 10 releases.
Through the GitHub=>Zenodo workflow the developers have created 8 **Zenodo** versioned software DOIs.
An **ASCL** identifier was created for Tardis in February 2015.

A tabulation of all object PIDs or descriptive articles is given in the Table below.

This case study did not  analyze the ways the various research objects were curated, linked, or used. 
Nevertheless it does consider the developer's preferred citations for this work, how these varied over the development of the software, and how these preferred citations are affected by "style."
Early literature focused citations list two main contributors, Kerzendorf & Sim.  
Presently the [preferred citation(s)](https://tardis-sn.github.io/tardis/credits.html) for `tardis` include the 2014 **MNRAS** software proxy article and also the citation of a versioned Zenodo software DOI.
The current versioned software citataion request is for v3.0.a2; last updated 5 May 2019 [95b565c](https://github.com/tardis-sn/tardis/commit/95b565c798f57cc03438d84b0948fbbf762cad56)).
The use of the versioned software DOI to distribute credit goes back somewhat further than version 3. 
Prior to v3 developement the developers were listing the concept DOI of `tardis` (doi:10.5281/zenodo.592480) in their citation instructions.
Further, a comment given in the description metadata of the Version v2.0.2 Zenodo software DOI, *"first official zenodo release with all authors,"* suggests that the developers intended at this instance to use the software DOI as a means to directly credit inividual contributors to the Tardis software.

Aside: it might be worth noting that the preferred software DOI is 1 version out of date (pointing to v3.0.a2 instead of v3.0.a3) because release documentation cannot point to a software DOI that won't exist until the release is fixed and made.

**PID and Authorship Table**

| Entry  | PID | Date |  Authors | Comments |
| ----------- | --- | :------: | :---: | -------------------|
arXiv | arXiv:1401.5469 | Jan 2014 | [2](https://arxiv.org/abs/1401.5469) | v1 "accepted by MNRAS" 
ASCL.net | ascl:1402.018 | Feb 2014 | [2](https://web.archive.org/web/20190927143030/http://ascl.net/1402.018) | Code entry last updated [2017-12-15](http://ascl.net/phpBB3/viewtopic.php?t=32935)
MNRAS article | doi:10.1093/mnras/stu055 | May 2014 | [2](https://doi.org/10.1093/mnras/stu055) | Primary software citation proxy (43)
Zenodo v1.0.1 | doi:10.5281/zenodo.17630 | May 2015 | [13](https://doi.org/10.5281/zenodo.17630) | tardis: v1.0.1
Zenodo v2.0 | doi:10.5281/zenodo.1213132 | Apr 2018 | [29](https://doi.org/10.5281/zenodo.1213132) | tardis-sn/tardis: TARDIS v2
Zenodo v2_test1 | doi:10.5281/zenodo.1213671 | Apr 2018 | [29](https://doi.org/10.5281/zenodo.1213671) | tardis-sn/tardis: TARDIS test release
Zenodo v2_test2 | doi:10.5281/zenodo.1213676 | Apr 2018 | [3](https://doi.org/10.5281/zenodo.1213676) | 3 ORCIDs 
Zenodo v2.0.2 | doi:10.5281/zenodo.1292315 | Jun 2018 | [33](https://doi.org/10.5281/zenodo.1292315) | 7 ORCIDs, "first official zenodo release with all authors" 
Zenodo v3.0.a1 | doi:10.5281/zenodo.2589622 | Mar 2019 | [33](https://doi.org/10.5281/zenodo.2589622) | tardis-sn/tardis: TARDIS v3.0 alpha1
Zenodo v3.0.a2 | doi:10.5281/zenodo.2590539 | Mar 2019 | [33](https://doi.org/10.5281/zenodo.2590539) | tardis-sn/tardis: TARDIS v3.0 alpha2
Zenodo v3.0.a3 | doi:10.5281/zenodo.2799539 | May 2019 | [33](https://doi.org/10.5281/zenodo.2799539) | tardis-sn/tardis: TARDIS v3.0 alpha3

This Version v2.0.2 software was archived to Zenodo in June 2018. 
We took this as a starting point to review the literature for mentions of the Tardis software and review how these were cited in the literature. 
We categorized recent uses of `tardis` and documented what research objects were cited.
A tabulation of all the mentions of "tardis" in the literature since June 2018 is given in the Table below. 
The list is a join of two ADS queries:
1) a full text search for "tardis" that removes non-supernova related papers;
2) a reference search for the Proxy 2014 paper.

Each manuscript was read and the mention of tardis extracted. 

| BibCode mentioning tardis | Mention type                                       | Reference Processing
|     :---                  | :----                                              | :----
|     2018A&A...614A.115M   | failed to cite the software DOI                    | 
|     2018SSRv..214...72R   | tangential mention of code; did not use            |
|     2018MNRAS.477.3425B   | failed to cite the software DOI                    |
|     2018ApJ...865L...3P   | cited Software DOI (v2.0.2)                        | Sent to Asclepias broker
|     2018MNRAS.480.3609B   | dropped Software DOI inline to the text (footnote) | 
|     2018A&A...620A.156E   | mentioned but did not use the software             |
|     2019A&A...621A..29V   | failed to cite the software DOI                    |
|     2019Natur.565..324I   | cited the ASCL record                              |    
|     2019A&A...622A.102M   | cited the software DOI (v2.0.2)                    | Not sent to broker
|     2019ApJ...871..250H   | cited the software DOI (v2.0.2)                    | Sent to Asclepias broker
|     2019MNRAS.484.4785M   | dropped the software DOI inline to the text (ackno)|
|     2019ApJ...876..148C   | mentioned but did not use the software             | 
|     2019AstL...45..276P   | mentioned but did not use the software             |
|     2019arXiv190611206P   | mentioned but did not use the software             |
|     2019arXiv190604205B   | mention code by proxy; did not use software        |
|     2019LRCA....5....1N   | cited the software DOI (v2.0.2)                    | Sent to Asclepias broker
|     2019PrPNP.107..109K   | mention code by proxy; did not use software        |
|     2019arXiv190803001K   | cited the software DOI  (v3.0-alpha2)              | v 3.0-alpha.2 DOI; Not sent to broker
|     2019MNRAS.487.2538J   | mentioned but did not use the software             | 
|     2019arXiv190904545M   | has not yet cited the code. ;-)                    |


The software proxy article was cited for all 19 instances above. 
This include mentions where `tardis` was not named, but the software was discussed through a citation to Kerzendorf & Sim (2014).
Of these 8 articles did not in fact use the software, and it is not clear that a versioned software citation would be appropriate or rational when software hasn't been used.

For the remaining 11 cases, versioned software was listed in the reference section of the preprint article 5 times.
Twice more the authors "mentioned" a versioned software DOI by dropping the URL into the text (footnote or acknowledgements) instead of properly citing it in the reference section.
Overall this means that authors as users of `tardis` tried to "cite" a versioned software DOI 64% of the time since June 2018.

But trying to cite software and succeeding in a way that can be counted (by an index like ADS) yield two different outcomes. 
Dropping a software DOI URl in to the main text of a paper  will not result in a citation counted by ADS and thus not transmit credit to the 31 additional contributors to this project not listed in Kerzendorf & Sim (2014).
Twice again the proper bibliographic citation of the software DOI was not detected by the ADS reference matching algorithm. 
These two latter instances provide the source of the remaining discussion in this case study. 




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
