# Method Submission Guidelines

This document expands on the information in the [README.md](README.md).

## Quality Criteria

### Documentation Quality Criteria

The quality criteria for documentation ensure that all information required for the application of a method and the reproducibility of results is documented in a standardized and easily comprehensible manner. To this end, the following sections provide recommendations that extend the mandatory [checklist items](README.md#documentation-quality-criteria).

#### Configuration Files

If enabled in the submission form, methods on the Methods Hub can be executed in an interactive environment using [binder](https://mybinder.readthedocs.io/en/latest/index.html). For such methods, the repository needs to adhere to the [binder configuration file requirements](https://mybinder.readthedocs.io/en/latest/using/config_files.html) (which are mostly the same as for Methods Hub).

#### postBuild File

The postBuild file is used to render the Methods Hub friendly README to HTML. This process can be tested using Quarto, and can be automated on Github using the [preview action](https://github.com/GESIS-Methods-Hub/preview?tab=readme-ov-file#usage).

### Code Quality Criteria

The code quality criteria ensure that the code is easy to use and modify. To this end, we recommend the following in addition to the mandatory [checklist items](README.md#code-quality-criteria):

- The method should not depend on certain other methods, but should use open formats for input and output. If there are standard formats for the particular task at hand, these should be used to ensure the interoperability of the methods.
- The method should be easy to configure. A configuration through command line parameters and/or configuration files is preferable over having to edit the source code.
- The method code should follow basic coding standards (e.g., of [Google](https://google.github.io/styleguide/) or [GNU](https://www.gnu.org/prep/standards/standards.html)).
- The method repository should contain unit tests that test for common, borderline and unusual cases to ensure that the method works as expected.
- The method repository should allow for generating technical documentation (e.g., using [Sphinx](https://www.sphinx-doc.org) or similar tools).

#### Trusted Third-party Review Venues

For methods for which a paper is published at venues that ensure the methods reusability and documentation quality through a review process, the Methods Hub submission process is faster as the [code quality criteria](README.md#code-quality-criteria) check is skipped. These venues are:

- [Journal of open source software](https://joss.theoj.org/)
- [The R journal](https://journal.r-project.org/)
- [R open science](https://ropensci.org/)

You can suggest further venues by mail to the [Methods Hub team][methodshub-email].

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
