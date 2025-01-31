# Methods Hub's Guidelines for Methods

Here you will find the guidelines used by Methods Hub for methods.
If you are preparing a tutorial,
check the [guidelines used by Methods Hub for tutorials](https://github.com/GESIS-Methods-Hub/guidelines-for-tutorials).

## Accepted formats

| Format | Notes |
| --- | --- |
| Python Package | |
| R package | |
| Jupyter Notebook | |

## Required Files

The Git repository with the method **must** have the following files

- [`README.*`](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-readmes)
- [`LICENSE.*`](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/licensing-a-repository)
- [`CITATION.cff`](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-citation-files)

Additionally, the Git repository **must** also have the [necessary files for the interactive environment](https://repo2docker.readthedocs.io/en/latest/configuration/index.html). For example,

- `binder/postBuild`
- `binder/environment.yml`

## Template

A template is provided at [`method-README-template.md`](method-README-template.md).

## Further Reading

- [Method Submission Guide](method-submission-guidelines.md)