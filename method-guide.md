# Method Submission Guide

*This document serves as a guide for developing and submitting methods to the Methods Hub. It assists in method preparation through checklist, template and guidelines to ensure conformance to the defined standards.*

## Abstract

The Methods Hub is an infrastructure project whose goal is to provide open and accessible computational methods to collect, access, and work with Digital Behavioral Data (DBD). The bulk of methods will stem from computer science, notably showcasing cutting-edge AI/ML techniques, alongside those originating from social sciences. It aims to serve as a pioneering platform designed to facilitate the propagation of computer science methodologies into social science research.

*Verify conformance to the method guidelines using the [method checklist](https://github.com/GESIS-Methods-Hub/guidelines-for-methods/blob/main/method-checklists)*

## Methods Hub Content Goal

The goal of Methods Hub content is to provide reusable, reviewed and relevant methods to social scientists that are appliable to Digital Behavioral Data.

## Methods Hub Content Objectives

Methods Hub content has the following objectives:

1. Enabling reuse of recent AI/ML models on Digital Behavioral Data in social science
2. Empower social scientists in using AI methods
3. Allows AI/ML method developers to reach a wider audience and contribute cross domain research challenges

## Glossary

| Term     | Explanation  |
|----------|--------------|
| Method   | Code snippets, one or more programming function , one or more programming classes or modularized software source code and its documentation. |
| Tutorial | A stepwise guide with or without code that explains working with an important tool, technology, or the available method(s). Tutorials facilitate and enable researchers to work with SOTA methods. |

## List of Abbreviations

| Abbreviation | In full |
|--------------|---------|
| DBD   | Digital behavioral data |
| MH    | Methods Hub |
| CFF   | Citation File Format |
| AI/ML | Artificial Intelligence/Machine Learning  |
| SOTA  | State-of-the art |

## 1. Methods (Computational Methods)

Methods Hub contains state-of-the-art AI/ML methods that can be applied to social science use cases and research questions. Only a fraction of these state-of-the-art methods is being used in the social science domain. However, there exists a vast array of untapped potential methods that can significantly provide benefits to the field. The community is encouraged to follow this guide to identify, develop and share advanced AI/ML methods specifically prepared for the social science community. Offering such content through the Methods Hub portal make them directly available to the target audience. This document serves as a guide for preparing methods to be Methods Hub ready.

It encourages existing methods that are relevant and of interest to social scientists to be offered through the Methods Hub platform. New research modules cna be developed keeping these guidelines in mind to share them through the Methods Hub platform as well. Alternate criteria is also defined to facilitate prominant method Git Repositories that are highly desired by the community to be inclusive while staying within scope of the Methods Hub.

### 1.1. Methods Dimensions

Methods Hub portal stands on the principles of open science only facilitating content that is developed with open resources and is made publicly available with open license. The methods submitted are reviewed from three overlapping dimensions to ensure that they meet the requirements of the Methods Hub. They are:

1. Method relevance i.e., the method is applicable to social science use cases or research questions. Can the method be used with DBD.
2. Recent AI/ML methods i.e., a SOTA method in the computer science or social science community.
3. Method quality i.e., good code and documentation quality. The code quality ensures that the code is easy reuse and modify if need be. The documentation quality that ensures that all necessary information to replicate results are correctly documented in an easy to follow manner. *Note: We follow a lightweight journal like review process to verify the method quality*. We also accept the review of trusted third parties e.g., renowned software publishing venues to make sure that the method is well documented and require minimum effort to understand and reuse for new research questions and use cases.

The methods recently developed in the computer science community with AI/ML and NLP models are more often representing as SOTA research. However, they need to establish relevance for applicability of the method in social science. The guidelines assist in crafting the method README for this purpose. Whereas the methods developed in the social science community are known to be relevant to the social science community already, but they may not always be using SOTA AI/ML models. The method review process ensures that the methods shared through the Methods Hub platform are representing SOTA AI/ML methods and have established relevance with social science use cases.

### 1.2. Trusted Third-party Review Bodies

There are journals and other software publishing venues that ensures the software is reusable and well-documented through a review process. Some of the trusted software publishing venues in computer science and social science venues are listed here ([prominent social science software publishing venues](supporting-documents/prominent-venues.md)). *The list is expected to grow with newer venues identified and reported*. These venues have well defined documentation requirements to make the code readable, understandable, and reusable. *For example, [sweater: Speedy Word Embedding Association Test and Extras Using R](https://joss.theoj.org/papers/10.21105/joss.04036)*. The code is reviewed for its quality too; therefore, these methods already comply with the MH method submission requirements and can be submitted directly.

### 1.3. Alternative for Established Methods

The prominent AI/ML methods that are applicable and of interest in the social science domain, having well established Git Repositories with active communities can also be added to Methods Hub. As a bridge, Methods Hub extends the use of these methods to social science research community allowing more methods to choose from and modify for their research questions. Such established method Git Repositories e.g., [SANSA](https://sda.tech/author/hajirajabeen/) and [BERD-NFDI](https://github.com/BERD-NFDI/bear-ml/tree/main/bearml) are of value in the social science domain as well. To establish relevance with these methods, an alternative option is provided i.e., to write tutorials that demonstrate the use of these methods on a social science use case, as a step-wise easy to follow process. The [tutorial template](https://github.com/GESIS-Methods-Hub/guidelines-for-tutorials) provides details on writing a tutorial for MH. This also facilitates to indirectly include a variety of methods on different platforms through the tutorial.

*Note: Follow the [method checklist](https://github.com/GESIS-Methods-Hub/guidelines-for-methods/blob/main/method-checklists) to ensure all requirements for publishing method through the MH are already met.*

## 2. Method Preconditions

There are three preconditions following open access protocols. To fulfill preconditions, the methods must be scripted in open language, are publicly accessible and have an open license. The platform supports scripts in open languages e.g., Python, R etc. and does not cover commercial tools e.g., MATLAB, SPSS etc. The code must be publicly accessible to all from popular code sharing platforms like GitHub or GitLab.

Licenses like [MIT open license](https://github.com/git/git-scm.com/blob/main/MIT-LICENSE.txt), [Apache 2.0 open license](https://github.com/apache/.github/blob/main/LICENSE) and CC-BY 4.0 are popular open-source licenses widely used in the GitHub community. The MIT license is known for its simplicity and permissiveness, allowing developers to freely use, modify, and distribute the software while requiring them to include the original license and disclaimer in any substantial portions of the code. The Apache License 2.0 is a more comprehensive license that provides clear guidelines on contributions, patents, and liability. Although these three are suggested as the frequently used open-source licenses, it doesn’t limit the use of any other open-source license.

## 3. Scoping Criteria

Methods Hub is a method market for social science methods and, therefore, the content submitted in the Methods Hub portal must be relevant to social science. Therefore, the scope criteria are defined around relevance of the method to the social science domain. The scope of the method is determined by;

### 3.1. Relevance to Social Science

The method has relevance to social science demonstrated through method documentation as:

1. Write use case(s) or research questions in the README file of the method that are directly related to social science. Provide use cases that showcase how the method can be generalized to different scenarios, therefore establishing a strong relevance with the social science audience.  
2. Provide evidence that the method can be used DBD datasets (ideally providing link to the [GESIS DBD dataset](https://www.gesis.org/en/institute/digital-behavioral-data)). It also assists in demonstrating relevance to social science through applicability to data from digital social platforms. More on this, along with sample data can be provided in the "Input Output Data" section in README.  
3. The method fits into the method tasks defined as loose vocabulary.

Note: In case of any difficulty in assigning a method to its relevant task, please report to Methods Hub Team

### 3.2. Tasks

The tasks that the method can perform is presented as loose vocabulary refering tasks and subtasks in a hierarchical manner. The method submission expects the method to have a specific task from the [Method Tasks Taxonomy](methods-tasks.md).

## 4. Method Quality Guidelines

Computational methods are the most common type of content on the Methods Hub. It aims to lower the technical barriers for using recent AI/ML methods in social science, while encouraging to develop reusable methods.

### 4.1. Method Documentation Quality

#### 4.1.1. Required Documents

The method documentation must contain at least the following four types of documents.  

1. README file in [method template](https://github.com/GESIS-Methods-Hub/guidelines-for-methods/blob/main/method-README-template.md)
2. Configuration file i.e., Requirements.txt, install.R, configuration.yml etc.
3. [Citation File Format (.CFF), CITATION file](https://citation-file-format.github.io/) or alternative for citing method
4. License file (e.g. [MIT](https://github.com/git/git-scm.com/blob/main/MIT-LICENSE.txt), [Apache 2.0](https://github.com/apache/.github/blob/main/LICENSE), CC-BY 4.0)
5. The Git repository has the [necessary files for setting up a binder environment](https://mybinder.readthedocs.io/en/latest/using/config_files.html)[^1]. For example, adding `binder/postBuild` file, using [postBuild](https://methodshub.gesis.org/snippet/postBuild) to the Git Repository

*There must be only one of these files in the Git Repository to avoid confusion. All the other versions of these files should be organized in subdirectories.*

The **README file** is crucial for the readability, understandability, and reusability of the method. It may also contain optional subsections of disclaimer, acknowledgements, or publication, if applies. However, it is very important to mention the developer contact details to help reach back to the developer if need be.

There must be a **[configuration file](https://mybinder.readthedocs.io/en/latest/using/config_files.html)** that recreates the environment in which the method is used (i.e., requirements.txt, install.R, environment.yml etc.) file. It helps reusability of the method by executing it in the same environment it was originally created in. The [Turing Way](https://book.the-turing-way.org/index.html) provides a comprehensive guideline on how to produce this configuration file.

**[Citation file formats (CFF)](https://citation-file-format.github.io/)** are standardized structures designed to capture and represent bibliographic information about scholarly references. This file contains metadata such as author names, author ORCID, method title, method developed date etc. to help cite the method as a resource in scholarly articles. The [citation(template).cff](https://citation-file-format.github.io/) can be modified for a method.

**Open licenses** like [MIT open license](https://github.com/git/git-scm.com/blob/main/MIT-LICENSE.txt), [Apache 2.0 open license](https://github.com/apache/.github/blob/main/LICENSE) and CC-BY 4.0 are popular open-source licenses widely used in the GitHub community. Although these three are suggested as the frequently used open-source licenses, it doesn’t limit the use of any other open-source license.

*Providing these files boost open research culture, attribution and may lead to newer collaborations.*

#### 4.1.2 README guidelines

The README document of the method needs to follow the documentation quality guidelines provided here. The methods submitted will undergo a review process to ensure compliance with the guidelines. It is also aligned with the objectives of the Methods Hub to keep high quality content only.

The most important aspect to consider in writing the README of a method is its user friendliness. It emphasizes the need for having easy to understand and easy to follow documentation. The README description should explain the working of the method with social science terminologies, link to specific publications at social science venues. The research questions and use cases for the method should also be from the social science domain. In general, social scientists from different backgrounds should be able to follow the guidelines and reuse the method, aligned with the objective of Methods Hub, i.e., lowering technical barriers. The main README suggestions are:

- Avoid jargon in the method name, description, and use cases to help understandability of the README file for social scientists.
- README should link to different code files where necessary.
  - Any external information e.g., on the terms of API used in the method should link to the original instead of copying those points to the README as they may change over time.
  - Internal resources utilized by the method e.g., embeddings, preprocessing etc. should linked for transparency.
- The description should link to relevant social science publication using similar method.
- README should have crisp use cases that help to highlight the purpose of the method e.g., identifying positive and negative sentiment scores of tweets.
- The technical terms needed to help understand the method's purpose are to be explained separately as a list of definitions.
- Use appealing subsection headings to attract the audience.
  - Do not remove/change the original sections/subsections in the README template
  - For each subsection to rename, use separator (-) after the name in the template and then provide your subsection name e.g., Description - Why Topic Modeling.
  - Remove (Optional) from the title of the subsections that applies for your method. Remove all other optional subsections that do not apply.
- Show sample input and output of the method to help users understand the purpose of the method.
  - A method Git Repository must have a sample input data and output data to help replicate results.
  - The sample input and output should represent one of the use cases.
  - There should be some explanation of what the input and output means in layman terms.
  - The use cases may also be documented as research questions.
- The “How to use” section should have more details to elaborate on the use of the method
  - Providing a step-by-step guide to call the method and what to expect after each step.
  - It should provide how to apply different filters or parameter settings for the method. For example, calling the method topic modeling with different input data and configurations to expect different number of topics and arrangement of words within.
- In the Git Repository Structure” subsection, provide structure of your Git Repository in the form of a tree, to help navigate the directories easily.
- Images used in the README e.g., data models, pipeline, schema structure etc. should be properly explained.
- In the “Contact” subsection, mention your contact details that users can use to follow up in case of queries.
- Provide a limitation subsection mentioning the limitations of the method, if any.

The [README(template).md](method-README-template.md) has more on the structure of the document and how to write relevant information in each of these sections.

### 4.2. Method Code Quality

#### 4.2.1. Code Quality Guidelines

Writing code that is easy to (re)use, easy to maintain and easy to adapt is crucial for having methods that remain reusable over a longer period of time. Maintaining coding standards is highly desired and the following guidelines will assist in achieving it:

- The method should follow basic coding standards provided in the document ([basic coding conventions](supporting-documents/naming-conventions-code.md)). It refreshes the concepts of using consistent naming conventions and readable coding structures. However, its purpose is not to restrict developers to a single coding style.
- The code must be well structured and sufficiently commented.
- Similarly, pushing important decisions from the body of the method to the parameters to empower users alter the behavior of the method. Such parameters should be read from a separate 'config.json' file. The code should be flexible to follow different reuse based on the parameter settings file.  
- Unit tests should be provided to ensure the code is free from errors and all/most of the boundary conditions are checked.  
- The method code, in case taken from a bigger pipeline, should be modularized with minimum/no coupling or external dependencies.
- Technical documentation for the code (generated through a tool e.g., sphinx) are desired

*Defining method input and output interfacing as defined for the other methods used for the same task will help eaiser switch among methods to experiment with. It minimize the effort for the user to try different methods for the same task in their pipeline. Sci-kit-learn is a very good example for it. However, since Methods Hub is driven by community, it doesn't mean to standardize method interfacing at the MH level. The diversity and freedom in coding style is also equally important as far as the code is clearly readable, understandable and reusable.*

#### 4.2.2. Code Reusability

The method code should be reusable so that social scientists can apply it to their research questions.

- The “Enviornmental Setup” or “How to Use” along with "Input and Output Data" subsections should be sufficient replicate the results for the sample data without any invovlement of the user in the code i.e., just by executing code files or cells of notebook.
- The sample output must be consistently produced across multiple runs. Define random seeds to ensure same results.

**Reusability Supporting material:** The supporting material document is an early-stage effort in assisting developers to know about the tools and techniques to develop reusable methods. At present it helps on:

1. Creating and using virtual environments
2. Generating random seeds
3. Suggesting useful reproducibility tools

This document is expected to grow with time through contributions from the method developers and reviewers towards building a resource for facilitating efficient method development.

*Note: For methods in release 1 (scheduled in June 2024), ensuring that the method reusability and code quality is the responsibility of the method developer. The method Git Repository usage statistics (if available) are also considered e.g., watchers, downloads, forks, commits etc. In evaluating the code quality.*

## 5. Method Identification

Researchers and practiioners working in computational social science, computer science and natural language processing can identify methods as computational modules performing a specific task in the context of a research or development project concerning digital behavioral data.

1. It can be a few snippets of code that does something meaningful on the input data to give consistent and reliable output that is useful in the bigger picture. For example, POS tags or synonyms to words using built-in library.
2. It may also be acquired through code modularization where each module can be seen as a specific method e.g., the data collection module will be a data collection method from a given source, the preprocessing module can be the preprocessing method offering certain preprocessing options on the input data. This is the most prevalent form of method that gives the users freedom to pick different methods according to their requirements and align them in the pipeline that suits their intended purpose.  
3. It can also be a longer pipeline that has multiple code modules performing multiple tasks in a sequence. For example, collecting data from an online source, preprocessing it and vectorizing which is then consumed by an AI/ML model for analysis. It may also be complete end-to-end pipeline from data collection to analysis and visualizations. These methods are more helpful for getting quick results and proof of concept on a task. Both (2) and (3) have their own value and audience groups.  
4. Software application type of method, although not a common form of method represents software applications that can be downloaded and used directly, e.g., installing [ScienceLinker](https://git.gesis.org/sciencelinker/sciencelinker-development) through pip.

Generally, a method coded for a research model would have specific settings according to the data and research questions. However, generalizing the method to deal with more variety of data formats or to execute under different parameter settings would add a lot of value to the methods for some effort invested in this direction.

## 6. Resources and Supporting Material

- Social science software publishing venues: [prominent social science software publishing venues](prominent-venues.md)
- Templates
  - [CFF-template](https://citation-file-format.github.io/)
  - [method template](method-README-template.md)
  - [tutorial-template.md](https://github.com/GESIS-Methods-Hub/guidelines-for-tutorials)
- Social science relevance / DBD applicability:
  - [GESIS DBD dataset](https://www.gesis.org/en/institute/about-us/digital-behavioral-data)
- Code Reusability
  - [postBuild](https://methodshub.gesis.org/snippet/postBuild)
  - [General code quality guidelines](supporting-documents/naming-conventions-code.md)
  - [Method preview as GitHub Action](https://github.com/GESIS-Methods-Hub/preview?tab=readme-ov-file#usage)

## 7. References

[https://zis.gesis.org/submissionFiles/ZISPublicationGuideEnglishV2](https://zis.gesis.org/submissionFiles/ZISPublicationGuideEnglishV2)

## FAQs

**What is Methods Hub?**
Methods Hub is an infrastructure platform that provides openly accessible, reusable computational methods for working with Digital Behavioral Data (DBD) in social science research.

**Who can submit a method to the Methods Hub?**
Researchers, practitioners, and developers in computational social science, computer science, natural language processing and related fields can submit methods.

**Can I publish my computational method on Methods Hub?**
Yes, only if it is open access and open licensed, applies to a social science use case/research question and is applicable to Digital behavioral data.

**How can I increase my chances of getting my method published?**
By providing well written documentation following README template, providing all necessary files and making the code reusable without/with minimal user involvement.

**Which programming languages are supported?**
The platform supports open languages such as Python and R, but not commercial tools like MATLAB or SPSS.

**Can I publish my method using paid API or tool?**
No, the methods on Methods Hub must be fully resusable with all resources used by the method including APIs, packages being openly accessible to all.

**What if my method is already published in a peer-reviewed journal?**
Methods published in trusted third-party venues with proper documentation and code quality can be submitted directly.

**Can I submit a method that is not AI/ML-based?**
The focus is on state-of-the-art AI/ML methods, but methods that support social science research using Digital Behavioral Data in other ways may also be considered e.g., data cleansing, data preprocessing etc.

**Should I write tutorial about my method?**
Yes, tutorials increase the reach of a method to researchers and practitioners with limited practical experience of AI/ML methods. It is therefore, highly advised to write tutorial demonstrating the use of your method to a research question as step-by-step guide.

**Can I write tutorial about someone else's method?**
Yes, you can write a tutorial about other developers methods as your contribution. You can also write tutorials about methods not published on Methods Hub but are of interest to the Methods Hub audience. For more details, please visit the method guide and template.

**Where should the method code be hosted?**
The method must be publicly accessible on GitHub.

**What happens when I submit my method?**
When the method is submitted, it is held for review. During this period the reviewer(s) can add issues to the Git Repository if modifications are needed. Once there is no issue to resolve, the method is published on the portal.

**What does it mean that a method is published?**
When a method is published, it appears in the Methods Hub gallery and (from next day) is searchable through GESIS Search.
