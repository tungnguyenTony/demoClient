# Demo Client
## Client microservice description
Goals
  - The user could manage their client-related info.
  - The supporting information or field just enough for SME to get started (don't overwhelm the user and shouldn't be too complicated for implementation)
  - Could be connected to third-parties CRM to sync client and contact information.

Background and strategic fit: This service could consider an out of the box simple CRM (Customer Related Management) for our solution without touching the sale related aspect of a CRM. It could be a first step for us to support integration with any third party CRM like Hubspot, Pipedrive, or Salesforce.
==========

## Database design
![preview](https://github.com/tungnguyenTony/demoClient/blob/master/src/main/resources/static/images/common/CRM-Client%20Entity%20Relationship.jpg)

## Activities diagram
![preview](https://github.com/tungnguyenTony/demoClient/blob/master/src/main/resources/static/images/common/CRM-Client%20Activities.jpg)

## [Launch demo here](https://zamo-demo-client.herokuapp.com/client/dashboard#/)

## Example to call Client API
  - Go to https://apitester.com/#
  - Select Method as POST + use https://zamo-demo-client.herokuapp.com/client/data/insert link
  - In the project crmdatamockup / crm / request.json folder => copy the content into the post data
  - In the header add 1 record: Content-type - application / json
  - Click Test
  - If success will see the response below, if not see error message
