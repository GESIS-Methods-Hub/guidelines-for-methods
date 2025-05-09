# README Template: Specification and Illustration of the Methods Hub Friendly README
<!--
General specifications:
- This specification of the Methods Hub friendly README often uses the word 'should' to indicate the usual case. If you feel you need to do it differently, add a comment to argue for your case when you submit your method.
- A Methods Hub friendly README should contain all sections below that are not marked as optional, and can contain more sections.
- A Methods Hub friendly README should contain as few technical terms as possible and explain (or link to an explanation of) all used technical terms.
- A Methods Hub friendly README should link to all code files that it mentions using the [text](URL relative to this file) format. The relative URL (i.e., no "https://github.com") is neccessary for proper versioning in Methods Hub.
- A Methods Hub friendly README should contain an explanation (in the text) and an alternative for each image it contains (e.g., data models, pipeline, schema structure). Format: ![alternative text that describes what is visible in the image](URL relative to this file).
- A Methods Hub friendly README should link to authoritative sources rather than containing a copy of the information (e.g., documentation).
- A Methods Hub friendly README should use a uniform citation style for all references, for example APA7 https://apastyle.apa.org/style-grammar-guidelines/references/examples

Title:
1. The title must be the README's only first-level heading (line starting with a single '#').
2. The title should make the method's purpose clear.
3. The title (line 1 of this file) must be changed by you, but all other headings should be kept as they are.

Section templates:
The README template comes with text templates for each section (after each comment) that can be used, customized or removed as desired.
-->

## Description
<!--
1. Provide a brief and exact description of the method clearly mentioning its purpose i.e., what the method does or aims to achieve in abstract terms (avoiding technical details).
2. The focus should be on explaining the method in a way that helps users with different levels of expertise understand what it does, without going into technical details. It should clearly describe what inputs are needed and what outputs can be expected.
3. Briefly explain the input and output of the method and its note worthy features.
4. Provide link(s) to related papers from the social science domain using the method or similar methods for solving social science research questions. 
5. In a separate paragraph, highlight the reproducibility aspect of the method providing details or references to the resources used by the method, the data used in building the pre-trained modules etc.
6. It should also discuss the decisions and parameters controlling the behavior of the method.
-->
METHOD allows to do XXX.

