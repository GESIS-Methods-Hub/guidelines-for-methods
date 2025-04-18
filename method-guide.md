# Method Submission Guidelines

The Methods Hub aims to provide high-quality and easy-to-use computer science methods to social scientists. A special focus of the Methods Hub is on [digital behavioral data](https://www.gesis.org/en/institute/about-us/digital-behavioral-data). Offering such methods through the Methods Hub makes them directly available to the target audience. However, the Method Hub only accepts state-of-the-art methods that follow the principles of open science, that are available in a format that is accessible for social scientists and that are relevant for social science research.

To prepare methods for inclusion into the Methods Hub, follow the [method publishing checklist](README.md#method-publishing-checklist). This checklist is also used to check whether a submitted method is ready for inclusion or whether further changes are required. The checklist links back to this document for details. After you checked all items in the list, continue with the submission process on the [Methods Hub portal](https://methodshub.gesis.org).

## Glossary

| Term     | Explanation  |
|----------|--------------|
| Method   | Code snippets, one or more programming function, one or more programming classes or modularized software source code and its documentation. |
| Tutorial | A stepwise guide with or without code that explains working with an important tool, technology, or the available method(s). |

## Quality Criteria

### Trusted Third-party Review Venues

For methods for which a paper is published at venues that ensure the methods reusability and documentation quality through a review process, the Methods Hub submission process is faster as the [documentation and code quality check](README.md#quality-criteria) is skipped. These venues are:

- [Journal of open source software](https://joss.theoj.org/)
- [The R journal](https://journal.r-project.org/)
- [R open science](https://ropensci.org/)

You can suggest further venues by mail to the [Methods Hub team][methodshub-email].

### Documentation Quality Criteria

The documentation quality criteria ensure that all necessary information to replicate results are correctly documented in an easy to follow manner.

#### Required Documents

The method documentation must contain at least the following four types of documents.  

1. README file in [method template](https://github.com/GESIS-Methods-Hub/guidelines-for-methods/blob/main/method-README-template.md)
2. Configuration file i.e., Requirements.txt, install.R, configuration.yml etc.
3. [Citation File Format (.CFF), CITATION file](https://citation-file-format.github.io/) or alternative for citing method
4. License file (e.g. [MIT](https://github.com/git/git-scm.com/blob/main/MIT-LICENSE.txt), [Apache 2.0](https://github.com/apache/.github/blob/main/LICENSE), CC-BY 4.0)
5. The Git repository has the [necessary files for setting up a binder environment](https://mybinder.readthedocs.io/en/latest/using/config_files.html)[^1]. For example, adding `binder/postBuild` file, using [postBuild](https://methodshub.gesis.org/snippet/postBuild) to the Git Repository

The **README file** is crucial for the readability, understandability, and reusability of the method. It may also contain optional subsections of disclaimer, acknowledgements, or publication, if applies. However, it is very important to mention the developer contact details to help reach back to the developer if need be.

There must be a **[configuration file](https://mybinder.readthedocs.io/en/latest/using/config_files.html)** that recreates the environment in which the method is used (i.e., requirements.txt, install.R, environment.yml etc.) file. It helps reusability of the method by executing it in the same environment it was originally created in. The [Turing Way](https://book.the-turing-way.org/index.html) provides a comprehensive guideline on how to produce this configuration file.

**[Citation file formats (CFF)](https://citation-file-format.github.io/)** are standardized structures designed to capture and represent bibliographic information about scholarly references. This file contains metadata such as author names, author ORCID, method title, method developed date etc. to help cite the method as a resource in scholarly articles. The [citation(template).cff](https://citation-file-format.github.io/) can be modified for a method.

**Open licenses** like [MIT open license](https://github.com/git/git-scm.com/blob/main/MIT-LICENSE.txt), [Apache 2.0 open license](https://github.com/apache/.github/blob/main/LICENSE) and CC-BY 4.0 are popular open-source licenses widely used in the GitHub community. Although these three are suggested as the frequently used open-source licenses, it doesn’t limit the use of any other open-source license.

*Providing these files boost open research culture, attribution and may lead to newer collaborations.*

#### README Guidelines

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

### Code Quality Criteria

The code quality criteria ensuree that the code is easy reuse and modify if need be.

#### Code Quality Guidelines

Writing code that is easy to (re)use, easy to maintain and easy to adapt is crucial for having methods that remain reusable over a longer period of time. Maintaining coding standards is highly desired and the following guidelines will assist in achieving it:

- The method should follow basic coding standards provided in the document ([basic coding conventions](supporting-documents/naming-conventions-code.md)). It refreshes the concepts of using consistent naming conventions and readable coding structures. However, its purpose is not to restrict developers to a single coding style.
- The code must be well structured and sufficiently commented.
- Similarly, pushing important decisions from the body of the method to the parameters to empower users alter the behavior of the method. Such parameters should be read from a separate 'config.json' file. The code should be flexible to follow different reuse based on the parameter settings file.  
- Unit tests should be provided to ensure the code is free from errors and all/most of the boundary conditions are checked.  
- The method code, in case taken from a bigger pipeline, should be modularized with minimum/no coupling or external dependencies.
- Technical documentation for the code (generated through a tool e.g., sphinx) are desired

*Defining method input and output interfacing as defined for the other methods used for the same task will help eaiser switch among methods to experiment with. It minimize the effort for the user to try different methods for the same task in their pipeline. Sci-kit-learn is a very good example for it. However, since Methods Hub is driven by community, it doesn't mean to standardize method interfacing at the Methods Hub level. The diversity and freedom in coding style is also equally important as far as the code is clearly readable, understandable and reusable.*

#### Code Reusability

The method code should be reusable so that social scientists can apply it to their research questions.

- The “Enviornmental Setup” or “How to Use” along with "Input and Output Data" subsections should be sufficient replicate the results for the sample data without any invovlement of the user in the code i.e., just by executing code files or cells of notebook.
- The sample output must be consistently produced across multiple runs. Define random seeds to ensure same results.

**Reusability Supporting material:** The supporting material document is an early-stage effort in assisting developers to know about the tools and techniques to develop reusable methods. At present it helps on:

1. Creating and using virtual environments
2. Generating random seeds
3. Suggesting useful reproducibility tools

This document is expected to grow with time through contributions from the method developers and reviewers towards building a resource for facilitating efficient method development.

*Note: For methods in release 1 (scheduled in June 2024), ensuring that the method reusability and code quality is the responsibility of the method developer. The method Git Repository usage statistics (if available) are also considered e.g., watchers, downloads, forks, commits etc. In evaluating the code quality.*

## Method Identification

Researchers and practitioners working in computational social science, computer science and natural language processing can identify methods as computational modules performing a specific task in the context of a research or development project concerning digital behavioral data.

1. It can be a few snippets of code that does something meaningful on the input data to give consistent and reliable output that is useful in the bigger picture. For example, POS tags or synonyms to words using built-in library.
2. It may also be acquired through code modularization where each module can be seen as a specific method e.g., the data collection module will be a data collection method from a given source, the preprocessing module can be the preprocessing method offering certain preprocessing options on the input data. This is the most prevalent form of method that gives the users freedom to pick different methods according to their requirements and align them in the pipeline that suits their intended purpose.  
3. It can also be a longer pipeline that has multiple code modules performing multiple tasks in a sequence. For example, collecting data from an online source, preprocessing it and vectorizing which is then consumed by an artificial intelligence model for analysis. It may also be complete end-to-end pipeline from data collection to analysis and visualizations. These methods are more helpful for getting quick results and proof of concept on a task. Both (2) and (3) have their own value and audience groups.  
4. Software application type of method, although not a common form of method represents software applications that can be downloaded and used directly, e.g., installing [ScienceLinker](https://git.gesis.org/sciencelinker/sciencelinker-development) through pip.

Generally, a method coded for a research model would have specific settings according to the data and research questions. However, generalizing the method to deal with more variety of data formats or to execute under different parameter settings would add a lot of value to the methods for some effort invested in this direction.

## Resources and Supporting Material

[Method preview as GitHub Action](https://github.com/GESIS-Methods-Hub/preview?tab=readme-ov-file#usage)

## FAQs

**What is the Methods Hub?**
The Methods Hub is an infrastructure platform that provides openly accessible, reusable computational methods for working with digital behavioral data in social science research.

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

**Can I submit a method that is not artificial-intelligence-based?**
The focus is on state-of-the-art artificial intelligence methods, but methods that support social science research using Digital Behavioral Data in other ways may also be considered e.g., data cleansing, data preprocessing etc.

**Should I write tutorial about my method?**
Yes, tutorials increase the reach of a method to researchers and practitioners with limited practical experience of artificial intelligence methods. It is therefore, highly advised to write tutorial demonstrating the use of your method to a research question as step-by-step guide.

**Can I write tutorial about someone else's method?**
Yes, you can write a tutorial about other developers methods as your contribution. You can also write tutorials about methods not published on Methods Hub but are of interest to the Methods Hub audience. For more details, please visit the method guide and template.

**Where should the method code be hosted?**
The method must be publicly accessible on GitHub.

**What happens when I submit my method?**
When the method is submitted, it is held for review. During this period the reviewer(s) can add issues to the Git Repository if modifications are needed. Once there is no issue to resolve, the method is published on the portal.

**What does it mean that a method is published?**
When a method is published, it appears in the Methods Hub gallery and (from next day) is searchable through GESIS Search.

[methodshub-email]: mailto:methodshub@gesis.org
