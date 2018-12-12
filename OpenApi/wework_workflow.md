# WeWork Open API Specification Workflow
Phil Sturgeon: Software engineer at WeWork
- Design-first API specification

## Intro
Satellite crashed because of imperial unit vs metric.
Unit was not specified.x

> Don't write documentation, write API specificaitons

## Advantages from API specifications
- Code generation for both sides

## A lot of specificaiton languages
- HAR
- JSON Schema
- RAML
- OpenAPI

## Workflow requirements
* Have one source of througth
* 

> Don't blame REST for unspecified JSON APIs

## Specification
- Documentation
- Contract testing
- validation on both sides
- client library generation


## Documentation
Don't use Swagger, use Redoc.
Swagger is just RPC

Devs don't like to write docs.

## Contract testing

## What is design first?
### Planning
Write specs before code

- feedback from client
- implement feedback without writing code

When agreed, copy OpenAPI into ticketing system

### no specs but already api
#### One-off
- traffic sniffers: swagger inspector
- static data: jsonschema.net
- postman export (apimatic transformer)
- code (not recommended, annotation based): swagger generate

### open api guis
- stoplight.io
- apicurio (good for creating specs)

### ide/editor plugins
- atom
- vscode
- eclipse
- jetbrains suite

## Linting
- speccy

Add it to continious integration

## Contract testing
- avoid contract duplication, dont' add them to your tests
like: `this should do this`

Json schema has tests
slight differences between openapi and json schema

> Use json schema for models, openapi for api

## Mock
- prism (v3 comign oson)
- ohter...

hosted:

- stoplight.io
- restpoint.io
- getsandbox.com
- postman mock server

## SDK generator
see github projects

- openapi generator (openapitools)
- openapi3 generator (fmvilas)

## Postman collections
- Apimatic transformer
- push via postman pro api
- new endpoints, improved examples, appear in Postman GUI

## Documenation
- use Redoc

## E2E testing
- RSpec + faraday +  openapi validation service (ajv based)

## Json schema client validation
- emake it availabel to browser (Link html tag)


Json Hyperschame for HATEOAS vin your api

> Stoplight can help you with this workflow

## book:
surviving other peoples apis