METHOD takes XXX in XXX format as input and provides XXX in XXX format as output.
Alternatively, METHOD can also be configured to XXX.
METHOD works with XXX data.
METHOD can use any [XXX-compatible API](https://example.com).
The output of METHOD is compatible with [XXX](https://example.com).

METHOD placed Xth in the [XXX](https:/example.com) competition on XXX.
METHOD is much faster than other methods.
METHOD runs quickly on standard hardware.
METHOD requires a GPU.

## Use Cases
<!--
1. The use cases section should contain a list of use cases relevant to the social sciences.
2. Each use case should start with a description of a person, continues with a description of a task the person has, and then details how the person uses the method to assist in the task.
3. Each use case may list publications in which the use case occurs (e.g., in APA7 style, https://apastyle.apa.org/style-grammar-guidelines/references/examples).
-->
- A XXX wants to do XXX. Their situation is that XXX. They use METHOD by doing XXX to do XXX, which solves their original problem because XXX.

  Example publications that illustrate this use case:

  - XXX.
  - XXX.

## Input Data
<!--
1. The input data section should illustrate the input data format by showing a (possibly abbreviated) example item and explaining (or linking to an explanation of) the data fields.
2. The input data section should specify which parts of the input data are optional and what effect it has to not provide these.
3. The input data section should link to a small example input file in the same repository that can be used to test the method (this test should be described in the section "How to Use").
-->
METHOD takes as input XXX in [XXX format](https://example.com) and XXX in [XXX format](https://example.com).

Example input data XXX (excerpt of [example-input-file1.json](example-input-file1.json)):

```{json}
{
  "key": [
    "value [...]"
  ],
  "key": "value"
}
```

- `key`. A list of XXX. If missing or empty, then XXX.
- `key`. XXX. One of XXX, XXX, or XXX. If missing, then XXX.
- `key`. XXX. A number between XXX and XXX. If missing, then XXX.
- `key`. XXX. Required.

Example input data XXX (one line of [example-input-file2.ndjson](example-input-file2.ndjson), formatted for readability):

```{json}
{
  "key": [
    "value [...]"
  ]
}
```

- `key`. XXX.

## Output Data
<!--
1. The output data section should illustrate the output data format by showing a (possibly abbreviated) example item and explaining (or linking to an explanation of) the data fields.
2. The output data section should link to a small example output file in the same repository that can be re-created (as far as the method is non-random) from the input data (as described in the section "How to Use").
-->
METHOD produces XXX in [XXX format](https://example.com).
The README template produces a README according to the [Methods Hub friendly README specification](https://github.com/GESIS-Methods-Hub/guidelines-for-methods/blob/main/README-template.md?plain=1).

Example output data (excerpt of [example-output-file.csv](example-output-file.csv)):

```{csv}
header 1,header 2
value 1-1,value 1-2
value 2-1,value 2-2
```

## Hardware Requirements
<!--
1. The hardware requirements section should list all requirements (storage, memory, compute, GPUs, cluster software, ...) that exceed the capabilities of a cheap virtual machine provided by cloud computing company (2 x86 CPU core, 4 GB RAM, 40GB HDD).
2. If the method requires a GPU, the hardware requirements section must list the minimal GPU requirements (especially VRAM).
-->
METHOD runs on a cheap virtual machine provided by cloud computing company (2 x86 CPU core, 4 GB RAM, 40GB HDD).
METHOD requires a GPU (compute capability XXX, XXX GB VRAM) to run.

## Environment Setup
<!--
1. The environment setup section should list all requirements and provide all further steps to prepare an environment for running the method (installing requirements, downloading files, creating directoriees, etc.).
2. The environment setup section should recommend to use a virtual environment or similar if the programming language supports one.
-->
METHOD requires at least XXX version XXX.
To avoid problems with your system's Python installation, create and activate a [virtual environment](https://docs.python.org/3/library/venv.html).

METHOD requires an XXX API key. Get one [here](https:/example.com/) and paste it into [example-key-file.txt](example-key-file.txt).
METHOD requires XXX in directory XXX. Download it from [here](https:/example.com/).

Then install all requirements using:

```{bash}
pip install -r requirements.txt
```

Then install METHOD in R using:

```{R}
install.packages("METHOD")
```

## How to Use
<!--
1. The how to use section should provide the list of steps that are necessary to produce the example output file (see section Output Data) after having set up the environment (see section Environment Setup).
2. The how to use section should explain how to customize the steps to one's own needs, usually through configuration files or command line parameters, or refer to the appropriate open documentation.
-->
To apply METHOD to the [example input](#input-data) and generate the [example output](#output-data), proceed as follows:

```{bash}
python method.py example-input-file1.json example-input-file2.ndjson
```

To adapt these steps to your needs, see the [online documentation of METHOD](https://example.com).

To adapt these steps to your needs, see the output of `python method.py --help`.

To adapt these steps to your needs, adapt the [configuration file](example-configuration-file.conf):

- `xxx`: Controls XXX. (default: "XXX")

To adapt these steps to your needs, apply the following command line parameters:

- `--xxx`: Controls XXX. (default: "XXX")

To adapt these steps to your needs, adapt the [configuration file](example-configuration-file.conf) or apply the following command line parameters (overwriting respective settings in the configuration file):

- `--xxx`: Controls XXX. (default: "XXX")

## Technical Details
<!--
1. The technical details section should proview a process overview, linking to key source code files at every step of the process.
2. In case a publication provides the details mentioned below, the technical details section should link to this publication using a sentence like "See the [publication](url-of-publication-best-using-doi) for ...". In this case, the mentioned technical details can be omitted from the section.
3. The technical details section should list all information needed to reproduce the method, including employed other methods and selected parameters.
4. The input data section should link to external data it uses, preferably using a DOI to a dataset page or to API documentation.
5. The technical details section should mention how other methods and their parameters were selected and which alternatives were tried.
6. The technical details section should for employed machine learning models mention on what kind of data they were trained.
-->

METHOD does XXX by performing the following steps:

1. Reading. The data is read from the input file (`--input-file`) and converted into XXX. (see [method-package/example-source-file.py](method-package/example-source-file.py))
2. Downloading data. XXX data is fetched from [XXX](https:/example.com/).
3. XXX. To do XXX, the method uses [XXX](https:/example.com/) with XXX set to XXX (change using `--xxx` or setting `xxx` in the [configuration file](example.conf)). (see [method-package/example-source-file.py](method-package/example-source-file.py))
4. Writing. The result is written to the output file (`--output-file`). (see [method-package/example-source-file.py](method-package/example-source-file.py))

See the [publication](https:/example.com/) for tested and selected models and parameters, the reasoning behind the model selection, and employed datasets for training.

## References
<!--
1. The references section is optional, especially if they are cited in a publication that explains the technical details (see section Technical Details).
2. The references section should provide references of publications related to this method (e.g., in APA7 style, https://apastyle.apa.org/style-grammar-guidelines/references/examples).
-->
- Dataset used for training:
  
  XXX.

- Employed model:
  
  XXX.

- Underlying infrastructure:
  
  XXX.

## Acknowledgements
<!--
1. The acknowledgments section is optional.
2. The acknowledgments section should list expressions of gratitude to people or organizations who contributed, supported or guided.
-->
Special thanks to the creators of [XXX](https://example.com) for providing XXX.
Special thanks to [XXX](https://example.com) for XXX.

## Disclaimer
<!--
1. The disclaimer section is optional.
2. The disclaimer section should list disclaimers, legal notices, or usage restrictions for the method.
-->
METHOD is intended for academic research, and users are responsible for ensuring the legality and ethicality of their data use.
Ensure you follow the [XXX Terms of Service](https://example.com) when using this method.

## Contact Details
<!-- 
1. The contact details section should specify whom to contact for questions or contributions and how (can be separate entitites; for example email addresses or links to the GitHub issue board).
-->
In case of questions, contact [XXX](mailto:XXX).
For contributions and bug reports, open an issue at [XXX](https://example.com).
