# ![LOGO](logo.png) Fusion Tables **flow**ground Connector

## Description

A generated **flow**ground connector for the Fusion Tables API (version v2).

Generated from: https://www.googleapis.com/fusiontables/v2<br/>
Generated at: 2019-09-24T15:08:11+00:00

## API Description

API for working with Fusion Tables data.<br/>

## Authorization

Supported authorization schemes:
- OAuth2 - Oauth 2.0 authentication

For OAuth 2.0 you need to specify OAuth Client credentials as environment variables in the connector repository:
* `OAUTH_CLIENT_ID` - your OAuth client id
* `OAUTH_CLIENT_SECRET` - your OAuth client secret

## Actions

### fusiontables.query.sqlGet
> Executes a SQL statement which can be any of <br/>
> - SELECT<br/>
> - SHOW<br/>
> - DESCRIBE<br/>

*Tags:* `query`

#### Input Parameters
* `hdrs` - _optional_ - Whether column names are included (in the first row). Default is true.<br/>
* `sql` - _required_ - A SQL statement which can be any of <br/>
- SELECT<br/>
- SHOW<br/>
- DESCRIBE<br/>
* `typed` - _optional_ - Whether typed values are returned in the (JSON) response: numbers for numeric values and parsed geometries for KML values. Default is true.<br/>
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.<br/>
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.<br/>
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.<br/>
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.<br/>

### fusiontables.query.sql
> Executes a Fusion Tables SQL statement, which can be any of <br/>
> - SELECT<br/>
> - INSERT<br/>
> - UPDATE<br/>
> - DELETE<br/>
> - SHOW<br/>
> - DESCRIBE<br/>
> - CREATE statement.<br/>

*Tags:* `query`

#### Input Parameters
* `hdrs` - _optional_ - Whether column names are included in the first row. Default is true.<br/>
* `sql` - _required_ - A Fusion Tables SQL statement, which can be any of <br/>
- SELECT<br/>
- INSERT<br/>
- UPDATE<br/>
- DELETE<br/>
- SHOW<br/>
- DESCRIBE<br/>
- CREATE<br/>
* `typed` - _optional_ - Whether typed values are returned in the (JSON) response: numbers for numeric values and parsed geometries for KML values. Default is true.<br/>
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.<br/>
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.<br/>
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.<br/>
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.<br/>

### fusiontables.table.list
> Retrieves a list of tables a user owns.<br/>

*Tags:* `table`

#### Input Parameters
* `maxResults` - _optional_ - Maximum number of tables to return. Default is 5.<br/>
* `pageToken` - _optional_ - Continuation token specifying which result page to return.<br/>
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.<br/>
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.<br/>
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.<br/>
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.<br/>
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.<br/>

### fusiontables.table.insert
> Creates a new table.<br/>

*Tags:* `table`

#### Input Parameters
* `alt` - _optional_ - Data format for the response.<br/>
    Possible values: csv, json.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.<br/>
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.<br/>
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.<br/>
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.<br/>
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.<br/>
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.<br/>

### fusiontables.table.importTable
> Imports a new table.<br/>

*Tags:* `table`

#### Input Parameters
* `delimiter` - _optional_ - The delimiter used to separate cell values. This can only consist of a single character. Default is ,.<br/>
* `encoding` - _optional_ - The encoding of the content. Default is UTF-8. Use auto-detect if you are unsure of the encoding.<br/>
* `name` - _required_ - The name to be assigned to the new table.<br/>
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.<br/>
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.<br/>
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.<br/>
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.<br/>

### fusiontables.table.delete
> Deletes a table.<br/>

*Tags:* `table`

#### Input Parameters
* `tableId` - _required_ - ID of the table to be deleted.<br/>
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.<br/>
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.<br/>
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.<br/>
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.<br/>
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.<br/>
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.<br/>

### fusiontables.table.get
> Retrieves a specific table by its ID.<br/>

*Tags:* `table`

