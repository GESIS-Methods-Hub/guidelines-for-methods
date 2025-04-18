# Methods Hub's Guidelines for Methods

Here you will find the guidelines used by Methods Hub for methods. If you are preparing a tutorial, check the [guidelines used by Methods Hub for tutorials](https://github.com/GESIS-Methods-Hub/guidelines-for-tutorials).

## Method publishing checklist

Each method submitted to the [Methods Hub](https://methodshub.gesis.org/) is checked for compliance with the following criteria before publication.

### Openness criteria

- [ ] The method is developed in an open-source programming language (e.g., Python or R).
- [ ] The method is publicly accessible in a Git Repository that it does not share with other methods.
- [ ] The method is [published under an open license](https://opensource.guide/legal/#which-open-source-license-is-appropriate-for-my-project).

### Scoping criteria

- [ ] The method is relevant for the social sciences (shown through use cases in the [method README](#documentation-quality-criteria)).
- [ ] The method is applicable to Digital Behavioral Data (ideally [GESIS DBD](https://www.gesis.org/en/institute/about-us/digital-behavioral-data); shown through sample data in the Git Repository).
- [ ] The method belongs to a relevant task type of the [Method Tasks Taxonomy](methods-tasks.md) (has to be selected in the submission form).

For more details check the [Scoping Criteria](method-guide.md#scoping-criteria) section of the guidelines.

### Quality criteria

Can be skipped for methods for which a paper is published by [trusted third-party review venues](method-guide.md#trusted-third-party-review-venues).

#### Documentation quality criteria

- [ ] The method repository contains the configuration files for installing all requirements (e.g., `environment.yml`, `requirements.txt`, `install.R`).
- [ ] The method repository contains a `LICENSE` file (corresponding to an [open license](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/adding-a-license-to-a-repository)).
- [ ] The method repository contains a [`CITATION.cff`](https://citation-file-format.github.io/) file.
- [ ] The method repository contains a [Methods Hub friendly README](method-README-template.md) (can be  `README.me` or another file; has to be selected in the submission form).
- [ ] The method repository contains the [postBuild](https://methodshub.gesis.org/snippet/postBuild) file.

#### Code quality criteria

- [ ] By executing the code as described in the Methods Hub friendly README, the sample output described in the same file is generated with adequate fidelity (e.g., the output can be different for methods relying on randomness or external data sources).
- [ ] The execution relies only on publicly available resources.
- [ ] The method code contains documentation (comments) for parameters and decisions that allows one to adjust the method.
- [ ] The method code is structured into modules (if need be).

For more details on documentation and code quality, check the [Method Quality Guidelines](method-guide.md#method-quality-guidelines) section of the guidelines.

## Contact

Methods Hub Team &lt;[methodshub@gesis.org][methodshub-email]&gt;

[methodshub-email]: mailto:methodshub@gesis.org
