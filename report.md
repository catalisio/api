# Catalisio API
## Report
Generating a report is asynchronous. To get a report, there are 3 steps :
1. Ask for a generation
2. Wait until the report generation status is done
3. Get the report

Types of available reports :
1. keyword

### Ask for a generation
`POST /<publicSiteId>/report/<type>`
#### Description
Ask for a report generation. A worker will treat the demand as soon as possible.

`<type>` is the type of the report you want.
#### Data
View the documentation for type of report you want.
#### Response body
```
{
    "reportId" : <report_id>
}
```
### Get status
`GET /<publicSiteId>/report/<reportId>/status`
#### Description
Get the status for a report generation. Statuses are :
* `in queue` : demand is ok, but still waiting for treatment
* `working` : the report is in treatment
* `done` : the report is ready
* `error` : something is wrong
#### Response body
```
{
    "reportId" : <report_id>,
    "status" : <status>,
    "creationDate" : <creation_date>
}
```
### Get the report
`GET /<publicSiteId>/report/<reportId>`
#### Description
Get the report has a file.
#### Response
The response is a file stream.