#### Input Parameters
* `tableId` - _required_ - Identifier for the table being requested.<br/>
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.<br/>
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.<br/>
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.<br/>
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.<br/>
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.<br/>
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.<br/>

### fusiontables.table.patch
> Updates an existing table. Unless explicitly requested, only the name, description, and attribution will be updated. This method supports patch semantics.<br/>

*Tags:* `table`

#### Input Parameters
* `replaceViewDefinition` - _optional_ - Whether the view definition is also updated. The specified view definition replaces the existing one. Only a view can be updated with a new definition.<br/>
* `tableId` - _required_ - ID of the table that is being updated.<br/>
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.<br/>
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.<br/>
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.<br/>
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.<br/>
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.<br/>

### fusiontables.table.update
> Updates an existing table. Unless explicitly requested, only the name, description, and attribution will be updated.<br/>

*Tags:* `table`

#### Input Parameters
* `replaceViewDefinition` - _optional_ - Whether the view definition is also updated. The specified view definition replaces the existing one. Only a view can be updated with a new definition.<br/>
* `tableId` - _required_ - ID of the table that is being updated.<br/>
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.<br/>
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.<br/>
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.<br/>
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.<br/>
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.<br/>

### fusiontables.column.list
> Retrieves a list of columns.<br/>

*Tags:* `column`

#### Input Parameters
* `maxResults` - _optional_ - Maximum number of columns to return. Default is 5.<br/>
* `pageToken` - _optional_ - Continuation token specifying which result page to return.<br/>
* `tableId` - _required_ - Table whose columns are being listed.<br/>
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.<br/>
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.<br/>
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.<br/>
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.<br/>

### fusiontables.column.insert
> Adds a new column to the table.<br/>

*Tags:* `column`

#### Input Parameters
* `tableId` - _required_ - Table for which a new column is being added.<br/>
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.<br/>
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.<br/>
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.<br/>
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.<br/>
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.<br/>
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.<br/>

### fusiontables.column.delete
> Deletes the specified column.<br/>

*Tags:* `column`

#### Input Parameters
* `columnId` - _required_ - Name or identifier for the column being deleted.<br/>
* `tableId` - _required_ - Table from which the column is being deleted.<br/>
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.<br/>
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.<br/>
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.<br/>
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.<br/>
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.<br/>

### fusiontables.column.get
> Retrieves a specific column by its ID.<br/>

*Tags:* `column`

#### Input Parameters
* `columnId` - _required_ - Name or identifier for the column that is being requested.<br/>
* `tableId` - _required_ - Table to which the column belongs.<br/>
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.<br/>
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.<br/>
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.<br/>
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.<br/>
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.<br/>

### fusiontables.column.patch
> Updates the name or type of an existing column. This method supports patch semantics.<br/>

*Tags:* `column`

#### Input Parameters
* `columnId` - _required_ - Name or identifier for the column that is being updated.<br/>
* `tableId` - _required_ - Table for which the column is being updated.<br/>
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.<br/>
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.<br/>
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.<br/>
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.<br/>
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.<br/>

### fusiontables.column.update
> Updates the name or type of an existing column.<br/>

*Tags:* `column`

#### Input Parameters
* `columnId` - _required_ - Name or identifier for the column that is being updated.<br/>
* `tableId` - _required_ - Table for which the column is being updated.<br/>
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.<br/>
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.<br/>
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.<br/>
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.<br/>
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.<br/>

### fusiontables.table.copy
> Copies a table.<br/>

*Tags:* `table`

#### Input Parameters
* `copyPresentation` - _optional_ - Whether to also copy tabs, styles, and templates. Default is false.<br/>
* `tableId` - _required_ - ID of the table that is being copied.<br/>
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.<br/>
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.<br/>
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.<br/>
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.<br/>
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.<br/>

### fusiontables.table.importRows
> Imports more rows into a table.<br/>

*Tags:* `table`

