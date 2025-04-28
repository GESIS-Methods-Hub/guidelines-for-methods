# README Template: Specification and Illustration of the Methods Hub Friendly README
<!--
General specifications:
- This specification of the Methods Hub friendly README often uses the word 'should' to indicate the usual case. If you feel you need to do it differently, add a comment to argue for your case when you submit your method.
- A Methods Hub friendly README should contain all sections below that are not marked as optional, and can contain more sections.
- A Methods Hub friendly README should contain as few technical terms as possible and explain (or link to an explanation of) all used technical terms.
- A Methods Hub friendly README should link to all code files that it mentions using the [text](URL) format.
- A Methods Hub friendly README should contain an explanation for each image it contains (e.g., data models, pipeline, schema structure).
- A Methods Hub friendly README should link to authoritative sources rather than containing a copy of the information (e.g., documentation).
- A Methods Hub friendly README should use a uniform citation style for all references, for example APA7 https://apastyle.apa.org/style-grammar-guidelines/references/examples

The title:
1. The title must be the README's only first-level heading (line starting with a single '#').
2. The title should make the method's purpose clear.
3. The title (line 1 of this file) must be changed by you, but all other headings should be kept as they are.
-->

## Description
<!--
1. The description should make the method's purpose clear (extending on the title).
2. The description should specify both input and output of the method (examples and details should be in the respective sections).
3. The description should mention different ways of using the method and important parameters if they exist (details should be in the section `How to Use`).
4. The description should mention what makes the method special (details, including how a model was trained, should be in the section 'Technical Details').
-->
The README template illustrates the Methods Hub friendly README. Though the README template is not a method, this document is written as if it were one for the sake of illustration.

