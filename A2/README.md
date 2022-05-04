## HCDE410SP22 - Assignment A2

The homework assignment HCDE410: Human Data Interaction A2. Assignment cloned from [Brock Craft's](https://github.com/brockcraft/hcde410sp22) and edited by me. This repo is protected under the MIT license.


### Datasets

**Can be found in the annotationdatasets.zip**.
The datasets used in the main jupyter file can be found in annotationdatasets folder. The data files come from the [Wikipedia Talk Corpus](https://meta.wikimedia.org/wiki/Research:Detox/Data_Release) and can be found downloaded from [Figshare](https://figshare.com/projects/Wikipedia_Talk/16731) for free under the Wikimedia open access policy. There are two types of data files downloaded.

**Annotator Demographics** are demographic information about the individual crowdsourced participants who labeled the Wikipedia text files.
- aggression_worker_demographics.tsv
- attack_worker_demographics.tsv
- toxicity_worker_demographics.tsv

| **Data Variable** | **Description** |
|-----------| ------------|
| worker_id | Unique code attached to an individual annotator |
| gender | Gender of the annotator; *male, female, other* |
| english_first_language | Binary variable whether annotator is a native English speaker, *1*, or not a native English speaker, *0* |
| age_group | Nominal age bracket of the annotator; under 18, 18-30, 30-45, 45-60, over 60|
| education | Highest education achieved by the annotator; none, some highschool, highschool, professional, bachelors, masters, doctorate|

*Please note that all variables are recorded as strings data types. Professional degree is assumed to be trade school or equivalent.*

**Annotation Datasets** are the Wikipedia text files with a score provided by the annotators to measure whether toxicity, aggression, or attack language is found within the text file.
- toxicity_annotations.tsv

| **Data Variable** | **Description** |
|-----------| ------------|
| rev_id | Unique code attached to each Wikipedia text comment |
| worker_id | Unique code attached to an individual annotator |
| toxicity | Binary variable whether the text comment contains toxicity; *1* if identified as toxic, *0* if post not identified as toxic |
| toxicity_score | A 5 point Lichter scale to measure how toxic the comment is. Scale is: -2 Very Toxic, -1 Toxic, 0 Neither, 1 Healthy Contribution, 2 Very Health contribution|

*Please note that all variables are recorded as strings data types.*

### hcde410-a2.ipynb

The file that conducts an analysis to identify:
- Demographics of the annotators.
- Missing or incomplete annotator data.
- Relationship of annotators and the toxicity dataset.

The file outputs the dataset a2_all_annotator_demographics.csv and images contained within the a2graphics file.

### a2_all_annotator_demographics.csv

The file is a combination of all 3 annotator demographic datasets cleaned to remove  duplicates. The file columns are the exact same as the annotation dataset above.

### a2graphics

The data viusalizations to show relationships of demographics represented by the annotators in the annotator demographic datasets. Graphis are created for the following topics:
- Gender
- Native English Speaker
- Age Group
- Education