#### Input Parameters
* `delimiter` - _optional_ - The delimiter used to separate cell values. This can only consist of a single character. Default is ,.<br/>
* `encoding` - _optional_ - The encoding of the content. Default is UTF-8. Use auto-detect if you are unsure of the encoding.<br/>
* `endLine` - _optional_ - The index of the line up to which data will be imported. Default is to import the entire file. If endLine is negative, it is an offset from the end of the file; the imported content will exclude the last endLine lines.<br/>
* `isStrict` - _optional_ - Whether the imported CSV must have the same number of values for each row. If false, rows with fewer values will be padded with empty values. Default is true.<br/>
* `startLine` - _optional_ - The index of the first line from which to start importing, inclusive. Default is 0.<br/>
* `tableId` - _required_ - The table into which new rows are being imported.<br/>
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.<br/>

### fusiontables.table.refetchSheet
> Replaces rows of the table with the rows of the spreadsheet that is first imported from. Current rows remain visible until all replacement rows are ready.<br/>

*Tags:* `table`

#### Input Parameters
* `tableId` - _required_ - Table whose rows will be replaced from the spreadsheet.<br/>
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.<br/>
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.<br/>
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.<br/>
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.<br/>
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.<br/>
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.<br/>

### fusiontables.table.replaceRows
> Replaces rows of an existing table. Current rows remain visible until all replacement rows are ready.<br/>

*Tags:* `table`

#### Input Parameters
* `delimiter` - _optional_ - The delimiter used to separate cell values. This can only consist of a single character. Default is ,.<br/>
* `encoding` - _optional_ - The encoding of the content. Default is UTF-8. Use 'auto-detect' if you are unsure of the encoding.<br/>
* `endLine` - _optional_ - The index of the line up to which data will be imported. Default is to import the entire file. If endLine is negative, it is an offset from the end of the file; the imported content will exclude the last endLine lines.<br/>
* `isStrict` - _optional_ - Whether the imported CSV must have the same number of column values for each row. If true, throws an exception if the CSV does not have the same number of columns. If false, rows with fewer column values will be padded with empty values. Default is true.<br/>
* `startLine` - _optional_ - The index of the first line from which to start importing, inclusive. Default is 0.<br/>
* `tableId` - _required_ - Table whose rows will be replaced.<br/>
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.<br/>

### fusiontables.style.list
> Retrieves a list of styles.<br/>

*Tags:* `style`

#### Input Parameters
* `maxResults` - _optional_ - Maximum number of styles to return. Optional. Default is 5.<br/>
* `pageToken` - _optional_ - Continuation token specifying which result page to return. Optional.<br/>
* `tableId` - _required_ - Table whose styles are being listed<br/>
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.<br/>
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.<br/>
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.<br/>
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.<br/>

### fusiontables.style.insert
> Adds a new style for the table.<br/>

*Tags:* `style`

#### Input Parameters
* `tableId` - _required_ - Table for which a new style is being added<br/>
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.<br/>
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.<br/>
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.<br/>
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.<br/>
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.<br/>
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.<br/>

### fusiontables.style.delete
> Deletes a style.<br/>

*Tags:* `style`

#### Input Parameters
* `styleId` - _required_ - Identifier (within a table) for the style being deleted<br/>
* `tableId` - _required_ - Table from which the style is being deleted<br/>
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.<br/>
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.<br/>
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.<br/>
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.<br/>
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.<br/>

### fusiontables.style.get
> Gets a specific style.<br/>

*Tags:* `style`

#### Input Parameters
* `styleId` - _required_ - Identifier (integer) for a specific style in a table<br/>
* `tableId` - _required_ - Table to which the requested style belongs<br/>
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.<br/>
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.<br/>
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.<br/>
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.<br/>
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.<br/>

### fusiontables.style.patch
> Updates an existing style. This method supports patch semantics.<br/>

*Tags:* `style`

#### Input Parameters
* `styleId` - _required_ - Identifier (within a table) for the style being updated.<br/>
* `tableId` - _required_ - Table whose style is being updated.<br/>
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.<br/>
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.<br/>
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.<br/>
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.<br/>
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.<br/>

