# How Dutch governemnt is using Open API V3 as source of truth
Dimitri van Hees - Co Founder, Apiwise

## Introduction
Government applieds Environmental Act. "Can I build a shed in my backyard?" (ETA 2020)

One of the biggest IT challenges of the Dutch Government
We can't centralize legislation, but we can centralize the way the gov apis work.

## The projection problem
Coordinate Reference System

- Netherlands: RD
- Europe: ETRS89
- Global: WGS84 -> used by mobile phones (not precise)
- GeoJSON dropped 'projection' 

### CRS Negotiation
Own specification, because there is no standard yet.

## Describe apis
- Available tools
- sharing knowledge
- sharing templates
- sharing examples
- own tools
- EU: WCAG 2.0

Solution: Let's use OpenAPI 3.X spec

## Apply to add to standards in Netherlands
- paperwork
-  expert lobbying
- expert reviews
- expert exampination
- public reviews
- etc.

=> National API Strategy :yaay:

## Move to Github, Markdown, JsDelivr, etc
- API in markdown
- Collabs
- Versioning
- Forks for different usecases
- Reusable OAS3 componetns

## Federated OAS
=> possible to coorperate with EU for OAS?


## Switch to English
-> Governemnt issue should be in Dutch, but this is not open.

## Reference duplicaiton in OAS
- use relative urls
- OAS generation to avoid typos

## Future
- Reusable JSON Schemas



## Challenges

### Open API first
openapi.yml -> extensions -> internal endpoint -> openapi.yml
... etc

### Different enpoints
- Absolute URI
- mocking/example
- versioning

### OpenAPI specific challenges
- JSON scheme vs openApi
- reusablility: traits?
- extendablility: overlays?
- examples: runtime expressions?

