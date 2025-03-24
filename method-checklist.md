# Method publishing checklist

Please follow the checklist to ensure your content is ready for publishing on the [Methods Hub portal](https://methodshub.gesis.org/). *Note: the content submitted for publishing is held for review to crosscheck all requirements before publishing.*

Methods that have [established communities](https://github.com/GESIS-Methods-Hub/guidelines-for-methods/blob/main/method-submission-guidelines.md#13alternative-for-established-methods) or are published by [trusted third parties](https://github.com/GESIS-Methods-Hub/guidelines-for-methods/blob/main/method-submission-guidelines.md#12trusted-third-party-review-bodies) can be considered as special case (bypassing some of the documentation requirements) for publishing through Methods Hub. *Please consult Methods Hub Team first by [email][methodshub-email] for further details.*

## Checklist
### Preconditions as openness criteria
- [ ] Developed in open-sourced programming language e.g., Python, R 
- [ ] Publicly accessible script 
- [ ] Open license

For more details check the [Method Preconditions](https://github.com/GESIS-Methods-Hub/guidelines-for-methods/blob/main/method-submission-guidelines.md#3-method-preconditions) section of the guidelines.

### Scope criteria as relevance to social science
- [ ] Establishing social science relevance through use case, research question or citing relevant social science publications 
- [ ] The method is applicable to Digital Behavioral Data (DBD) (ideally [GESIS DBD](https://www.gesis.org/en/institute/about-us/digital-behavioral-data)), also demonstrated through sample data in the repo 
- [ ] The method has a relevant task in the Methods Hub task vocabulary (for more on [method tasks](https://github.com/GESIS-Methods-Hub/guidelines-for-methods/blob/main/methods-tasks.md))

For more details check the [Scoping Criteria](https://github.com/GESIS-Methods-Hub/guidelines-for-methods/blob/main/method-submission-guidelines.md#4-scoping-criteria) section of the guidelines.

### Code and documenation quality

#### Documentation quality
- [ ] Configuration file i.e., `environment.yml`, `requirements.txt`, `install.R`.
- [ ] Open license file e.g., MIT open license, Apache 2.0 open license and CC-BY 4.0 etc. (for more on [GitHub licenses](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/adding-a-license-to-a-repository))
- [ ] [Citation File Format (.CFF), CITATION file](https://citation-file-format.github.io/) or alternative for citing method 
- [ ] README file in [method template](https://github.com/GESIS-Methods-Hub/guidelines-for-methods/blob/main/method-README-template.md) 
- [ ] Add binder/postbuild file to your repo for Methods Hub homepage rendering, by copying [postBuild](https://methodshub.gesis.org/snippet/postBuild) to repo 
- [ ] Optional: Verify Methods Hub rendering of your repo by [previewing as GitHub Action](https://github.com/GESIS-Methods-Hub/preview?tab=readme-ov-file#usage) 

#### Code quality
- [ ] The code is executable without requiring any information from the user (under default settings)
- [ ] The method replicates the sample output using sample input in the Git Repository 
- [ ] Parameters, decisions used in the code are read from a separate file e.g., `config.json` that the user can easily update without interacting with the code 
- [ ] The method is reproducible using only publicly available resources i.e., not using any commercial tools, packages, APIs etc. 
- [ ] The code is structured into modules (if need be) and is sufficiently commented to facilitate modification

For more details on documentation and code quality, check the [Method Quality Guidelines](https://github.com/GESIS-Methods-Hub/guidelines-for-methods/blob/main/method-submission-guidelines.md#5-method-quality-guidelines) section of the guidelines.

## Contact

Methods Hub Team &lt;[methodshub@gesis.org][methodshub-email]&gt;

[methodshub-email]: mailto:methodshub@gesis.org
