# Methods Hub's Guidelines for Methods

Here you will find the guidelines used by Methods Hub for methods. If you are preparing a tutorial, check the [guidelines used by Methods Hub for tutorials](https://github.com/GESIS-Methods-Hub/guidelines-for-tutorials).

The Methods Hub aims to provide high-quality and easy-to-use computer science methods to social scientists. Offering such methods through the Methods Hub makes them directly available to the target audience. However, the Method Hub only accepts methods that follow the principles of open science, that are available in a format that is accessible for social scientists and that are relevant for social science research. A special focus of the Methods Hub is on methods that work on [digital behavioral data](https://www.gesis.org/en/institute/about-us/digital-behavioral-data), but also other methods are welcome.

A method for the Methods Hub is a sequence of instructions that a computer should execute to perform a specific task and that is bundled for reusability, as well as its documentation.

To be included in the Methods Hub, a method is checked to see if it fulfils the criteria in the [method-publishing-checklist](#method-publishing-checklist) below. If you believe your method meets these criteria, submit it for review on the [Methods Hub Portal](https://methodshub.gesis.org). After acceptance, consider to [write and submit a tutorial](https://github.com/GESIS-Methods-Hub/guidelines-for-tutorials) for your method.

## Method publishing checklist

Each method submitted to the [Methods Hub](https://methodshub.gesis.org/) is checked for compliance with the following criteria before publication.

### Openness criteria

- [ ] The method is developed in an open-source programming language (e.g., Python or R).
- [ ] The method is publicly accessible in a Git Repository that does not contain other methods.
- [ ] The method is [published under an open license](https://opensource.guide/legal/#which-open-source-license-is-appropriate-for-my-project).

### Scoping criteria

- [ ] The method is relevant for the social sciences (shown through use cases in the Methods Hub friendly README of the repository; see [documentation quality criteria](#documentation-quality-criteria)).
- [ ] The method is applicable to Digital Behavioral Data (ideally [GESIS DBD](https://www.gesis.org/en/institute/about-us/digital-behavioral-data); shown through sample data in the Git Repository).
- [ ] The method belongs to a relevant task type of the first (most abstract) level of the [Method Tasks Taxonomy](tasks.md) (has to be selected in the submission form; if none of the current second level types fits the method, please contact us at [methodshub@gesis.org][methodshub-email] to extend the taxonomy).

### Quality criteria

#### Documentation quality criteria

- [ ] The method repository contains the configuration files for installing all requirements (e.g., `environment.yml`, `requirements.txt`, `install.R`).
- [ ] The method repository contains a `LICENSE` file (corresponding to an [open license](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/adding-a-license-to-a-repository)) at the root level of the repository.
- [ ] The method repository contains a [`CITATION.cff`](https://citation-file-format.github.io/) file at the root level of the repository.
- [ ] The method repository contains a [Methods Hub friendly README](https://github.com/GESIS-Methods-Hub/guidelines-for-methods/blob/main/README-template.md?plain=1) (can be  `README.me` or another file; has to be selected in the submission form).
- [ ] The method repository contains the [postBuild](https://methodshub.gesis.org/snippet/postBuild) file at the root level of the repository.

#### Code quality criteria

The code quality criteria can be skipped for methods for which a paper is published by [trusted third-party review venues](guidelines.md#trusted-third-party-review-venues).

- [ ] By executing the code as described in the Methods Hub friendly README of the repository (see [documentation quality criteria](#documentation-quality-criteria)), the sample output described in the same file is generated with adequate fidelity (e.g., the output can be different for methods relying on randomness or external data sources).
- [ ] The execution relies only on publicly available resources.
- [ ] The method code contains documentation (comments) for parameters and decisions that allows one to adjust the method.
- [ ] The method code is structured into modules (if need be).

For more details on documentation and code quality, check the [Quality Criteria](guidelines.md#quality-criteria) section of the guidelines.

## Contact

Methods Hub Team &lt;[methodshub@gesis.org][methodshub-email]&gt;

[methodshub-email]: mailto:methodshub@gesis.org
