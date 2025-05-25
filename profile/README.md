# UniversalCEFR: Enabling Open Multilingual Research on Language Proficiency Assessment

UniversalCEFR is a largescale, multilingual, multidimensional dataset comprising of texts annotated according to the [CEFR (Common European Framework of Reference)](https://www.coe.int/en/web/common-european-framework-reference-languages/level-descriptions). The collection comprises of a total of **505,807 CEFR-labeled texts** annotated according to the in **13 languages** in 4 script (Latin, Arabic, Devanagari, and Cyrillic).

 - English (en)
 - Spanish (es)
 - German (de)
 - Dutch (nl)
 - Czech (cs)
 - Italian (it)
 - French (fr)
 - Estonian (et)
 - Portuguese (pt)
 - Arabic (ar)
 - Hindi (hi)
 - Russian (ru)
 - Welsh (cy)

To enable open research in both automated readability and language
proficiency assessment, UniversalCEFR comprises curated from educational and learner-oriented resources, standardized into a unified data format to support consistent processing, analysis, and modeling across tasks and languages.

## UniversalCEFR Data Format / Schema
To ensure interoperability, transformation, and machine readability, adopted **standardised JSON format** for each CEFR-labeled text. These fields include the source dataset, language, granularity (document, paragraph, sentence, discourse), production category (learner or reference), and license.

| **Field**         | **Description**                                                                                                                                                                                                                                                                                       |
|-------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `title`           | The unique title of the text retrieved from its original corpus (`NA` if there are no titles such as CEFR-assessed sentences or paragraphs).                                                                                                                                                         |
| `lang`            | The source language of the text in ISO 638-1 format (e.g., `en` for English).                                                                                                                                                                                                                         |
| `source_name`     | The source dataset name where the text is collected as indicated from their source dataset, paper, and/or documentation (e.g., `cambridge-exams` from Xia et al., 2016).                                                                                                                             |
| `format`          | The format of the text in terms of level of granularity as indicated from their source dataset, paper, and/or documentation. The recognized formats are the following: [`document-level`, `paragraph-level`, `discourse-level`, `sentence-level`].                                                   |
| `category`        | The classification of the text in terms of who created the material. The recognized categories are `reference` for texts created by experts, teachers, and language learning professionals and `learner` for texts written by language learners and students.                                         |
| `cefr_level`      | The CEFR level associated with the text. The six recognized CEFR levels are the following: [`A1`, `A2`, `B1`, `B2`, `C1`, `C2`]. A small fraction (<1%) of text in UniversalCEFR contains unlabelled text, texts with plus signs (e.g., `A1+`), and texts with no level indicator (e.g., `A`, `B`). |
| `license`         | The licensing information associated with the text (e.g., `CC-BY-NC-SA` or `Unknown` if not stated).                                                                                                                                                                                                                         |
| `text`            | The actual content of the text itself.  

## Accessing UniversalCEFR 

If you're interested in a specific individual or group of datasets from UniversalCEFR, you may access their transformed, standardised version through the UniversalCEFR Huggingface Org: https://huggingface.co/UniversalCEFR

If you use any of the datasets indexed in UniversalCEFR, **please cite the original dataset papers** they are associated with. You can find them in the data directory above.

Note that there are a few datasets in UniversalCEFR---`EFCAMDAT`, `APA-LHA`, and `DEPlain`---that are not directly available from the UniversalCEFR Huggingface Org as they require users to agree with their Terms of Use before using them for non-commercial research. Once you've done this, you can use the preprocessing Python scripts in `universal-cefr-experiments` repository to transform the raw version to UniversalCEFR version.

## Join the UniversalCEFR Initiative

### Initiators and Collaborators
An initiative started as a collaboration between the researchers around the world who are interested in **1) building a more open and accessible language proficiency assessment data resources** that are also **2) standardised for maximized machine readability**.

 1. Joseph Marvin Imperial (University of Bath, UK and National University Philippines)
 2. Abdullah Barayan (Cardiff University, UK)
 3. Regina Stodden (Bielefeld University, Germany)
 4. Rodrigo Wilkens (University of Exeter, UK)
 5. Ricardo Muñoz Sánchez (University of Gothenburg, Sweden)
 6. Lingyun Gao (UCLouvain, Belgium)
 7. Melissa Torgbi (University of Bath, UK)
 8. Dawn Knight (Cardiff University, UK)
 9.  Gail Forey (University of Bath, UK)
 10. Reka R. Jablonkai (University of Bath, UK)
 11. Ekaterina Kochmar (MBZUAI, UAE)
 12. Robert Reynolds (Brigham Young University, USA)
 13. Eugénio Ribeiro (INESC-ID Lisboa and Instituto Universitário de Lisboa , Portugal)
 14. Horacio Saggion (Universitat Pompeu Fabra, Spain)
 15. Elena Volodina (University of Gothenburg, Sweden)
 16. Sowmya Vajjala (National Research Council, Canada)
 17. Thomas François (UCLouvain, Belgium)
 18. Fernando Alva-Manchego (Cardiff University, UK)
 19. Harish Tayyar Madabushi (University of Bath, UK)

### How to Join?
We want to grow this community of researchers, language experts, and educators to further advance openly accessible CEFR/language proficiency assessment datasets for all. 

If you're interested in this direction and/or have open dataset/s you want to add to UniversalCEFR for better exposure and utility to researchers, please fill up this **[form](https://forms.office.com/e/hjd7ew0M8C)**. 

When we index your dataset to UniversalCEFR, we will cite you and the paper/project from which the dataset came across the UniversalCEFR platforms. 

### Contact
For questions, concerns, clarifications, and issues, please contact [Joseph Marvin Imperial](https://www.josephimperial.com/) (jmri20@bath.ac.uk).

## Reference
Please use the following information when citing UniversalCEFR:

To be updated.




> Written with [StackEdit](https://stackedit.io/).
