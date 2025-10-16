# swim-avimet-api
Provisional repo for an OGC API specification for SWIM aviation weather messages

## Building

The standard document is automatically built with Metanorma when changes are pushed into the ```main``` branch.

The document can be generated locally using the Metanorma CLI Docker container:

```docker run -v "$(pwd)":/metanorma/ -w /metanorma metanorma/metanorma metanorma compile --agree-to-terms -t ogc -x xml,html,doc -o doc document.adoc```

