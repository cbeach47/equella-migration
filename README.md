# equella-migration
Toolset to migrate attachments from Equella items to other repositories

To invoke:
```
java -jar equella-migration-vYYYYMMDD.jar config.properties
```


Inputs (via a `properties` file):
```
// Required
// Kaltura migration scheme: kaltura
scheme
// Required - filters target items via a single collection uuid
collection
// Required - filters target items via a single metadata path
metadata.filter.path
metadata.filter.value
// Required - institution URL
url
// Authenticates via Client Credentials OAuth
oauth.key
oauth.secret
// kaltura.* are specifically for the Kaltura scheme
// Associates a static value to the Kaltura categories
kaltura.categories.static
// Associates an Equella metadata path (assumes there are multiple matching metadata paths) to Kaltura tags
kaltura.tags
```
