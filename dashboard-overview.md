---

Copyright:
  years: 2018, 2019
lastupdated: "2019-04-15"

subcollection: databases-for-mongodb

---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen: .screen}
{:codeblock: .codeblock}
{:pre: .pre}
{:tip: .tip}

# The UI - Dashboard Overview
{: #dashboard-overview}

The _Overview_ page shows you information about your {{site.data.keyword.databases-for-mongodb_full}} database. The overview includes essential identifying information.

## Deployment Details

The _Deployment Details_ panel shows a quick description of your deployment.

### Type

The type of database that is offered by the service, and the database version that your service uses. 

### ID

The ID is a [CRN (Cloud Resource Name)](https://{DomainName}/docs/overview/crn.html) which uniquely identifies the database deployment. The CRN is used to refer to the database in the API and can be used with the CLI.

## Recent Tasks

Every time that you make administrative changes to your service (such as scaling, or taking a manual backup), a task starts up. The _Recent Tasks_ panel shows the task name and progress bar for any running tasks, and a list of the most recent completed tasks.

## Connections

The _Connections_ panel contains connection strings for your deployment. Each tab contains connection information tailored to the type of connection or the protocol that uses it. Basic information includes things like hostname and port number, as well as the TLS self-signed certificate, the replica set name, and arguments that can be passed to the driver or binary that you are using to connect. 

Reference tables for the different connection types are available on the [Getting Credentials and Connection Strings](/docs/services/databases-for-redis?topic=databases-for-redis-connection-strings) page.

Connection strings reflect whether your deployment uses public endpoints or private endpoints. For more information, see the [Service Endpoints Integration](/docs/services/databases-for-mongodb?topic=databases-for-mongodb-service-endpoints) page.

## Security

Encryption at rest is enabled for all {{site.data.keyword.databases-for-mongodb}} deployments. If you brought your own encryption key from [Key Protect](/docs/services/databases-for-mongodb?topic=databases-for-mongodb-key-protect), the panel provides a link to your Key Protect instance and the _Encryption Key_ field has the name of the key.

## Instance Administration API

You can manage your {{site.data.keyword.databases-for-mongodb}} service through the {{site.data.keyword.cloud_notm}} databases API. This panel provides the essential information for using the API.

### Foundation Endpoint

The foundation endpoint is the opening stanza of the URL to be used to send API requests to. It combines the region that your service resides in and the base {{site.data.keyword.cloud_notm}} databases API endpoint. 

### Deployment ID

Many API calls require the ID of the database deployment. The database deployment's ID/CRN shown here is the same as the ID/CRN shown in the Deployment Details, in a click-to-copy field to make it simpler to use. 

The ID needs to be URL encoded to be used in an API call because the CRN includes a "/".
{: .tip}

### {{site.data.keyword.cloud_notm}} databases API Reference

For more information about the {{site.data.keyword.cloud_notm}} databases API, see the [API reference](https://{DomainName}/apidocs/cloud-databases-api) page.

## Settings

The _Settings_ tab contains the UI for many of the tunable settings for your deployment. You can 
- [scale](/docs/services/databases-for-mongodb?topic=databases-for-mongodb-resources-scaling)
- [change the admin password](/docs/services/databases-for-mongodb?topic=databases-for-mongodb-admin-password)
- [implement or modify an IP whitelist](/docs/services/databases-for-mongodb?topic=cloud-databases-whitelisting)

## Backups

The _Backups_ tab is the UI for managing your deployments backups. All of the available backups are listed with their timestamps. Click on a backup to grab its ID or to restore it into a new deployment. More information is on the [Managing Backups](/docs/services/databases-for-mongodb?topic=databases-for-mongodb-dashboard-backups) page.

## Docs

The _Docs_ link opens the main documentation page for {{site.data.keyword.databases-for-mongodb}} in a new tab.