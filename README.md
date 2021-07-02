# PapyGreek Treebanks 1.0

These XML files contain documentary papyrus texts written in Postclassical Greek (ca. 300 BCE–700 CE), morphosyntactically annotated according to Dependency Grammar. The source of the digital editions of the papyri is [Papyri.info IDP (Integrating Digital Papyrology) Data](https://github.com/papyri/idp.data) in TEI EpiDoc XML, and the texts have been preprocessed into annotatable form (omitting TEI tags) to include both editorial regularisations (`reg`) and the original (`orig`) forms of the words (cf. [Vierros and Henriksson 2017](https://hal.archives-ouvertes.fr/hal-01279493v2), [Vierros 2018)](https://www.degruyter.com/document/doi/10.1515/9783110547450-006/html); the linguistic annotation of the `reg` and `orig` tokens may differ from one another, revealing linguistic variation. The platform for handling the papyri (preprocessing, annotation, adding metadata, etc.) is the [PapyGreek portal](https://papygreek.hum.helsinki.fi/), developed by Henriksson for the project [Digital Grammar of Greek Documentary Papyri (PapyGreek)](https://www2.helsinki.fi/en/researchgroups/digital-grammar-of-greek-documentary-papyri). PapyGreek portal has replaced the older platform _Sematia_ (no longer used) and some of the annotations included in _Sematia_ have been imported to PapyGreek.

- Text count 395
- Sentence count 3102
- Token count 44036

The syntactic trees have been semi-manually annotated using the [Arethusa](https://www.perseids.org/tools/arethusa/app/#/) editor, by different people (indicated in the metadata tag `<annotator>`) and each text has gone through a review process (review board: Marja Vierros and Polina Yordanova). We have followed the Ancient Greek Dependency Treebank Guidelines 2.0 ([Celano 2014](https://github.com/PerseusDL/treebank_data/blob/master/AGDT2/guidelines/Greek_guidelines.md)) for the morphological and syntactic layer (the advanced syntactic/semantic layer is not included). Additional PapyGreek Guidelines are [here](https://docs.google.com/document/d/1bqZaRU2E_Ixg6Z3s9qcY4EWN6DB1k5C3I4Vgs7vSsh4/edit#heading=h.yi9iujik2bb2). All morphological information is in the nine-place string of the `<postag>` ([key](https://docs.google.com/document/d/1hzrAkSwhTcHVBnJSOJ28j6PP1vPP9MiQo5Zj989dttc/edit?usp=sharing)).

**The texts have different types of contextualizing metadata:**

`<document_meta>`: Place of Origin and Date of the document are retrieved from the IDP data, as are the [Trismegistos](https://www.trismegistos.org/index.php) and papyri.info identifiers.

`<hand_meta>`: Papyrus texts may have several parts written by different hands. We have added metadata in these text parts for the following information (filled in when applicable, otherwise left blank):

`<text_type>`: three levels of categories: hypercategory, category, subcategory (all three are not necessarily always given). For smaller subscript texts or marginal notes the text type may be completely missing. The text type list is applied from a similar list shared by the project [Everyday Writing in Graeco-Roman and Late Antique Egypt EVWRIT](https://www.evwrit.ugent.be/) (Ghent).

`<person>`: four different functions for people concerning each handwriting part can be present: Author, Writer, Addressee and External Scribal Official. These people have been assigned their own PapyGreek ID number `<pg_id>`, so that a person appearing in multiple documents can be identified (especially important when the handwriting is the same in several documents, but no name for that person is mentioned in the text, i.e. the Writer). The PG-ID has some stable information (if these are known): the name, gender, and TM Person ID. The people are provided with optional additional information that pertain to one document only, such as description of the handwriting, the honorific epithet, ethnic label, occupation/role, domicile, age, and education of the person (if these are known and applicable). On some documents, where no knowledge of the hand is available in printed editions, the PG-ID for the Writer may not be present at the moment.

The treebanks are licensed under a CC BY-SA 4.0 License (see LICENSE file).

