# JSON Schemas of October CMS config files

## Form fields `fields.yaml`
> The form fields configuration is used for creating backend forms
  
**fields.yaml schema URL**:  
```
https://raw.githubusercontent.com/inetis-ch/october-schemas/master/fields.json
```
[October CMS documentation](https://octobercms.com/docs/backend/forms#form-fields)

## Lists columns `columns.yaml`
> The column configuration is used for creating backend record list
  
**columns.yaml schema URL**:  
```
https://raw.githubusercontent.com/inetis-ch/october-schemas/master/columns.json
```
[October CMS documentation](https://octobercms.com/docs/backend/lists#list-columns)

## List config `config_list.yaml`
> The list configuration is used for creating backend record list

**config_list.yaml schema URL**:
```
https://raw.githubusercontent.com/inetis-ch/october-schemas/master/config_list.json
```
[October CMS documentation](https://docs.octobercms.com/3.x/extend/lists/list-controller.html)

---

## Setup your IDE for autocomplete

### PhpStorm

Open Settings/Preferences dialog, go to Languages & Frameworks | Schemas and DTDs | JSON Schema Mappings.   
Add new json schema and specify :
 - a name (what you want)
 - the URL (see above),
 - schema version 7  
 
add mapping "file path pattern" and set the file name (e.g. fields.yaml)

[Documentation](https://www.jetbrains.com/help/phpstorm/yaml.html#remote_json)

### Visual Studio Code

- Install [YAML extension by Red Hat](https://marketplace.visualstudio.com/items?itemName=redhat.vscode-yaml)
- Open your `settings.json` file and add following:
```json
{
    "yaml.schemas": {
        "https://raw.githubusercontent.com/inetis-ch/october-schemas/master/fields.json": [
            "fields.yaml"
        ],
        "https://raw.githubusercontent.com/inetis-ch/october-schemas/master/columns.json": [
            "columns.yaml"
        ]
    }
}
```
