
Stingray refers in this case study to an aggregation of articles and preprints, codebases and archived releases about `stingray`, a library in Python built to perform time series analysis and related tasks on astronomical light curves.
This aggregation includes
a [GitHub repository](https://github.com/StingraySoftware/stingray) created in October 2015 and
five tagged GitHub [releases](https://github.com/StingraySoftware/stingray/releases) with the first issued in February 2018. 
The authors submitted a [code article](https://doi.org/10.21105/joss.01393) to JOSS in April 2019 and after [its review](https://github.com/openjournals/joss-reviews/issues/1393) was accepted in June 2019.
There are also [five archived Zenodo versions](https://doi.org/10.5281/zenodo.1490116) (plus a Concept DOI that currently points to the latest release, [v0.1.3](https://doi.org/10.5281/zenodo.3242835)).
The Stingray code was assigned an [ASCL identifier](http://ascl.net/1608.001) in August 2016.
The code has been described in an [arXiv preprint](https://arxiv.org/abs/1901.07681), having two versions posted in January and August 2019. 
The two arXiv versions roughly correspond to the submitted and accepted version of an [ApJ article](https://doi.org/10.3847/1538-4357/ab258d) that was published in final form in August 2019. 

### ADS Indexing 1: Where to put the preprint
Stingray has proven instructive for testing many aspects of our Asclepias investigations into the software citation ecosystem. 
The first instruction has been to improve how ADS indexes and matches the many types of objects in this aggregation. 
For instance ADS indexed the preprint **arXiv** version of the **ApJ** article (January 2019) and this was matched to the **JOSS** article, which was indexed by ADS (June 2019) instead of the later published **ApJ** article (August 2019).  
This match precipitated from the requirement of the JOSS+ApJ review process that the two articles have exactly the same title (and author list -- see Authorship table below).
This merge was manually repaired in ADS, and the weighting system for matching **arXiv** preprints with **JOSS** articles modified.
The initial merge meant that the **JOSS** article initially inherited all citations (and references in) the **arXiv** preprint.

### ADS Indexing 2: Indexing related Zenodo objects
Second the only indexed *version* of the Software `stingray` in ADS is v0.1.
This version is indexed because it was cited in the references of the JOSS article. 
The JOSS article's metadata (in the Atom RSS and in CrossRef metadata) contain relations that point to v0.1.3 (`<archive_doi>https://doi.org/10.5281/zenodo.3242835</archive_doi>` in the RSS feed and `relation": {"references": ["id-type": "doi", "id": "https://doi.org/10.5281/zenodo.3242835",` in the CrossRef metadata).
Currently, ADS treats this related identifier as a "data link", which is not indexed; 
we are considering that it should be indexed as an associated work.

### Metadata on Titles and Authors
Third, we were able to audit the titles and authors listed for the many Stingray objects. 
Tabulations of the authors and titles are given below. 
One possible inference is that objects that have undergone curation (e.g., peer-review, e.g., managing/production editor review) have authorship and titles that have converged (notwithstanding letter case that may result from Journal style).


**PID and Authorship Table**

| Entry  | PID | Date |  Authors | Comments |
| ----------- | --- | :------: | :---: | -------------------|
ASCL.net | ascl:1608.001 | Aug 2016 | [5](https://web.archive.org/web/20190925160413/http://ascl.net/1608.001) | Code entry last updated [2019-08-27](http://ascl.net/phpBB3/viewtopic.php?t=34066)
Zenodo test_release | doi:10.5281/zenodo.1490117 | Nov 2018 | [24](https://doi.org/10.5281/zenodo.1490117) | Concept DOI:10.5281/zenodo.1490116 
arXiv | arXiv:1901.07681 | Jan 2019 | [12](https://arxiv.org/abs/1901.07681) | v1==v2; ~sameAs submitted & accepted to ApJ
Zenodo v0.1 | doi:10.5281/zenodo.3239519 | Jun 2019 | [27](https://doi.org/10.5281/zenodo.3239519) | 0 ORCIDs
Zenodo v0.1.1 | doi:10.5281/zenodo.3242825 | Jun 2019 | [28](https://doi.org/10.5281/zenodo.3242825) | 0 ORCIDs; JOSS submission
Zenodo v0.1.2 | doi:10.5281/zenodo.3242829 | Jun 2019 | [12](https://doi.org/10.5281/zenodo.3242829) | 3 ORCIDs
Zenodo v0.1.3 | doi:10.5281/zenodo.3242835 | Jun 2019 | [12](https://doi.org/10.5281/zenodo.3242835) | 3 ORCIDs; at close of JOSS review
JOSS article | doi:10.21105/joss.01393 | Jun 2019 | [12](https://doi.org/10.21105/joss.01393) | 3 ORCIDs
ApJ article | doi:10.3847/1538-4357/ab258d | Aug 2019 | [12](https://doi.org/10.3847/1538-4357/ab258d) | 4 ORCIDs; accepted May 2019

**Title Table**

| Entry  | Date |  Title | Comments |
| ----------- | :------: | :---: | -------------------|
ASCL.net | Aug 2016 | Stingray: Spectral-timing software | Code entry last updated [2019-08-27](http://ascl.net/phpBB3/viewtopic.php?t=34066)
Zenodo "test_release" | Nov 2018 | StingraySoftware/stingray: this is a test | first Zenodo indexed name
arXiv | Jan 2019 | Stingray: A Modern Python Library For Spectral Timing | v1==v2
Zenodo v0.1 | Jun 2019 | StingraySoftware/stingray: Version 0.1 | 
Zenodo v0.1.1 | Jun 2019 | StingraySoftware/stingray: JOSS paper | 
Zenodo v0.1.2 | Jun 2019 | stingray: A modern Python library for spectral timing | 
Zenodo v0.1.3 | Jun 2019 | stingray: A modern Python library for spectral timing | 
JOSS article | Jun 2019 | stingray: A modern Python library for spectral timing | 
ApJ article | Aug 2019 | Stingray: A Modern Python Library for Spectral Timing | Title case from Journal style?


### Links or Relations between objects
The fourth exercise we were able to undertake using Stingray is a review of the types of "links" or relations between these research objects.
These links are itemized in the Table below.
They are varied in origin, syntax, and directionality. 
Note that the relation types ("predicates") either come from the source itself, e.g., "Described in" is the ASCL term or from the metadata schema of the article, e.g., "hasPreprint" is from CrossRef. 
Finally, citations in the reference section of an article use the predicate "cites", while a relationship between associated work uses "references."

Some of the relationships are absorbed directly (or created) by ADS, and expressed in their user interface and API results.
These exposed relationships include **arXiv** to **ApJ** article and **ASCL** to **ApJ** article, as well as any citation-type relationship, e.g., **JOSS** citing **Zenodo**.
We note that in this instance the **arXiv** to **ApJ** link is inferred by ADS; it need not be. 
Such a link could be created [by the author in arXiv](https://arxiv.org/help/jref), or captured by the AAS Journals when the manuscript is accepted and expressed through metadata to CrossRef (*"hasPreprint"*).

Relationships that exist but are not exposed in ADS include **Zenodo** to **Zenodo** DOI versions and **Zenodo** (or **ASCL**) to **GitHub** links.
Note that the link between the **JOSS** article and the **Zenodo** software object is currently exposed as a ''data link'' rather than as an ''Associated Work'' in ADS.
One question we have is if relations such as these should be discovered and indexed (ingested into) by ADS, exposing them to the reader as additional associated works in the ADS UI. 
This gives the benefit of discovering codebases or code versions via ADS, yet adds significant complexity to the ADS system.

Relationships that *should* exist but are not explicit and cannot be expressed include **JOSS** to **ApJ** relation (either via citation or other informative predicate), nor **ApJ** to **Zenodo** via direct software citation. 
Citations between these objects could be enforced as a matter of editorial policy; informative relations, e.g., that a non-citation relation exists between the parallal peer-review done by **JOSS** and **ApJ** could be added via CrossRef metadata ([*"references"* or maybe *"hasRelatedMaterial"*](https://support.crossref.org/hc/en-us/articles/214357426-Relationships-between-DOIs-and-other-objects)). 
The final **ApJ** article probably should have cited the "final" **Zenodo** object (v0.1.3), fulfilling part of the AAS Journal's software policy which states that, [*"Ideally, both forms of citation should be included"*](https://journals.aas.org/policy-statement-on-software/).  


**Linking Table**

Relationship | Predicate | Exists? | Comments 
--- | :-: | :-: | ---
JOSS => Zenodo v0.1 | "cites" | Yes | In [CrossRef](https://api.crossref.org/v1/works/10.21105/joss.01393)
JOSS => Zenodo v0.1.3 | "references" | Yes | In [CrossRef](https://api.crossref.org/v1/works/10.21105/joss.01393)
arXiv => ApJ | "DOI" | Yes | *magic* 
ApJ => arXiv | "hasPreprint" | No | *AAS could collect & IOP could export*
ApJ => Zenodo | "cites" | No | *but should it?!?*
JOSS <=> ApJ | "cites" | No | *Not required*
JOSS <=> ApJ | "references" | No | *but there's branding* 
ASCL => GitHub | "Code site" | Yes | Only on [ASCL](https://web.archive.org/web/20190925160413/http://ascl.net/1608.001)
ASCL => ApJ | "Described in" | Yes | [ADS Associated Work](https://ui.adsabs.harvard.edu/abs/2019ApJ...881...39H/abstract)
ASCL => ApJ | "Preferred citation" | Yes | Only on [ASCL](https://web.archive.org/web/20190925160413/http://ascl.net/1608.001)
Zenodo => Github | "IsSupplementTo" | Yes | Datacite; all versions [example](https://api.datacite.org/dois/application/vnd.datacite.datacite+json/10.5281/zenodo.1490117)
Zenodo => arXiv | "IsSupplementTo" | Yes | DataCite; v0.1.2, [v0.1.3](https://api.datacite.org/dois/application/vnd.datacite.datacite+json/10.5281/zenodo.3242835)
Version DOI => Concept DOI | "IsVersionOf" | Yes | DataCite; all versions, e.g. [v0.1.2](https://api.datacite.org/dois/application/vnd.datacite.datacite+json/10.5281/zenodo.3242829)
Concept DOI => Version DOI | "HasVersion" | Yes | [DataCite](https://api.datacite.org/dois/application/vnd.datacite.datacite+json/10.5281/zenodo.1490116)

### Discussion

 * The role of curation in the creation of these research objects
 * Who creates what to which link when and how?
 * Associated works in ADS's UI