### fusiontables.style.update
> Updates an existing style.<br/>

*Tags:* `style`

#### Input Parameters
* `styleId` - _required_ - Identifier (within a table) for the style being updated.<br/>
* `tableId` - _required_ - Table whose style is being updated.<br/>
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.<br/>
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.<br/>
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.<br/>
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.<br/>
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.<br/>

### fusiontables.task.list
> Retrieves a list of tasks.<br/>

*Tags:* `task`

#### Input Parameters
* `maxResults` - _optional_ - Maximum number of tasks to return. Default is 5.<br/>
* `pageToken` - _optional_ - Continuation token specifying which result page to return.<br/>
* `startIndex` - _optional_ - Index of the first result returned in the current page.<br/>
* `tableId` - _required_ - Table whose tasks are being listed.<br/>
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.<br/>
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.<br/>
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.<br/>

### fusiontables.task.delete
> Deletes a specific task by its ID, unless that task has already started running.<br/>

*Tags:* `task`

#### Input Parameters
* `tableId` - _required_ - Table from which the task is being deleted.<br/>
* `taskId` - _required_ - The identifier of the task to delete.<br/>
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.<br/>
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.<br/>
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.<br/>
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.<br/>
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.<br/>

### fusiontables.task.get
> Retrieves a specific task by its ID.<br/>

*Tags:* `task`

#### Input Parameters
* `tableId` - _required_ - Table to which the task belongs.<br/>
* `taskId` - _required_ - The identifier of the task to get.<br/>
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.<br/>
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.<br/>
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.<br/>
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.<br/>
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.<br/>

### fusiontables.template.list
> Retrieves a list of templates.<br/>

*Tags:* `template`

#### Input Parameters
* `maxResults` - _optional_ - Maximum number of templates to return. Optional. Default is 5.<br/>
* `pageToken` - _optional_ - Continuation token specifying which results page to return. Optional.<br/>
* `tableId` - _required_ - Identifier for the table whose templates are being requested<br/>
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.<br/>
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.<br/>
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.<br/>
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.<br/>

### fusiontables.template.insert
> Creates a new template for the table.<br/>

*Tags:* `template`

#### Input Parameters
* `tableId` - _required_ - Table for which a new template is being created<br/>
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.<br/>
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.<br/>
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.<br/>
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.<br/>
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.<br/>
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.<br/>

### fusiontables.template.delete
> Deletes a template<br/>

*Tags:* `template`

#### Input Parameters
* `tableId` - _required_ - Table from which the template is being deleted<br/>
* `templateId` - _required_ - Identifier for the template which is being deleted<br/>
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.<br/>
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.<br/>
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.<br/>
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.<br/>
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.<br/>

### fusiontables.template.get
> Retrieves a specific template by its id<br/>

*Tags:* `template`

#### Input Parameters
* `tableId` - _required_ - Table to which the template belongs<br/>
* `templateId` - _required_ - Identifier for the template that is being requested<br/>
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.<br/>
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.<br/>
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.<br/>
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.<br/>
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.<br/>

### fusiontables.template.patch
> Updates an existing template. This method supports patch semantics.<br/>

*Tags:* `template`

#### Input Parameters
* `tableId` - _required_ - Table to which the updated template belongs<br/>
* `templateId` - _required_ - Identifier for the template that is being updated<br/>
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.<br/>
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.<br/>
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.<br/>
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.<br/>
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.<br/>

### fusiontables.template.update
> Updates an existing template<br/>

*Tags:* `template`

#### Input Parameters
* `tableId` - _required_ - Table to which the updated template belongs<br/>
* `templateId` - _required_ - Identifier for the template that is being updated<br/>
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.<br/>
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.<br/>
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.<br/>
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.<br/>
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.<br/>

## License

**flow**ground :- Telekom iPaaS / fusion-tables-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