The method takes as input the source code repository of another method (has to be applicable for social science research) and the knowledge of their programmer. It provides as output a Methods Hub friendly README that describes that other method in a unified and easily accessible way. Alternatively, it allows to check whether a README is Methods Hub friendly using the [specification](https://github.com/GESIS-Methods-Hub/guidelines-for-methods/blob/main/README-template.md?plain=1) (in `<!-- comment -->`s), as it is done after submitting a method to the Methods Hub. The method can use any OpenAI-compatible API (ChatGPT, Ollama, ...). The method placed 2nd in [NO competition](https:/example.com/). It has extremely low hardware requirements.

## Technical Details
<!--
1. In case a publication provides the details mentioned below, the technical details section should link to this publication using a sentence like "See the [publication](url-of-publication-best-using-doi) for ...". In this case, the technical details can be omitted.
2. The technical details section should list all information needed to reproduce the method, including a process overview, employed other methods, and selected parameters.
3. The technical details section should mention how other methods and their parameters were selected and which alternatives were tried.
4. The technical details section should for employed machine learning models mention on what kind of data they were trained.
-->
The README template uses [markdown](https://daringfireball.net/projects/markdown/syntax) to present a structured overview of a method and mark links. It takes the following steps:

1. Copying. This document is copied into the repository of the method to be submitted. This step uses the pre-trained [best practices model](https:/example.com/) that was fine-tuned on the [responses](https:/example.com/) from an online survey with XXX participants as well as expert interviews with PyTorch [thresholded frequency optimizer](https:/example.com/) and a learning rate of 0.1 based on results from our preliminary tests (we tested learning rates 0.0001, 0.001, 0.01, 0.1, and 1). The learning rate can be changed using the `--learning-rate` command line parameter.
2. Adapting. The template is then adapted so that it fits to the method of the repository. In our experiments we used [VIM](https://xkcd.com/378/) as a standard compromise between coolness and complexity, but the method can be configured to use any other text editor instead.
3. Submitting. The respository, including the README (from step 1) is [submitted to Methods Hub](https://methodshub.gesis.org/dashboard/methods/add/) using the system web browser (default settings, we used Firefox 137.0.2 on Windows 10).

See the [publication](https:/example.com/) for the reasoning behind the selected methods.

## Use Cases
<!--
1. The use cases section should contain a list of use cases relevant to the social sciences.
2. Each use case should start with a description of a person, continues with a description of a task the person has, and then details how the person uses the method to assist in the task.
3. Each use case may list publications (in APA7 style) in which the use case occurs.
-->
- A computational social scientist wants to have their method being featured in the Methods Hub. The method code is already contained in a repository on GitHub. They then use the README template to create a new file, `README-methods-hub.md`, by copying the content of this document into the new file and adapting it to their own method.

  Example publications that illustrate this use case:

  - Ample, E. X. & Obody, N. (2025). Getting into the Methods Hub. *Unpublished Papers*, 8(3), 42–43.

- A computational social scientist has created a README for their own script and wants to check whether the README is Methods Hub friendly to ensure it contains all necessary information. They compare their own README with the README template, adjusting their own README as necessary to match the specification provided in the template.

## Environment Setup
<!--
1. The environment setup section should list all requirements and provide all further steps to prepare an environment for running the method (installing requirements, downloading files, creating directoriees, etc.).
2. The environment setup section should recommend to use a virtual environment or similar if the programming language supports one.
-->
The README template requires an arbitrary text editor compatible with Markdown version 0.31.2. If this were an actual Python method, you should do the following. To avoid problems with your system's Python installation, create and activate a [virtual environment](https://docs.python.org/3/library/venv.html). Then install all requirements using:

```{python}
pip install -r requirements.txt
```

You do not need an API key to use the README template, but if you would need one, you would here find a link to documentation on how to get one and were to put it.

## Input Data
<!--
1. The input data section should illustrate the input data format by showing a (possibly abbreviated) example item and explaining (or linking to an explanation of) the data fields.
2. The input data section should link to a small example input file in the same repository that can be used to test the method (this test should be described in the section "How to Use").
3. The input data section should link to external data it uses, preferably using a DOI to a dataset page or to API documentation (if no such page exists, a publication can be linked).
-->
The README template takes as input information about a method, for example in [README-format](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax).

Example input data ([README-template.md](README-template.md)):

```{markdown}
# README Template: Specification and Illustration of the Methods Hub Friendly README

## Description
The README template illustrates the Methods Hub friendly README. [...]
```

## Output Data
<!--
1. The output data section should illustrate the output data format by showing a (possibly abbreviated) example item and explaining (or linking to an explanation of) the data fields.
2. The output data section should link to a small example output file in the same repository that can be re-created from the input data (as described in the section "How to Use").
-->
The README template produces a README according to the [Methods Hub friendly README specification](https://github.com/GESIS-Methods-Hub/guidelines-for-methods/blob/main/README-template.md?plain=1).

Example output data ([README-template.md](README-template.md)):

```{markdown}
# README Template: Specification and Illustration of the Methods Hub Friendly README

## Description
The README template illustrates the Methods Hub friendly README. [...]
```

## How to Use
<!--
1. The how to use section should provide the list of steps that are necessary to produce the example output file (see section Output Data) from the example input file (see section Input Data), after having set up the environment (see section Environment Setup).
2. The how to use section should explain how one can adapt the steps to one's needs, usually through configuration files or command line parameters.
-->
To prepare a method for the Methods Hub, use the README template as follows:

- Copy this document to your repository and adapt its text to your method. We recommend to name that copy as `README.md` and use it as the single method of your repository, but it is not required that your Methods Hub friendly README has this name for your method to be accepted into Methods Hub (e.g., if the `README.md` is intended for a different target audience).
- A step can also be illustrated as code, for example:

  ```{bash}
  python do-something.py README.md
  ```

- After following all steps in this list, the output file (see section Output Data) is reproduced from the input file

To adapt these steps to your needs, adapt the configuration file or use command line parameters:

The template does not use a configuration file. But if it would need one, we would here link to the file and explain how to change it to have certain effects or link to documentation that does the explanation.

- `example-option`: This is an example configuration option to illustrate how options could be described in a README. (default: "none")

The template has no command line parameters. But if it would have some, we would here explain how to use them to have certain effects, also saying when one parameter corresponds to some entry in the configuration file mentioned above. If there are many parameters and the method has a good `--help`, this text could also just detail the required parameters and then say: For more information, run `method-command --help`.

- `--example-parameter`: This is an example parameter to illustrate how parameters could be described in a README. (default: "none"; overwrites configuration option `example-option`)

## Git Repository Structure
<!--
1. The git repository structure section should describe each file and directory - excluding README, Licence, environment configuration files, gitignore, and similar - in a hierarchical list
-->
- [guidelines.md](guidelines.md): Provides details beyond the checklist in the [README.md].
- [README-template.md](README-template.md): Specifies and illustrates the Methods Hub friendly README.
- [examples](examples): Does not exist, but illustrates in this list how a directory could be shown.
  - [input.txt](examples/input.txt): Does not exist, but could be an example input to illustrate the input format of this method (see sections [Input Data](#input-data) and [How to Use](#how-to-use))
  - [output.txt](examples/output.txt): Does not exist, but could be an example output to illustrate the output of this method (generated from the [input.txt](examples/input.txt); see sections [Output Data](#output-data) and [How to Use](#how-to-use))

## Hardware Requirements
<!--
1. The hardware requirements section should list all requirements (storage, memory, compute, GPUs, cluster software, ...) that exceed the capabilities of a standard business laptop.
-->
This method can be run on a standard business laptop.

## References
<!--
1. The references section is optional.
2. The references section should provide references of publications related to this method.
-->
- To cite this method:
  
  Ample, E. X. & Obody, N. (2025). Getting into the Methods Hub. *Unpublished Papers*, 8(3), 42–43.

## Acknowledgements
<!--
1. The acknowledgments section is optional.
2. The acknowledgments section should list expressions of gratitude to people or organizations who contributed, supported or guided.
-->
Special thanks to the creators of the [Methods Hub friendly README specification](https://github.com/GESIS-Methods-Hub/guidelines-for-methods/blob/main/README-template.md?plain=1) for laying the foundation of this work.

## Disclaimer
<!--
1. The disclaimer section is optional.
2. The disclaimer section should list disclaimers, legal notices, or usage restrictions for the method.
-->
The tool is intended for academic research, and users are responsible for ensuring the legality and ethicality of their data use.

Please ensure you follow the [GitHub Terms of Service](https://docs.github.com/en/site-policy/github-terms/github-terms-of-service) when using this method.

## Contact Details
<!-- 
1. The contact details section should specify whom to contact for questions or contributions and how (can be separate entitites; for example email addresses or links to the GitHub issue board).
-->
For questions, contributions and bug reports, contact [the Methods Hub team](mailto:methodshub@gesis.org).
