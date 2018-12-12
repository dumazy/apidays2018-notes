# Keep your specs close to your code
Gregory Koberger - CEO at ReadMe

## Introduction
an intro to the `$ oas` CLI tool and two other tools

- oas
- swagger-inline
- openap.is

### Ways to thing about OAs
- Design
- Documentation

## OAS
install with `npm install oas -g`

### commands

#### oas init
Create base OAS file:

- name api
- version
- license
- base url
- json, yaml...


#### oas endpoint
Write endpoints and use code generation for paths.
Never gets out of date.

Commands gives temlplate code, copy paste into endpoint code.

#### oas generate
Creates final.json file with the enpoints from comments at code

#### oas host
Will generate and validate, and eventually host it on openap.is

#### Using readme
`rdme swagger swagger.json`

Has generated code snippets for multiple languages.

