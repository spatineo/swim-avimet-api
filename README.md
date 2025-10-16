# swim-avimet-api
Provisional repo for an OGC API specification for SWIM aviation weather messages

## Content

This repository contains the content for an OGC standard.

* `document.adoc` - the main standard document with references to all sections
* remaining ``adoc``s - each section of the standard document is in a separate document: follow directions in each document to populate
* `figures` - figures go here
* `images` - Image files for graphics go here. Image files for figures go in the `figures` directory. Only place in here images not used in figures (e.g., as parts of tables, as logos, etc.)
* `requirements` - directory for requirements and requirement classes to be referenced in `clause_7_normative_text.adoc`
* `code` - sample code to accompany the standard, if desired
* `abstract_tests` - the Abstract Test Suite comprising one test for every requirement, optional
* `UML` - UML diagrams, if applicable


## Building

The standard document is automatically built with Metanorma when changes are pushed into the ```main``` branch.

The document can be generated locally using the Metanorma CLI Docker container:

```docker run -v "$(pwd)":/metanorma/ -w /metanorma metanorma/metanorma metanorma compile --agree-to-terms -t ogc -x xml,html,doc -o doc document.adoc```

