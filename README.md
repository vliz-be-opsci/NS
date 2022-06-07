# NS

This `namespace` project «NS» creates a formal base URL for various ontologies introduced in various projects of the [VLIZ-OpenScience Team](https://github.com/vliz-be-opsci)


## Contents

Currently the following ontologies are available:

| link                                 | usage & purpose                                        |
|--------------------------------------|--------------------------------------------------------|
| (dmbon-assistant)[./dmbon-assistant] | Predicates and classes interpreted by the (dmbon-assistant project)[https://github.com/vliz-be-opsci/dmbon-assistant]


## Adding ontologies

* Simply provide an extra relative ./*ttl file describing the namespaced terms, predicates and or classes it is composed of.
* Note that inside the source ttl you can use specific placeholders to be replaced dynamically.
* Add a reference to it in the table above for reference
* Push to github, thus triggering the action to publish
* Check for the result on {{baseurl}}

## Dynamic placeholders

| placeholder   | replaced by                                                                       |
|--------------:|-----------------------------------------------------------------------------------|   
| `{{baseurl}}` | the URL of this 'NS' space resp.                                                  |
| `{{self}}`    | the name of this ontology file                                                    |


## Automated publishing

The actual publishing (conversion to html) of this content is orchestrated through the github action «pylode-to-pages»
See (https://vliz-be-opsci/pylode-to-pages) for more details on how to achieve the same for you namespaced ontologies
