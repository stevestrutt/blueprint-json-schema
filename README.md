# JSON Schema for Schematics Blueprints

Initial JSON Schema for template validation in VSCode using Redhat YAML extension. 

Basic validation of all required fields in Schema. 

To use schema directly from github add the `modeline`

`# yaml-language-server: $schema=https://raw.githubusercontent.com/stevestrutt/blueprint-json-schema/master/schema.json`

Alternatively download schema.json to the local filesystem. Filepath is relative to the currently active VSCode workspace. The following will locate the schema in the same directory as   

`# yaml-language-server: $schema=../schema.json`

Example templates can be found in the /templates folder


## Initial release
- All blueprint template keywords defined for Schema V1.0
- No conditional evaluation of sub-schemas, e.g. source_type > github/catalog broken at release 1.3 of YAML extension. 


