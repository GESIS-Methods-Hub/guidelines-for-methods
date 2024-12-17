## Input/Output Specification
### User Query (if applicable): 
This refers to the information the user provides to personalize or refine the process (e.g., a query for semantic search or a seed topic for topic modeling).
Example: "User inputs a search query to identify similar social media posts."
### Input Dataset/Corpus (if applicable): 
This refers to the dataset or text corpus the method operates on.
Example: "The method processes a collection of social media posts in JSON format."

### Output:
Providing a sample output on the sample input to help cross check.
Example: "The output is a ranked list of posts saved in a JSON file, including the similarity score for each match."
For methods without ranked results, describe what the user can expect.
Example: "The output consists of topic distributions and representative words for each topic."

## How to Use
- Providing HowTos on the method for different types of usages
- Describe how the method should be used, including installation, configuration, and any specific instructions for users.
- *Following these steps should be sufficient to execute the method for sample input. Any one with non-technical background should be able to follow these steps.*
- For reproducibility, preserve the original working environment, set random seed control and provide configurations in a JSON file

## Repo Structure
- Explain the overall structure of the method, including directories, key files, and their functions.
For example,
The tool's architecture includes a src/ directory for core scripts, with requester.py handling data collection, board.py managing board-specific requests, and utils.py for auxiliary functions. Data is stored in a data/ directory created upon initiation, and documentation is available in docs/.

## Hardware Requirements (Optional)
- The hardware requirements may be needed in specific cases when a method is known to require more memory/compute power. 
- The method need to be executed on a specific architecture (GPUs, Hadoop cluster etc.)
- *Remove this section if it doesn't apply to your method otherwise remove the (optional) from the title* 
