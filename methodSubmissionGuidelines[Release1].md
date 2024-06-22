# Method Submission Guide
:- *Version 0.1*

Taimoor Khan, Hajira Jabeen

_This document serves as a guide for adding methods to the Methods Hub. It assists in preparing methods for the Methods Hub through workflows, checklists, and guidelines to ensure conformance to the defined standards._

**Abstract:**

The Methods Hub is an infrastructure project whose goal is to provide open and accessible computational methods to collect, access, and work with Digital Behavioral Data (DBD). The bulk of our methods will stem from computer science, notably showcasing cutting-edge AI/ML techniques, alongside those originating from social science. It aims to serve as a pioneering platform designed to facilitate the propagation of computer science methodologies into social science research.

_Note: This is a living document for content submission guidelines and therefore, the method submission scenarios, their definition and the checklist to adhere to are frozen for release 1 (June 2024). Additional changes in this regard will be considered for the next release._

Methods Hub Content Goal

The Methods Hub content goal is to provide well-documented, high-quality, relevant content to social scientists that is appliable to Digital Behavioral Data.

Methods Hub Content Objectives

Methods Hub content has the following objectives.

1. Enabling reuse of recent AI/ML models on Digital Behavioral Data in social science.
2. Empower social scientists in using AI methods.
3. Allows AI/ML method developers to reach a wider audience and contribute cross domain research challenges.

Glossary

