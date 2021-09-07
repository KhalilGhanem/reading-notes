# GraphQL @connectio

Add relationships between types

## @connection

The @connection directive enables us to specify relationships between @model types. this supports one-to-one, one-to-many, and many-to-one relationships.

We can implement many-to-many relationships using two one-to-many connections and a joining @model type.

## Definition

`directive @connection(keyName: String, fields: [String!]) on FIELD_DEFINITION`

## Usage

Relationships between types are specified by annotating `fields` on an `@model` object type with the @connection directive.

* The `fields` argument can be provided and indicates which fields can be queried by to get connected objects.
* The `keyName` argument can optionally be used to specify the name of secondary index.

~~~R
 example:
type Project @model {
  id: ID!
  name: String
  team: Team @connection
}

type Team @model {
  id: ID!
  name: String!
}
~~~
