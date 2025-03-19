# Methods Hub's Guidelines for Methods

Here you will find the guidelines used by Methods Hub for methods. If you are preparing a tutorial, check the [guidelines used by Methods Hub for tutorials](https://github.com/GESIS-Methods-Hub/guidelines-for-tutorials).

## Accepted formats

| Format | Notes |
| --- | --- |
| Python Package | |
| R package | |
| Jupyter Notebook | |

## To publish your method
- Fulfill the checklist requirements [Method checklist](https://github.com/GESIS-Methods-Hub/guidelines-for-methods/blob/main/method-checklist.md)
- The method README must be in template [Method README template](https://github.com/GESIS-Methods-Hub/guidelines-for-methods/blob/main/method-README-template.md)

## Required Files

The Git repository with the method **must** have the following files

- [`README.*`](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-readmes)
- [`LICENSE.*`](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/licensing-a-repository)
- [`CITATION.cff`](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-citation-files)

Additionally, the Git repository **must** also have the [necessary files for setting up a binder environment](https://mybinder.readthedocs.io/en/latest/using/config_files.html)[^1]. For example,

- `binder/postBuild` from [postBuild](https://methodshub.gesis.org/snippet/postBuild)
- `binder/environment.yml`

Optional,  
- Verify rendering through Methods Hub, using [Methods Hub preview as GitHub Action](https://github.com/GESIS-Methods-Hub/preview?tab=readme-ov-file#usage) *(Update the branch name as per your repository)*

## Further Reading
- For more on Methods, visit [Methods guide](method-submission-guidelines.md)


[^1]: That environment will be used for rendering the tutorial and for the interactive execution.
