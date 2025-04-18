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

The quality criteria for documentation ensure that all information required for the application of a method and the reproducibility of results is documented in a standardized and easily comprehensible manner. To this end, the following sections provide recommendations that extend the mandatory [checklist items](README.md#documentation-quality-criteria).

#### Configuration Files

If enabled in the submission form, methods on the Methods Hub can be executed in an interactive environment using [binder](https://mybinder.readthedocs.io/en/latest/index.html). For such methods, the repository needs to adhere to the [binder configuration file requirements](https://mybinder.readthedocs.io/en/latest/using/config_files.html) (which are mostly the same as for Methods Hub).

#### Methods Hub Friendly README

Providing a [Methods Hub friendly README](method-README-template.md) ensures that the method is described in a standardized format that is accessible for social scientists. In addition to the specifics that the linked template file mentions for each section, we recommend the following:

- The README should contain as little computer science jargon as possible. Technical terms should be explained if they can not be avoided.
- If the README mentions code files, it should also [link to them](https://daringfireball.net/projects/markdown/syntax#link).
- The README should for each image (e.g., data models, pipeline, schema structure) also contain an explanation in text.
- The README should not contain information of programming interfaces or similar if it could instead link to the authoritative source.

#### postBuild File

The postBuild file is used to render the Methods Hub friendly README to HTML. This process can be tested using Quarto, and can be automated on Github using the [preview action](https://github.com/GESIS-Methods-Hub/preview?tab=readme-ov-file#usage).

### Code Quality Criteria

The code quality criteria ensure that the code is easy to use and modify. To this end, we recommend the following in addition to the mandatory [checklist items](README.md#code-quality-criteria):

- The method should not depend on certain other methods, but should use open formats for input and output. If there are standard formats for the particular task at hand, these should be used to ensure the interoperability of the methods.
- The method should be easy to configure. A configuration through command line parameters and/or configuration files is preferable over having to edit the source code.
- The method code should follow basic coding standards (e.g., of [Google](https://google.github.io/styleguide/) or [GNU](https://www.gnu.org/prep/standards/standards.html)).
- The method repository should contain unit tests that test for common, borderline and unusual cases to ensure that the method works as expected.
- The method repository should allow for generating technical documentation (e.g., using [Sphinx](https://www.sphinx-doc.org) or similar tools).

## Method Identification

Researchers and practitioners working in computational social science, computer science and natural language processing can identify methods as computational modules performing a specific task in the context of a research or development project concerning digital behavioral data.

1. It can be a few snippets of code that does something meaningful on the input data to give consistent and reliable output that is useful in the bigger picture. For example, POS tags or synonyms to words using built-in library.
2. It may also be acquired through code modularization where each module can be seen as a specific method e.g., the data collection module will be a data collection method from a given source, the preprocessing module can be the preprocessing method offering certain preprocessing options on the input data. This is the most prevalent form of method that gives the users freedom to pick different methods according to their requirements and align them in the pipeline that suits their intended purpose.  
3. It can also be a longer pipeline that has multiple code modules performing multiple tasks in a sequence. For example, collecting data from an online source, preprocessing it and vectorizing which is then consumed by an artificial intelligence model for analysis. It may also be complete end-to-end pipeline from data collection to analysis and visualizations. These methods are more helpful for getting quick results and proof of concept on a task. Both (2) and (3) have their own value and audience groups.  
4. Software application type of method, although not a common form of method represents software applications that can be downloaded and used directly, e.g., installing [ScienceLinker](https://git.gesis.org/sciencelinker/sciencelinker-development) through pip.

Generally, a method coded for a research model would have specific settings according to the data and research questions. However, generalizing the method to deal with more variety of data formats or to execute under different parameter settings would add a lot of value to the methods for some effort invested in this direction.

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