|     |     |
| --- | --- |
| Method | Code snippets, one or more programming function<sup>[\[1\]](#footnote-2)</sup>, one or more programming classes or modularized software source code and its documentation. |
| Tutorial | A stepwise guide with or without code that explains working with an important tool, technology, or the available method(s). Tutorials facilitate and enable researchers to work with SOTA methods |
|     |     |

List of Abbreviations

|     |     |
| --- | --- |
| DBD | Digital behavioral data |
| MH  | Methods Hub |
| CFF | Citation File Format |
| AI/ML | Artificial Intelligence/Machine Learning |
| CS  | Computer Science |
| SocSci | Social Science |

**Table of contents**

[1\. Method Submission Workflow 8](#_Toc163597893)

[1.1. Method Submission Scenarios 9](#_Toc163597894)

[1.1.1. Scenario CS1: CS reputed publication with quality-controlled code 10](#_Toc163597895)

[1.1.2. Scenario CS2: CS reputed publication without quality-controlled code 10](#_Toc163597896)

[1.1.3. Scenario CS3: CS new/unpublished method 10](#_Toc163597897)

[1.1.4. Scenario CS4: CS reputed publications with established community 11](#_Toc163597898)

[1.1.5. Scenario SocSci1: Social science software publication 11](#_Toc163597899)

[1.1.6. Scenario SocSci2: Social science publication without quality-controlled code 12](#_Toc163597900)

[1.1.7. Scenario SocSci3: 12](#_Toc163597901)

[2\. Methods Submission Checklist 14](#_Toc163597902)

[2.1. Checklist CS1: CS Publication with Quality-Controlled Code 14](#_Toc163597903)

[2.2. Checklist CS2/CS3: CS Publication without Quality-Controlled Code or Unpublished Methods 15](#_Toc163597904)

[2.3. Checklist CS4: CS Publication with Established Community 15](#_Toc163597905)

[2.4. Checklist SS1: Social Science Quality-Controlled Software Publication 16](#_Toc163597906)

[2.5. Checklist SS2/SS3: Social Science Publication Without Quality-controlled Software or Unpublished Method 16](#_Toc163597907)

[3\. Method Preconditions 18](#_Toc163597908)

[4\. Method Scope 19](#_Toc163597909)

[4.1. Method/Task Categories 19](#_Toc163597910)

[5\. Method Quality Guidelines 21](#_Toc163597911)

[5.1. Method Documentation Quality 21](#_Toc163597912)

[5.1.1. Documents List 21](#_Toc163597913)

[5.1.2. README Guidelines 22](#_Toc163597914)

[5.2. Method Code Quality 23](#_Toc163597915)

[5.2.1. Code Quality Guidelines 23](#_Toc163597916)

[7\. Resources and Supporting Material 26](#_Toc163597917)

[9\. References 27](#_Toc163597918)

**List of Figures**

[Figure 1: The general method submission workflow 7](#_Toc163605929)

[Figure 2: Dimensions of methods submitted into the Methods Hub 8](#_Toc163605930)

[Figure 3: Method development preconditions 16](#_Toc163605931)

**List of Tables**

[Table 1: Method submission scenarios 9](#_Toc163461848)

[Table 2: checklist CS1: CS publication (methodology) with quality-controlled code 13](#_Toc163461849)

[Table 3: checklist CS2/CS3: CS publication (methodology) without quality-controlled code or unpublished methods 14](#_Toc163461850)

[Table 4: Checklist CS4: CS publication (methodology) with established community 14](#_Toc163461851)

[Table 5: Checklist SS1: Social science quality-controlled software publication 15](#_Toc163461852)

[Table 6: Checklist SS2/SS3: social science method publication without quality-controlled software or unpublished method 15](#_Toc163461853)

1\. Method Submission Workflow

This document serves as a roadmap for navigating the method submission process by offering different scenarios, and steps under each scenario to submit a method. The method submission workflow is aimed to empower developers/researchers to identify recent and interesting methods, resolve submission constraints if any, and make methods and tutorials Methods Hub-ready i.e., developers and researchers can shape their methods following these guidelines. _Figure 1_ provides the method submission workflow where the methods prepared are self-reported into the _content catalog_<sup>[\[2\]](#footnote-3)</sup>. The method submission workflow is followed by the method review workflow that ensures adherence to the provided standards; however, the review workflow is out of this document's scope.

Figure 1: The general method submission workflow

The Methods Hub contains stateoftheart AI/ML methods that can be applied to social science use cases and research questions. Only a fraction of methods is being used in the social science domain, however, there exists a vast array of untapped potential methods that could significantly provide benefits to the field.

It brings us into the three overlapping dimensions to decide whether a method can be submitted into the Methods Hub, given in _Figure 2_. They are:

1. Relevance to social science
2. Recent AI/ML methods
3. If reviewed and published (quality control)

Figure 2: Dimensions of methods submitted into the Methods Hub

The overlapping of these dimensions leads to different possible cases. For example, a method that is stateo –f-the-art and published at a prominent venue but its relevance to social science is not established. Or a method published at a prominent social science venue, but the recency of the method used is not verified. Similarly, the software or code accompanying the method may not be reviewed for its quality and reusability. It is therefore important to treat these methods differently. We have defined scenarios for these methods with different flow of steps leading to method submission into the MH.

_Note: Chapter 6 provides details of what to consider a method and how to identify methods from research pipelines._

## 1.1. Method Submission Scenarios

From the three dimensions in _Figure 2_, the possible scenarios for submitting methods into the Methods Hub are given in _Table 1_. **Scenario CS1** represents AI/ML methods from the computer science domain that are state-of-the-art, have quality-controlled code and are published at reputed computer science venues. **Scenario SocSci1** represents social science methods with quality-controlled code published at a prominent social science venue. Similarly, the other scenarios have different levels of recency, relevance to social science and quality review in the publication process.

Table 1: Method submission scenarios

|     | Computer Science | Social Science |     |
| --- | --- | --- | --- |
| Evidence for Relevance | **Scenario CS1:** CS reputed Publication with quality-controlled code | **Scenario SocSci1:** Social Science reputed publication with quality-controlled code | State of the art in CS, AI |
| **Scenario CS2:** CS reputed publication without quality-controlled code | **Scenario SocSci2:** Social Science reputed publication without quality-controlled code |
| **Scenario CS-SocSci3:** Unpublished methods from computer and social science domain |     |     |
| **Scenario CS4:** CS reputed publication (methodology) with established communities |     |     |

Next, we define method submission workflows for methods falling into the scenarios in _Table 1_, along with the associated constraints and checklists to comply with.

- - 1. Scenario CS1: CS reputed publication with quality-controlled code

The methods in this scenario are recent computer science publications with peer reviewed methodology along with the quality-controlled code. The methodology itself is novel and transparent that instills confidence in its findings. The code for these methods also underwent _review process_ establishing acceptable quality in the computer science domain. Therefore, the code is known to be quality-controlled i.e., _well documented and reusable_.

For submission in the MH, these methods need to resolve the following constraints:

1. Resolve preconditions. ([Chapter 3: Preconditions](#_3._Method_Preconditions), provide details on what preconditions are and how to address them)
2. Resolve scope ([Chapter 4: Scope criteria](#_4._Scope_Criteria), provide details on how to meet the scoping criteria)

The checklist associated with this scenario ([2.1. Checklist CS1](#_2.1._Checklist_CS1:)) assists in ticking the conditions for resolving preconditions and scope criteria.

- - 1. Scenario CS2: CS reputed publication without quality-controlled code

1.1.3. Scenario CS-SocSci3: New unpublished method

The methods in scenario _CS2_ are recent computer science methods that are peer reviewed and published; however, the code is not quality controlled as part of the review process. Note that only providing code along with the publication does not guarantee the quality of code. For example, [propensity method](https://www.sciencedirect.com/science/article/pii/S1751157722000323?via%3Dihub) is published at a computer science method publishing venue i.e., journal of informatics without quality-controlled code.

In the case of scenario _CS3_ the methods represent recent AI/ML research but are not yet published and therefore, has not undergone any review process.

The method that falls into scenarios CS2 or CS3 need to resolve the following constraints:

1. Resolve preconditions ([Chapter 3: Preconditions](#_3._Method_Preconditions), provide details on what preconditions are and how to address them)
2. Resolve scope ([Chapter 4: Scope criteria](#_4._Scope_Criteria), provide details on how to meet the scoping criteria)
3. Ensure following the method submission documentation guidelines ([Section 5.1: Documentation quality](#_5.1._Method_Documentation), presents the required documents for submitting a method and specific structures of those documents)
4. Ensure code reusability ([Section 5.2: Code quality](#_5.2._Method_Code), provides support and resources on making code readable, understandable, and reusable)

The checklist associated with these scenarios ([2.2. Checklist CS2/CS3](#_2.2._Checklist_CS2/CS3:)) assists in ticking the conditions required for these methods.

1.1.4. Scenario CS4: CS reputed publications with established community

The scenario _CS4_ includes prominent contributions published in the computer science domain that are applicable and of interest in the social science domain. However, they are also well established on GitHub and have active communities around them. For example, [SANSA](https://sda.tech/author/hajirajabeen/) and [BERD-NFDI](https://github.com/BERD-NFDI/bear-ml/tree/main/bearml) are well established methods that may be of value in the social science domain as well.

In general, this scenario represents methods where it may not be fruitful to suggest modification to the method code and documentation as they have established community and are being well received in the community. We are interested in bringing these methods to the MH for social scientists too.

The methods falling in this scenario need to resolve the following constraints:

1. Writing tutorial(s) that establish relevance to social science. And demonstrate use of their methods targeted towards Social Science.

The checklist associated with these scenarios ([2.3. Checklist CS4](#_2.3._Checklist_CS4:)) assists in ticking the conditions required for these methods. The [tutorial template](https://gesisev.sharepoint.com/:t:/s/O365_Team_KTS-BDA/ERKFBhSnpfdBtH31lgVNoYMBw6AbdwO-x7mRp3gMx0NQPg?e=7ZVCDG) provides a structure for writing tutorials having mandatory and optional sections.

Writing a tutorial provides an alternative from updating the actual repo documentation of a well-established method, while serving as the linkage to establish relevance for the MH.

1.1.5. Scenario SocSci1: Social science software publication

This scenario represents the social science venues that publish software in the social science domain. Some of the [prominent social science software publishing venues](https://gesisev.sharepoint.com/:w:/s/O365_Team_KTS-BDA/Eb0_H8VsXRJMlH38ykigwR4BzChexXqfWIhEZsWWUuVcxg?e=Tlwp4N) are listed. The list is expected to grow with newer venues identified and reported.

These venues have well defined documentation requirements to make the code readable, understandable, and reusable. For example, [sweater: Speedy Word Embedding Association Test and Extras Using R](https://joss.theoj.org/papers/10.21105/joss.04036). The code is reviewed for its quality too; therefore, these methods already comply with the MH method submission requirements and can be submitted directly.

These methods need to resolve the following constraints:

1. Assign the method to an appropriate task category(ies) ([Section 4.1 method/task categories](#_4.1._Method/Task_Categories), provide method/task categories that may be assigned to methods. These categories are not mutually exclusive and are frozen for release 1 i.e., in June2024.)

The checklist associated with these scenarios ([2.4. Checklist SS1](#_2.4._Checklist_SS1:)) assists in ticking the conditions required for these methods.

_Note: In case your method is published as software at a social science venue, but its name is not on the list of prominent social science venues, consult the Methods Hub Team._

1.1.6. Scenario SocSci2: Social science publication without quality-controlled code

In scenario SocSci2, the research paper offers a methodology published at a social science venue; however, software is not part of a publication. Therefore, the method has undergone the review process and is applicable to social science research questions, but the code quality has not yet been established. For example, [Misclassification in Automated Content Analysis Causes Bias in Regression. Can We Fix It? Yes We Can!](https://www.tandfonline.com/doi/full/10.1080/19312458.2023.2293713)

These methods need to resolve the following constraints:

1. Resolve preconditions ([Chapter 3: Preconditions](#_3._Method_Preconditions), provide details on what preconditions are and how to address them)
2. Assign the method to an appropriate task category(ies) ([Section 4.1 method/task categories](#_4.1._Method/Task_Categories), provide method/task categories that may be assigned to methods. These categories are not mutually exclusive and are frozen for release 1 i.e., in June2024.)
3. Ensure following the method submission documentation guidelines ([Section 5.1: Documentation quality](#_5.1._Method_Documentation), presents the required documents for submitting a method and specific structures of those documents)
4. Ensure code reusability ([Section 5.2: Code quality](#_5.2._Method_Code), provides support and resources on making code readable, understandable, and reusable)

The checklist associated with these scenarios ([2.5. Checklist SS2/SS3](#_2.5._Checklist_SS2/SS3:)) assists in ticking the conditions required for these methods.

The remaining document is structured as follows. Chapter 2 provides the checklists for each of the scenarios discussed in chapter 1. Chapters 3 and 4 provide guidelines on how to make the method open access and relevant to social scientists. Chapter 5 discusses the documentation and code quality guidelines for the methods. Chapter 6 assists to determine identifying methods from previous, current, or future research work and how to modularize it for the Methods Hub. Chapter 7 lists additional resources in following the guidelines and preparing the methods for submission.

# 2\. Methods Submission Checklist

The Methods checklist provides the minimum criteria that need to be met for the methods to be submitted to the Methods Hub.

Method Name: \_**\_**\_**\_**\_**\_**\_**\_**\_**\_**\_**\_**

Method Developer & Email: \_**\_**\_**\_**\_**\_**\_**\_**\_**\_**\___\__

Method repo URL: \_**\_**\_**\_**\_**\_**\_**\_**\_**\_**\_**\_**\__

## 2.1. Checklist CS1: CS Publication with Quality-Controlled Code

Table 2: checklist CS1: CS publication (methodology) with quality-controlled code

| [Preconditions (Chapter3)](#_3._Method_Preconditions) |     |
| --- |     | --- |
| ☐<br><br>☐<br><br>☐ | Open-sourced language<br><br>Open script<br><br>Open license |
| [Scope criteria (Chapter 4)](#_4._Scope_Criteria) |     |
| ☐<br><br>☐<br><br>☐ | Social science use case(s)<br><br>DBD applicability<br><br>Assign the method to an appropriate method/task category(ies) |

## 2.2. Checklist CS2/CS3: CS Publication without Quality-Controlled Code or Unpublished Methods

Table 3: checklist CS2/CS3: CS publication (methodology) without quality-controlled code or unpublished methods

| [Preconditions (Chapter 3)](#_3._Method_Preconditions) |     |     |
| --- |     |     | --- | --- |
| ☐<br><br>☐<br><br>☐ | Open-sourced language<br><br>Open script<br><br>Open license |     |
| [Scope criteria (Chapter 4)](#_4._Scope_Criteria) |     |     |
| ☐<br><br>☐<br><br>☐ | Social science use case(s)<br><br>DBD applicability<br><br>Assign the method to an appropriate method/task category(ies) |     |
| [Documentation and code quality (Chapter 5)](#_5._Method_Quality) |     |     |
| ☐<br><br>☐<br><br>☐<br><br>☐<br><br>☐<br><br>☐<br><br>☐ | [Documentations Required](#_5.1.1._Documents_List)<br><br>Citation file format as a .cff or plain file<br><br>Requirements.txt or yaml file<br><br>License file<br><br>README<br><br>Code file(s)<br><br>[Documentations Quality (Section 5.1.2)](#_5.1.2._Documentation_%28README%29)<br><br>README is complete and user friendly, using the MethodReadMeTemplate and guidelines in section 5.1.<br><br>[Code Quality (Section 5.2)](#_5.2._Method_Code)<br><br>The code is reusable | [citation(template).cff](https://gesisev.sharepoint.com/:u:/s/O365_Team_KTS-BDA/EaNptjMTYLxJjGJirpC35uoBV0YhngXvU9TsHjhguuJxJw?e=R2gZkB)<br><br>[README (template).md](https://gesisev.sharepoint.com/:t:/s/O365_Team_KTS-BDA/EYr_RPTy8QRMpNli_OqKcHEBvqbnKXqVCioRCEcNKRX-sA?e=XJ6PtI) |

## 2.3. Checklist CS4: CS Publication with Established Community

Table 4: Checklist CS4: CS publication (methodology) with established community

| Tutorial writing |     |     |
| --- |     |     | --- | --- |
| ☐   | Write a tutorial to establish relevance | [Tutorial(template)](https://gesisev.sharepoint.com/sites/O365_Team_KTS-BDA/Freigegebene%20Dokumente/Forms/AllItems.aspx?id=%2Fsites%2FO365%5FTeam%5FKTS%2DBDA%2FFreigegebene%20Dokumente%2FGeneral%2FSTB%2FMethodsHub%2FContentCollectionGuidelines%2FMethodSubmissionGuidelines%2Ftutorial%2Dtemplate%2Ftutorial%2Dtemplate%2Dv0%2E2%2Emd&parent=%2Fsites%2FO365%5FTeam%5FKTS%2DBDA%2FFreigegebene%20Dokumente%2FGeneral%2FSTB%2FMethodsHub%2FContentCollectionGuidelines%2FMethodSubmissionGuidelines%2Ftutorial%2Dtemplate&p=true&ga=1) |

## 2.4. Checklist SocSci1: Social Science Quality-Controlled Software Publication

Table 5: Checklist SS1: Social science quality-controlled software publication

| [Method categorization (Section 4.1)](#_4.1._Method/Task_Categories) |     |
| --- |     | --- |
| ☐   | Assign the method to an appropriate method/task category(ies) |

## 2.5. Checklist SocSci2/SS3: Social Science Publication Without Quality-controlled Software or Unpublished Method

Table 6: Checklist SS2/SS3: social science method publication without quality-controlled software or unpublished method

| [Preconditions (Chapter 3)](#_3._Method_Preconditions) |     |     |
| --- |     |     | --- | --- |
| ☐<br><br>☐<br><br>☐ | Open-sourced language<br><br>Open script<br><br>Open license |     |
| [Scope criteria (Chapter 4)](#_4._Scope_Criteria) |     |     |
| ☐<br><br>☐<br><br>☐ | Social science use case(s)<br><br>DBD applicability<br><br>Assign the method to an appropriate method/task category(ies) |     |
| [Documentation and code quality (Chapter 5)](#_5._Method_Quality) |     |     |
| ☐<br><br>☐<br><br>☐<br><br>☐<br><br>☐<br><br>☐<br><br>☐ | [Documentations Required (Section 5.1)](#_5.1.1._Documents_List)<br><br>Citation file format as a .cff or plain file<br><br>Requirements.txt or yaml file<br><br>License file<br><br>README<br><br>Code file(s)<br><br>[Documentations Quality (Section 5.1.2)](#_5.1.2._Documentation_%28README%29)<br><br>The README is complete and user friendly, using the MethodReadMeTemplate and guidelines in section 5.1.<br><br>[Code Quality (Section 5.2)](#_5.2._Method_Code)<br><br>The code is reusable | [citation(template).cff](https://gesisev.sharepoint.com/:u:/s/O365_Team_KTS-BDA/EaNptjMTYLxJjGJirpC35uoBV0YhngXvU9TsHjhguuJxJw?e=R2gZkB)<br><br>[README](https://gesisev.sharepoint.com/:t:/s/O365_Team_KTS-BDA/EYr_RPTy8QRMpNli_OqKcHEBvqbnKXqVCioRCEcNKRX-sA?e=XJ6PtI)(template).md |

# 3\. Method Preconditions

&nbsp;

There are three preconditions following open access protocols. To fulfill preconditions, the methods should be scripted in open language, are publicly accessible and have an open license. The platform supports scripts in open languages e.g., Python, R and does not cover commercial tools e.g., MATLAB, SPSS etc. The code must be publicly accessible to all from popular code sharing platforms like GitHub or GitLab, _Figure 3_.

![](data:image/png;base64,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)

Figure 3: Method development preconditions

**Licenses** like [MIT open license](https://github.com/git/git-scm.com/blob/main/MIT-LICENSE.txt), [Apache 2.0 open license](https://github.com/apache/.github/blob/main/LICENSE) and CC-BY 4.0 are popular open-source licenses widely used in the GitHub community. The MIT license is known for its simplicity and permissiveness, allowing developers to freely use, modify, and distribute the software while requiring them to include the original license and disclaimer in any substantial portions of the code. The Apache License 2.0 is a more comprehensive license that provides clear guidelines on contributions, patents, and liability. Although these three are suggested as the frequently used open-source licenses, it doesn’t limit the use of any other open-source license.

# 4\. Scope Criteria  

Methods Hub is a method market for social science methods and, therefore, the content submitted in the Methods Hub portal must be relevant to social science. Therefore, the scope criteria are defined around relevance of the method to the social science domain. We are using the following three criteria to determine the scope of the method.

&nbsp;  

The scope or relevance to social science is resolved through method documentation as:

1. Write use case(s) in the README or research questions of a method that are directly related to social science. Providing multiple use cases offers the opportunity to perceive methods differently in diverse scenarios, therefore establishing a strong relevance with the social science audience. ([for help on writing social science use cases](https://gesisev.sharepoint.com/:w:/s/O365_Team_KTS-BDA/EUtz1wwvnIlIiu12tJkINZcBNLqQiCE_ToJBGOMnoMyufg?e=9LtaNK))
2. Provide public DBD dataset (ideally providing link to the [GESIS DBD dataset](https://www.gesis.org/en/institute/digital-behavioral-data)) that can be used with the method. It also assists in demonstrating relevance to social science.  
3. The method must fall into the method/task category(ies) defined for Methods Hub.

_Note: In case of any difficulty in assigning a method to method/task category(ies), please report to Methods Hub Team_

&nbsp;

&nbsp;

## 4.1. Method/Task Categories

**Data Collection and Retrieval:** This category encompasses methods for obtaining and gathering data from various sources. These methods serve as the foundation for acquiring diverse datasets for subsequent analysis.

**Data Preprocessing:** Data preprocessing involves preparing raw data for analysis. This category includes methods to clean, structure, and enhance the quality of data. Tasks such as data cleaning, text preprocessing, data encryption, data anonymization, feature engineering, normalization, and data transformation fall under this category.

**Data Mining:** Data mining involves uncovering patterns, trends, and valuable insights from large datasets. This category includes various techniques such as text mining, sentiment analysis, topic modeling, named entity recognition, text classification, text clustering, graph mining, data classification, data clustering, data enrichment, and the utilization of large language models. These methods help in extracting meaningful information from structured and unstructured data.

**Analysis:** The analysis category focuses on examining and interpreting data to derive meaningful conclusions. It includes methods such as social network analysis, spatial analysis, temporal analysis, time-series analysis, pattern recognition, community detection, outlier detection, anomaly detection, and the use of advanced language models. These methods provide insights into relationships, trends, and anomalies within the data.

**Data Visualization:** Data visualization involves presenting data in a visual format to aid understanding. This category includes network visualization for representing relationships and tabular data visualization for structured numerical information. Effective visualization enhances the communication of findings and patterns derived from the data.

_To explore the taxonomy categories and their_ **_sub-categories_** _in detail, please visit_ [_methods categorization description document_](https://gesisev.sharepoint.com/:w:/s/O365_Team_STB_WP_Methods_Hub/EQ5KNJ95AodNq7weScTp6jsBx8E3CkUA-Aq90xWc_QPMbg?e=Su9MaL)_._

# 5\. Method Quality Guidelines

Computational methods are the most common type of content on the Methods Hub. It aims to lower the technical barriers for using recent AI/ML models in social science, while encouraging to develop reusable workflows.

This chapter provides guidelines for preparing method quality that is acceptable for Methods Hub. Section 5.1 deals with the quality of the _method documentation_ while section 5.2 presents quality criteria for the _method code._

&nbsp;

## 5.1. Method Documentation Quality

### 5.1.1. Documents List

The method documentation must contain at least the following four types of documents.  

1. README file
2. Requirements
3. Citation File Format (.CFF) or CITATION file
4. License file (e.g. [MIT](https://github.com/git/git-scm.com/blob/main/MIT-LICENSE.txt), [Apache 2.0](https://github.com/apache/.github/blob/main/LICENSE), CC-BY 4.0)
5. Configuration yaml file (optional)

_There must be only one of these files in the repo to avoid confusion. All the other files should be organized in subdirectories._

The **README file** facilitates determining the readability, understandability, and reusability of the method. It may also contain optional subsections of disclaimer, acknowledgements, or publication, if applies. However, it is very important to mention the developer contact details to help reach back to the developer if need be.

The next subsection provides details on the internal structure of the README document.

The **requirements.txt** file contributes to reusability by recreating the environment needed to execute the method.  [Chapter 6](#_7._Resources_and) provides relevant resources on how to freeze the environment by preserving the libraries and packages along with their versions, so that they can be easily deployed again for reusability.

**Citation file formats (CFF)** are standardized structures designed to capture and represent bibliographic information about scholarly references. These files typically contain metadata such as author names, publication titles, journal information, publication dates, and other relevant details. These formats enable researchers, academics, and writers to manage and exchange citation data seamlessly across various reference management tools and platforms. Additionally, citation file formats play a crucial role in ensuring accurate and consistent citation styles in academic writing, facilitating proper attribution of sources, and enhancing the reproducibility of scholarly work. Plain text citation files are also used in some cases having similar structure for citation information. The [citation(template).cff](https://gesisev.sharepoint.com/sites/O365_Team_KTS-BDA/Freigegebene%20Dokumente/General/STB/MethodsHub/Content%20Submission%20Guidelines/20240411%20M.%20S.%20Guidelines%20v0.0.3%20%5bFor%20Release%201%5d/citation%28template%29.cff) can be used to update relevant parts for the method submitted.

**Licenses** like [MIT open license](https://github.com/git/git-scm.com/blob/main/MIT-LICENSE.txt), [Apache 2.0 open license](https://github.com/apache/.github/blob/main/LICENSE) and CC-BY 4.0 are popular open-source licenses widely used in the GitHub community. Although these three are suggested as the frequently used open-source licenses, it doesn’t limit the use of any other open-source license.

Providing these documents helps in boosting citations for the method and associated publication and may lead to new collaborations. Moreover, the open methods promote a culture of using and developing open methods.

&nbsp;

### 5.1.2. README guidelines

The README document of the method needs to follow the documentation quality guidelines provided here. The methods submitted will undergo a review process to ensure compliance with the guidelines. It is also aligned with the objectives of the Methods Hub to keep high quality content only.

The most important aspect to consider in writing the README of a method is its user friendliness. It emphasizes the need for having easy to understand and easy to follow documentation. The README file should speak to social scientists in their language, using terminologies from their domain that they can relate to. In general, social scientists from different backgrounds should be able to follow the guidelines and reuse the method, aligned with the objective of Methods Hub, lowering technical barriers. The main README guidelines are:

- Avoid jargon in the method name, description, and use cases to ensure that social science researchers can generally understand the purpose of a method.
- README should link to different code files where necessary.
  - Any external information e.g., on the terms of API used in the method should link to the original instead of copying those points to the README as they may change over time.
- The description should link to relevant social science publication using similar method.
  - The programming language of the repo should be mentioned earlier in the title or description.
- The technical terms needed to help understand the method's purpose are to be explained separately as a list of definitions.
- Use appealing subsection headings to attract the audience.  
  - Do not remove/change the existing subsections in the README template
  - For each subsection to rename, use separator (-) after the name in the template and then provide your subsection name.
- Show sample input and output of the method to help users understand the purpose of the method.
  - The sample input and output should represent one of the use cases.
  - There should be some explanation of what the output means in layman terms.
  - The use cases may also be documented as research questions or research questions that the method addresses may be given separately.
- The “How to use” section should have more details to elaborate on the use of the method
  - Providing a step-by-step guide to call the method and what to expect after each step.
  - It should provide how to apply different filters or parameter settings for the method. For example, calling claims generator with different input data or specifying which input fields are mandatory. Or specifying filters on 4chan data collection.
- In the “Repo Structure” subsection, provide structure of your repo in the form of a tree, to help navigate the repo directories easily.
- Images used in the README e.g., data models, pipeline, schema structure etc. should be properly explained.
- In the “Contact” subsection, mention your contact details that users can use to follow up in case of queries.
- Provide a limitation subsection mentioning the limitations of the method, if any.
- Optional subsections
  - Provide a disclaimer if it applies to the method.
  - Provide acknowledgements if needed.  
  - Provide relevant publication if applies.

The [README(template).md](https://gesisev.sharepoint.com/sites/O365_Team_KTS-BDA/Freigegebene%20Dokumente/General/STB/MethodsHub/Content%20Submission%20Guidelines/20240411%20M.%20S.%20Guidelines%20v0.0.3%20%5bFor%20Release%201%5d/README%28template%29.md) has more on the structure of the document and how to write relevant information in each of these sections.

## 5.2. Method Code Quality

### 5.2.1. Code Quality Guidelines

Writing code that is easy to (re)use, easy to maintain and easy to adapt is crucial for having methods that remain reusable over a longer period. Maintaining coding standards is highly desired and the following guidelines will assist in achieving it:

- The method should follow basic coding standards provided in the document ([basic coding conventions](https://gesisev.sharepoint.com/:w:/r/sites/O365_Team_KTS-BDA/_layouts/15/Doc.aspx?sourcedoc=%7BC14DBA5D-412F-43A6-8206-494DA574CE22%7D&file=naming-conventions-code.docx&action=default&mobileredirect=true)). It refreshes the concepts of using consistent naming conventions and readable coding structures. However, its purpose is not to restrict developers to a single coding style.
- The code must be well structured and sufficiently commented.
- Similarly, pushing important decisions from the body of the method to the parameters to empower users alter the behavior of the method. The code should be flexible to follow different workflows within the body of the method based on the parameter settings of the users.  
- Unit tests should be provided to ensure the code is free from errors and all/most of the boundary conditions are checked.  
- The method code, in case taken from a bigger pipeline, should be modularized with minimum/no coupling or external dependencies.
- Technical documentation for the code (generated through a tool e.g., sphinx)

_Standardizing the method input and output interfacing is also desired to facilitate users transfer their learning experience from one method to another. It also minimizes the effort required to switch methods for the same task. Sci-kit-learn is a very good example of it. However, it doesn’t mean we are standardizing the methods interfaces across the Methods Hub, which is out of our scope. However, the given coding guidelines by no means attempt to limit the coding styles and their freedom as far as the code is clearly readable, understandable, and reusable._

5.2.2. Code Reusability  

The method code should be reusable so that social scientists can apply it to their research questions.

- The “Setup” or “How to Use” subsection should provide the environment with the required packages, libraries in versions needed to run the method.
- The method should produce output when given the sample input to execute in the given environment.

**Reusability Supporting material:** The [supporting material document](https://gesisev.sharepoint.com/:w:/r/sites/O365_Team_KTS-BDA/_layouts/15/Doc.aspx?sourcedoc=%7B5706327B-AFD1-471E-833E-742252D9B0A7%7D&file=supplementary-for-methods.docx&action=default&mobileredirect=true) is an early-stage effort in assisting developers to know about the tools and techniques to develop reusable methods. At present it helps on:

1. Creating and using virtual environments
2. Generating random seeds
3. Suggesting useful reproducibility tools

This document is expected to grow with time through contributions from the method developers and reviewers towards building a resource for facilitating efficient method development.

**_Note:_** _For methods in release 1 (scheduled in June 2024), ensuring that the method reusability and code quality is the responsibility of the method developer._ The method repo usage statistics (if available) are also considered e.g., watchers, downloads, forks, commits etc. In evaluating the code quality.

6\. Method Identification Guidelines

The method identification process focuses on defining what qualifies to be a computational method for Methods Hub. There can be four possible forms of a method’s code:

1. A method can be a few snippets of code that does something meaningful on the input data to give consistent and reliable output that is useful in the bigger picture. For example, POS tags or synonyms to words using built-in library.
2. It may also be acquired through code modularization where each module can be seen as a specific method e.g., the data collection module will be a data collection method from a given source, the preprocessing module can be the preprocessing method offering certain preprocessing options on the input data. This is the most prevalent form of method that gives the developers freedom to pick different methods according to their requirements and structure them into the pipeline that suits their needs.
3. A method can also be a longer pipeline that has multiple code modules performing multiple steps in a sequence. For example, collecting data from an online source, preprocessing it and vectorizing it to be used by an AI/ML model. It may also be complete end-to-end pipeline from data collection to analysis and visualizations. These methods are more helpful for getting quick results and proof of concept on a task. Both (2) and (3) have their own value and audience groups.  
4. Software application type of method, although not a common form of method represents software applications that can be downloaded and used directly, e.g., installing [ScienceLinker](https://git.gesis.org/sciencelinker/sciencelinker-development) through pip.

Generally, a method coded for a research model would have very specific settings according to the nature of the data and the research questions. However, generalizing the method to deal with more variety of data formats or to execute under different parameter settings would add a lot of value to the methods for some effort invested in this direction.

&nbsp;

# 7\. Resources and Supporting Material

Content reporting catalog:

[Content reporting catalog](https://gesisev.sharepoint.com/:x:/s/O365_Abteilung_KTS/EezrYEr2jYlApNGVavszrrgBOKlAN3mYHix1xTlRidN1CA?e=duOLgV&wdLOR=cC2A02109-B450-41BA-AD66-B582CD664A2C)

Social science software publishing venues:

[prominent social science software publishing venues](https://gesisev.sharepoint.com/:w:/s/O365_Team_KTS-BDA/Eb0_H8VsXRJMlH38ykigwR4BzChexXqfWIhEZsWWUuVcxg?e=Tlwp4N)

Templates

[CFF-template](https://gesisev.sharepoint.com/:u:/s/O365_Team_KTS-BDA/EaNptjMTYLxJjGJirpC35uoBV0YhngXvU9TsHjhguuJxJw?e=R2gZkB)

[MethodReadmeTemplate-V0.1](https://gesisev.sharepoint.com/:t:/s/O365_Team_KTS-BDA/Eb-RQSD_VklKk53OjY4sgpYBcq5RWDsL8KVyeKlmhBGmHA?e=gAiP5Y)

[TutorialTemplate0.2](https://gesisev.sharepoint.com/sites/O365_Team_KTS-BDA/Freigegebene%20Dokumente/Forms/AllItems.aspx?id=%2Fsites%2FO365%5FTeam%5FKTS%2DBDA%2FFreigegebene%20Dokumente%2FGeneral%2FSTB%2FMethodsHub%2FContentCollectionGuidelines%2FMethodSubmissionGuidelines%2Ftutorial%2Dtemplate%2Ftutorial%2Dtemplate%2Dv0%2E2%2Emd&parent=%2Fsites%2FO365%5FTeam%5FKTS%2DBDA%2FFreigegebene%20Dokumente%2FGeneral%2FSTB%2FMethodsHub%2FContentCollectionGuidelines%2FMethodSubmissionGuidelines%2Ftutorial%2Dtemplate&p=true&ga=1)

Social science relevance / DBD applicability:

[writing social science use cases](https://gesisev.sharepoint.com/:w:/s/O365_Team_KTS-BDA/EUtz1wwvnIlIiu12tJkINZcBNLqQiCE_ToJBGOMnoMyufg?e=9LtaNK)

[GESIS DBD dataset](https://www.gesis.org/en/institute/digital-behavioral-data)

[_Methods/task categories_](https://gesisev.sharepoint.com/:w:/s/O365_Team_STB_WP_Methods_Hub/EQ5KNJ95AodNq7weScTp6jsBx8E3CkUA-Aq90xWc_QPMbg?e=Su9MaL)

Code Reusability

[General code quality guidelines](https://gesisev.sharepoint.com/:w:/r/sites/O365_Team_KTS-BDA/_layouts/15/Doc.aspx?sourcedoc=%7BC14DBA5D-412F-43A6-8206-494DA574CE22%7D&file=naming-conventions-code.docx&action=default&mobileredirect=true)

[Method environment virtualization](https://gesisev.sharepoint.com/:w:/r/sites/O365_Team_KTS-BDA/_layouts/15/Doc.aspx?sourcedoc=%7B5706327B-AFD1-471E-833E-742252D9B0A7%7D&file=supplementary-for-methods.docx&action=default&mobileredirect=true), freezing requirements

# 9\. References

<https://zis.gesis.org/submissionFiles/ZISPublicationGuideEnglishV2.1.pdf>

1. <https://code.org/curriculum/docs/k-5/glossary> [↑](#footnote-ref-2)

2. <https://gesisev.sharepoint.com/:x:/s/O365_Abteilung_KTS/EezrYEr2jYlApNGVavszrrgBOKlAN3mYHix1xTlRidN1CA?e=duOLgV&wdLOR=cC2A02109-B450-41BA-AD66-B582CD664A2C> [↑](#footnote-ref-3)
