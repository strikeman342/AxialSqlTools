This is a fork of https://github.com/Axial-SQL

I've forked this project to make some changes to make this plugin even better than it already is.

currently done:
- preserve comments during T-SQL formatting.

working on:
- update all System.Data.SqlClient references to Microsoft.Data.SqlClient references to take advantage of those capabilities
- update the 2 connectionstring builders to make them compatible with Azure SQL Servers & Azure SQL Managed Instances (using Entra to log in)
- update speed of the query history search by implementing FTS capabilities (if installed on the backend sql server)
- update query history search screen to be faster (currently there are issues when there are large queries in the history)
- add documentcaption to the query history table
- better handling of the commandbuttons that are used for the templates (currently done via try/catch, which has a noticable performance hit when having large amounts of templates)
- update "script selected object" to include indexes & triggers on views (if applicable), these are currently ignored
- update health dashboard to work with Azure SQL Managed Instances (not Azure SQL Servers)

