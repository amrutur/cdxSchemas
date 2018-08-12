Schemas and Examples for City Data Exchange (CDX) Platform
------------------------------------------------------------

All schemas are based on json schema as defined in: http://json-schema.org
Schema validation as per: https://www.jsonschemavalidator.net/

schemas/cdxSchemaForThings.json : Schema for describing things in the cdx platform.
Any thing's schema will get validated against this schema. As an example:
examples/exampleThing.json is validated against this schema.

schemas/cdxSchemaForMessageSchema.json : schema for describing message schemas
for messages to/from things. This schema is included in cdxSchemaForThings.json. 

schemas/cdxSchemaForOtherInfo.json: schema for describing other information of things. This is included in cdxSchemsForThings.json.

All schemas in the schemas/ folder will be managed and updated by the cdx platform developers

examples/exampleMessageSchema.json: An example message schema which describes the template of messages from a thing. This is validates against cdxSchemaForMessageSchema.json

examples/exampleMessage.json: An example message from a thing. This is validated against the exampleMessageSchema.json

examples/exampleOtherInfo.json: An example of other info portion of a thing. This is validated against schemas/cdxSchemaForOtherInfo.json



