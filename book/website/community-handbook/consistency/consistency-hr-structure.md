(ch-consistency-hr-structure)=
# Hard Requirements - Structure

The hard requirements in the consistency checklist ensure that _The Turing Way_ prioritises accessibility, collaboration, readability and ease of use. The requirement that deal with structure include: 

(ch-consistency-hardreqs-checkfour)=
## Check 1: Remove empty files from the `_toc.yml`

The `_toc.yml` file is where _The Turing Way's_ Table of Contents (ToC) lives.
Some files included in the ToC are empty, and their inclusion means that readers are able to navigate to them while reading _The Turing Way_.
This negatively impacts the reader's experience as they go through the book.

```{figure} ..\..\figures\empty_toc_file.png
---
height: 373px
name: empty_toc_file
alt: A screenshot of an empty file that was included in the Turing Way's Table of Contents.
---
Figure 3: A screenshot of an empty file that was included in the Turing Way's Table of Contents.
```

A general suggestion is to remove references to such files from the ToC and raise an issue in _The Turing Way_ Github [repo](https://github.com/alan-turing-institute/the-turing-way) for content to be written for those files. When content is written for them, they can then be added to the ToC.

For example, [this issue](https://github.com/alan-turing-institute/the-turing-way/issues/1391) curates a list of empty and incomplete files currently in _The Turing Way_, and 
[this PR](https://github.com/alan-turing-institute/the-turing-way/pull/1448) will write content for the `Data Licences` subchapter shown in the {ref}`image <empty_toc_file>`.

(ch-consistency-hardreqs-checkfive)=
## Check 2: Ensure chapters follow a consistent structure

_The Turing Way_ is made up of five guides that contain several chapters and subchapters. 
However, these chapters do not follow a uniform structure, taking away from the reader's experience.

```{figure} ..\..\figures\recommended_chapter_structure.png
---
height: 174px
name: recommended_chapter_structure
alt: A screenshot of the recommeded structure for chapters in the Turing Way.
---
Figure 4: A screenshot of an empty file that was included in the Turing Way's Table of Contents.
```

The recommended structure for chapters is shown in the {ref}`image <recommended_chapter_structure>`.
The landing page of the chapter should include information about any prerequisites required to understand the chapter, a summary of the chapter's content, and an explanation of why the chapter is useful.
While a chapter can contain as many or as little subchapters as necessary, it should also contain a separate checklist and resources section.
The checklist section itemises action points for the reader to take based on the concepts introduced in the chapter.
The resources section points the reader to other sources where they can learn more about the concepts discussed in the chapter and shows them related topics to explore.

> Please note that making chapters follow this structure may require splitting some of the existing content into new files.
> These files should be updated in the Table of Contents in the `_toc.yml` file.