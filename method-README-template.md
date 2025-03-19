# Method Title
1. The title should be meaningful and easy to follow.
2. It should reflect relevance to social science, if applicable 

## Description
1. Provide a brief and exact description of the method clearly mentioning its purpose i.e., what the method does or aims to achieve in abstract terms (avoiding technical details).
2. Focus should be to emphasize on the functionality as a blackbox, helping researchers with different levels of expertise and experience to understand what the method is doing.
3. Brielfly explain the input and output of the method and its note worthy features.
4. Provide link(s) to related papers from the social science domain using the method or similar methods for solving social science research questions. 
5. In a separate paragrpah, highlight the reproducibility aspect of the method providing details or references to the resources used by the method, the data used in building the pre-trained modules etc.
6. It should also provide different configuration parameters to assist in altering the behavior of the method for a related use case. 


## Keywords
- Keyword 1 (3 to 5 keywords highlighting the purpose of method)
- Keyword 2
- Keyword 3   

## Social Science Use Case(s)
1. Include use case(s) or research question(s) from social sciences that would make this method applicable in a certain scenario.
2. They should arise from the latest social science literature cited in the description. 

## Git Repository Structure
1. List files and their purpose as a tree-like structure.
2. Explain the script files and their purpose.
3. Explain the input, output and other intermediate files produced.
4. Explain the configuration and other utility files.

## Environment Setup
1. Provide configuration files preserving dependencies i.e., Requirements.txt, install.R, configuration.yml etc (including specific versions).
2. Provide steps/commands to install all dependencies required to run this method.
3. Load default configurations to execute the method without needing user envolvement e.g., for input or paths to resources. Store the configuration files separately (e.g., in config.json) where the users can change the paramters to alter the behavior of the method without directly interacting with the code.

## Input Data
1. Explain the input data using sample instances as input data in the Git Repository i.e., the features and what they represent. These may be generated samples, staying within data restrictions.
2. Provide links to the actual dataset that the method can work with, idealy [GESIS DBD data](https://www.gesis.org/en/institute/digital-behavioral-data).

## Output Data
1. Explain the sample output data in the Git Repository i.e., how to interpret the output.

## How to Use
1. Provide list of steps to execute the method for its intended purpose (assuming the environment is deployed).
2. Explain which files or paramters need to be updated and how to alter the behavior of the method.

## Hardware Requirements (Optional)
1. The hardware requirements may be needed in specific cases when a method is known to require more memory/compute power. 
2. The method need to be executed on a specific architecture (GPUs, Hadoop cluster etc.)

## Method Publication (Optional)
1. Include information on publications or articles associated to the method, if applicable.
2. Format your publication citation using APA style.

## References (Optional)
1. Include references to explore and learn more about the method, if applicable.
2. Format your references list using APA style.

## Contact Details
1. Provide contact information, having at least name and email address.
2. Those interested in the method may use this information to reach out with questions/feedback.

## Acknowledgements (if any)
1. Acknowledgements if any

## Disclaimer (Optional)
1. Add any disclaimers, legal notices, or usage restrictions for the method, if necessary.

## Help
1. Remove optional sections that don't apply to your method.
2. Remove "(Optional)" or "(if any)" from the section headings that apply to your method.
3. Some good examples for Python methods are [4TCT: A 4chan Text Collection Tool](https://methodshub.gesis.org/method/4TCT/), [Discovering Themes in Text with Topic Modeling (Latent Dirichlet Allocation)](https://methodshub.gesis.org/method/latent_dirichlet_allocation/) and for R methods [oolong](https://methodshub.gesis.org/method/oolong/)
4. Remove this section as well from the final version.
