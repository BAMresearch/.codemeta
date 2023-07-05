# BAM CodeMeta Guidelines

We use [CodeMeta](https://github.com/codemeta/codemeta) to provide standardized metadata for our repositories. 

CodeMeta is a minimal metadata schema in JSON-LD format for the description of scientific software. CodeMeta enables the standardized exchange of software metadata across repositories and organizations, thereby improving the integration of code and scientific software into the scholarly workflow.

The CodeMeta vocabulary is a subset of [schema.org](https://schema.org/), a structured vocabulary that is widely used to provide search engines with standardized information about the content of websites.
CodeMeta also provides several [crosswalks](https://codemeta.github.io/crosswalk/) for mapping its metadata schema to other metadata standards/vocabularies, e.g., from DataCite, GitHub API, Pythons disutils, and R packages.

By convention, you should name your CodeMeta file `codemeta.json` and put it at the root of your Github repository.

**A new CodeMeta compliant metadata file can easily be created with the [CodeMeta Generator](https://codemeta.github.io/codemeta-generator/)** or manually by following the [CodeMeta specification](https://codemeta.github.io/user-guide/). A list of all properties provided by the current CodeMeta context file can be found [here](https://codemeta.github.io/terms/).

The following table includes the minimal set of CodeMeta properties that should be used to describe code projects at BAM:

| Metadata property       | CodeMeta property         | Type                       | Description                                                                                                                                                 |
|-------------------------|---------------------------|----------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Name                    | name                      | Text                       | Name of the software.                                                                                                                                       |
| Description             | description               | Text                       | A description of the software.                                                                                                                              |
| License(s)              | license                   | CreativeWork or URL        | A license document that applies to the software, typically indicated by URL (e.g., from https://spdx.org/licenses/).                                        |
| Application category    | applicationCategory       | Text or URL                | Type of software application.                                                                                                                               |
| Programming language    | programmingLanguage       | ComputerLanguage   or Text | The computer programming language.                                                                                                                          |
| Code repository         | codeRepository            | URL                        | Link to the repository where the un-compiled, human readable code and related code is located (SVN, GitHub, CodePlex, institutional GitLab instance, etc.). |
| Download URL            | downloadUrl               | URL                        | If the file can be downloaded, URL to download the binary.                                                                                                  |
| Author                  | author                    | Organization or Person     | Author of the software.                                                                                                                                     |
| Author given name       | author: givenName         | Text                       | Given/first name of the author.                                                                                                                             |
| Author family name      | author: familyName        | Text                       | Family name of the author.                                                                                                                                  |
| Author e-mail address   | author: email             | Text                       | E-mail address of the author                                                                                                                                |
| Author affiliation      | author: affiliation       | Organization               | An organization that the author is affiliated with.                                                                                                         |
| Author affiliation name | author: affiliation: name | Text                       | Name of the organization that the author is affiliated with.     
