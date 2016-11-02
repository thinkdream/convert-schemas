# convert-schemas
Ideas about a tool that helps to convert a schema into another, scheme about data description

Of course, it's not about validation, even I think it's required

# General thoughts

I have an affinity to JSON Schema, I don't know why, I just like it, probably because it can be used almost everywhere, you can validate data, generate forms, convert it (easy or not) to other scheme, quite a standard.
 
The intention of this repository is not to be an "awesome" repository for JSON Schema, but a study over the capability to have scheme defined in a way and convert them at compile time or runtime into another scheme. 

Usually user intervention is required for some scheme, so I think that an approach to a sort of templating system for JSON would be very helpful, for usage by our library and to be customized by the developer. Probably for some targets plugins are needed, too.

The purpose is not to define a new schema language (even sometimes make sense) but to find the best way of conversion, a base schema and some targets (GraphQL, JSON Schema, etc.).
            
Let's star with an overview.      
      
# Libraries that converts or define different types of scheme
 
Some of these libraries below doesn't belong here, or, some are missing, but until a deeper understanding here is the  list:
 
## Schemas to start with
 
JSON Schema, Mongoose, GraphQL, Knex,  
 
## Transformers
 
https://github.com/amida-tech/jsonapter  ** looks quite interesting

https://github.com/georgeadamson/json-transformer **

https://github.com/codeslayer1/JSON-Transform  **

https://github.com/onechiporenko/jsonium **

https://github.com/nijikokun/generate-schema

https://github.com/wkrueger/swagger-ts-template

https://github.com/itd24/blacktea.jsonTemplates

https://github.com/nishants/jeyson

https://github.com/moappi/json2html

https://github.com/mock-end/json-from-template
 
 
 
## Unordered link list of formats transforms
 
https://github.com/ManjunathaN/jsonschema-to-graphql

https://github.com/joelkoz/omni-schema

https://github.com/muraljs/joiql

https://github.com/saibotsivad/json-schema-to-markdown

https://github.com/moqada/simple-api-client-generator

https://github.com/jhsware/isomorphic-schema

https://github.com/hapijs/joi

https://github.com/andrglo/json-schema-entity

https://github.com/ryanramage/schema-couch

https://github.com/ortoo/protobuf-to-mongoose

https://github.com/fastcodejava/schematodoc

https://github.com/vkarpov15/archetype-js

https://github.com/azuqua/rdb-migrate

https://github.com/xogroup/felicity

https://github.com/photobox/design-storage-schema

https://github.com/leizongmin/hojs-schema

https://github.com/noxt/json-model-generator

https://github.com/skolmer/i18n-tag-schema

https://github.com/ezirmusitua/json-generator

https://github.com/kissarat/schema-db

https://github.com/milesj/shapeshifter

https://github.com/andrewbober/xsd2jsonschema

https://github.com/paularmstrong/normalizr

https://github.com/bopjesvla/v-js

https://github.com/AaronCallahan/csv-to-schema

https://github.com/hippopotamus2/json-schema-docs

https://github.com/octo-sniffle/dbf2mysql

https://github.com/rab206/convert-ea-json-schema

https://github.com/philcockfield/react-schema

https://github.com/kriszyp/json-schema

https://github.com/deanlandolt/query-schema

https://github.com/eliot-akira/proptypes-schema

https://github.com/akabab/JSTSM

https://github.com/Genivia/SJOT

https://github.com/Boxable/lodash-schema

https://github.com/nijikokun/generate-schema

https://github.com/directlyio/redink-schema

https://github.com/Ensembl/XML-To-Blockly

https://github.com/mateusmaso/graphql-jay-hyperschema

https://github.com/joarwilk/gql2flow

https://github.com/AubreyHewes/redux-form-byschema

https://github.com/fairsayan/mongoose2swagger

https://github.com/dave-irvine/node-sqlschemify

https://github.com/kuip/meteor-schema-graphql-bridge

https://github.com/DScheglov/mongoose-schema-jsonschema

https://github.com/bjrmatos/json-schema-sugar

https://github.com/rootsdev/gedcomx-fs-json-schema

https://github.com/rootsdev/gedcomx-json-schema

https://github.com/FredLackey/generator-mssql-schema

https://github.com/raml2html/raml2html

https://github.com/raml2html/raml2md

https://github.com/raml2html/raml2obj

https://github.com/lightsofapollo/joi-to-json-schema

https://github.com/raml-org/ramldt2jsonschema

https://github.com/justincy/gedx-js-generator

https://github.com/morlay/json-schema-to-flow-type

https://github.com/andrewshawcare/swag-operator

https://github.com/json-schema-form/json-schema-form-core

https://github.com/scottbea/schemata

https://github.com/simon-p-r/hapi-json-schema

https://github.com/canastro/metamorphosis

https://github.com/simon-p-r/json-schema-models

https://github.com/smikodanic/mongoose_schema-json

https://github.com/qawemlilo/widget-knex-schema

https://github.com/simonguest/swagger-mongoose

https://github.com/kingsquare/swagger-sequelize

https://github.com/Svehla/table-to-schema

https://github.com/Kikobeats/osom

https://github.com/ashgkwd/tenali

https://github.com/shiwano/typhen-json-schema

https://github.com/greengerong/rebirth-model

https://github.com/IntegrateDev/json2schema

https://github.com/ElectricCookie/sure-js

https://github.com/scotthovestadt/schema-object

https://github.com/sarkistlt/mongoose-schema-to-graphql

https://github.com/polytypic/schemation

https://github.com/pmelisko/schema2doc

https://github.com/vstirbu/mongoose-jsonschema

https://github.com/fsbahman/apidoc-swagger

https://github.com/sprour/mongoose-schema-to-graphql

https://github.com/node-packages/json2schema

https://github.com/wwayne/mooseql

https://github.com/toystars/mongo-schema-gen

https://github.com/RevoltTV/joi-to-swagger

https://github.com/zhengxyit/waterline-schema-saas

https://github.com/joxoo/jsonschema-md

https://github.com/john-doherty/jsdoc-to-json-schema

https://github.com/rsuite/rsuite-schema

https://github.com/lbovet/typson

https://github.com/nanachimi/mongoosify

https://github.com/rajington/alexa-schemas

https://github.com/aishee/json-to-md

https://github.com/SpringTree/jsonschema-to-typings

https://github.com/mprinc/JsonTransform

https://github.com/vandium-io/joi-json

https://github.com/PGS-dev/raml-types-to-schemas

https://github.com/thomas4019/json-schema-editor

https://github.com/YangXin/json2schema

https://github.com/chaliy/sequelize-json-schema

https://github.com/sanusart/json-schema-batch-generator

https://github.com/pblabs/swaggering-mongoose

https://github.com/Aweary/json-to-graphql

https://github.com/arupex/model-convert

https://github.com/bongoYo/invoiceCreation


** https://github.com/jlblcc/json-schema-viewer
