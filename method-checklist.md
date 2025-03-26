# Method publishing checklist

Please follow the checklist to ensure your content is ready for publishing on the [Methods Hub portal](https://methodshub.gesis.org/). *Note: the content submitted for publishing is held for review to crosscheck all requirements before publishing.*

Methods that have [established communities](https://github.com/GESIS-Methods-Hub/guidelines-for-methods/blob/main/method-submission-guidelines.md#13alternative-for-established-methods) or are published by [trusted third parties](https://github.com/GESIS-Methods-Hub/guidelines-for-methods/blob/main/method-submission-guidelines.md#12trusted-third-party-review-bodies) can be considered as special case (bypassing some of the documentation requirements) for publishing through Methods Hub. *Please consult Methods Hub Team first by [email][methodshub-email] for further details.*

## Checklist
### Preconditions as openness criteria
- [ ] Developed in an open-source programming language e.g., Python, R. 
- [ ] The method is publicly accessible. 
- [ ] Has open license.

For more details check the [Method Preconditions](https://github.com/GESIS-Methods-Hub/guidelines-for-methods/blob/main/method-submission-guidelines.md#3-method-preconditions) section of the guidelines.

### Scope criteria as relevance to social science
- [ ] Establishing social science relevance through use case, research question or citing relevant social science publications. 
- [ ] The method is applicable to Digital Behavioral Data (DBD) (ideally [GESIS DBD](https://www.gesis.org/en/institute/about-us/digital-behavioral-data)), also demonstrated through sample data in the Git Repository. 
- [ ] The method has a relevant task in the [Method Tasks Taxonomy](https://github.com/GESIS-Methods-Hub/guidelines-for-methods/blob/main/methods-tasks.md).

For more details check the [Scoping Criteria](https://github.com/GESIS-Methods-Hub/guidelines-for-methods/blob/main/method-submission-guidelines.md#4-scoping-criteria) section of the guidelines.

### Code and documenation quality

#### Documentation quality
- [ ] Has configuration files i.e., `environment.yml`, `requirements.txt`, `install.R`.
- [ ] Has open license file e.g., MIT open license, Apache 2.0 open license and CC-BY 4.0 etc. (for more on [GitHub licenses](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/adding-a-license-to-a-repository)).
- [ ] Has [Citation File Format (.CFF), CITATION file](https://citation-file-format.github.io/) or alternative for citing the method. 
- [ ] Has README file in [method template](https://github.com/GESIS-Methods-Hub/guidelines-for-methods/blob/main/method-README-template.md). 
- [ ] The Git repository has the [necessary files for setting up a binder environment](https://mybinder.readthedocs.io/en/latest/using/config_files.html)[^1]. For example, adding `binder/postBuild` file, using [postBuild](https://methodshub.gesis.org/snippet/postBuild) to the Git Repository. 

#### Code quality
- [ ] The code is executable using the information in README.
- [ ] The method replicates the sample output using the sample input in the Git Repository (if applicable).
- [ ] The Parameters and decisions used in the code are sufficiently commented to assist in updating the method behavior. 
- [ ] The method is reproducible using only publicly available resources i.e., not using any commercial tools, packages, APIs etc. 
- [ ] The code is structured into modules (if need be) and is sufficiently commented to facilitate modification.

For more details on documentation and code quality, check the [Method Quality Guidelines](https://github.com/GESIS-Methods-Hub/guidelines-for-methods/blob/main/method-submission-guidelines.md#5-method-quality-guidelines) section of the guidelines.

## Contact

Methods Hub Team &lt;[methodshub@gesis.org][methodshub-email]&gt;

[methodshub-email]: mailto:methodshub@gesis.org
