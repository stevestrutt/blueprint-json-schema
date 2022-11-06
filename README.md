# VSCode language support for IBM Cloud Schematics blueprint templates 

Enable blueprint template editing and validation in VSCode using the Redhat YAML language server extension and blueprint JSON-Schema. 
- YAML language support with blueprint schema validation
  - Validation of YAML structure and blueprint key words 
- Autocomplete
  - Auto complete for template key words
- Hover support
  - Hovering over a node shows blueprint schema description


<br/>

## 1. Install the Red Hat YAML Language extension 



https://marketplace.visualstudio.com/items?itemName=redhat.vscode-yaml




Click on the “Extensions” button in the Activity Bar. It’s located on the side of VS Code’s client. Alternatively, you can use the keyboard shortcut “Ctrl+Shift+X” or "Cmd+Shift+X" on MacOS to open the “Extensions” screen.

This will bring you to the “Extensions” list. Type YAML in the search box and this will sort the available YAML extensions with the Red Hat extension at the top. 

![yamlextension](images/YAMLextension.png)


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


