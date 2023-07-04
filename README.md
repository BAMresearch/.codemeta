# BAM CodeMeta Guidelines

We use [CodeMeta](https://github.com/codemeta/codemeta) to provide standardized metadata for our repositories. 

CodeMeta is a minimal metadata schema in JSON-LD format for the description of scientific software. CodeMeta enables the standardized exchange of software metadata across repositories and organizations, thereby improving the integration of code and scientific software into the scholarly workflow.

The CodeMeta vocabulary is a subset of [schema.org](https://schema.org/), a structured vocabulary that is widely used to provide search engines with standardized information about the content of websites.
CodeMeta also provides several [crosswalks](https://codemeta.github.io/crosswalk/) for mapping its metadata schema to other metadata standards/vocabularies, e.g., from DataCite, GitHub API, Pythons disutils, and R packages.

A new CodeMeta compliant metadata file can easily be created with the [CodeMeta Generator](https://codemeta.github.io/codemeta-generator/) or manually by following the [CodeMeta specification](https://codemeta.github.io/user-guide/). A list of all properties provided by the current CodeMeta context file can be found [here](https://codemeta.github.io/terms/).

By convention, you should name your CodeMeta file `codemeta.json` and put it at the root of your Github repository.
