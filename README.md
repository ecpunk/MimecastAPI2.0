# Mimecast API 2.0 Integration Guide

## Table of Contents
1. [Overview](#overview)
2. [What's New in Mimecast API 2.0](#whats-new-in-mimecast-api-20)
3. [Choosing Between Mimecast API 2.0 and 1.0](#choosing-between-mimecast-api-20-and-10)
4. [Authentication & Authorization](#authentication--authorization)
5. [Postman Collection and Environment Configuration](#postman-collection-and-environment-configuration)
6. [Using the JSON Files with Postman](#using-the-json-files-with-postman)
7. [Practical Use Cases](#practical-use-cases)
8. [API Endpoint Reference](#api-endpoint-reference)
9. [Additional Resources](#additional-resources)

## Overview
This comprehensive guide is designed to assist developers with integrating and interacting with the Mimecast API 2.0. It includes detailed information on authentication processes, along with instructions for using the provided Postman collection and environment.

## What's New in Mimecast API 2.0
The latest version of Mimecast API introduces enhanced features and improvements over its predecessor. For the most recent updates and changes in API 2.0, users are encouraged to visit the 'What's new' section on the Mimecast documentation site.

## Choosing Between Mimecast API 2.0 and 1.0
Selecting the appropriate API version is crucial for optimal integration and performance:
- **API 2.0** is recommended for new Email Security Cloud Gateway customers, new Email Security Cloud Integrated customers (coming soon), and existing customers seeking access to new capabilities not available in API 1.0.
- **API 1.0** should continue to be used by existing Email Security Cloud Gateway customers with active integrations, but a migration plan to API 2.0 should be considered.

## Authentication & Authorization
After registering an application and obtaining the Client ID and Client Secret, these credentials are used to obtain an access token. The provided Postman collection includes examples of how to perform this step using different programming languages and tools like cURL, PowerShell, and Python.

## Postman Collection and Environment Configuration
### Environment Variables
Key variables in the "Mimecast Environment 2.0" Postman environment file include:

1. **bearerToken**
2. **accountCode**
3. **client_id**
4. **client_secret**

### Getting Started with Postman
To begin testing and development:

1. **Import and Configure**: Load the Mimecast environment and collection into Postman.
2. **Update Variables**: Populate the environment variables with your specific application details.
3. **Explore and Test**: Utilize the collection to make API calls, test endpoint functionalities, and familiarize yourself with the API's capabilities.

## Using the JSON Files with Postman
This guide includes two JSON files: "Mimecast 2.0.postman_collection.json" and "Mimecast Environment 2.0.postman_environment.json". These files are essential for interacting with the Mimecast API 2.0 using Postman and streamline the process of making API requests.

### Importing the Collection and Environment into Postman
1. **Importing the Collection**:
    - Open Postman.
    - Click on the 'Import' button at the top left corner.
    - Choose the "Mimecast 2.0.postman_collection.json" file.
    - This action imports all the API endpoints as a collection into Postman.

2. **Importing the Environment**:
    - Follow the same steps as above but select the "Mimecast Environment 2.0.postman_environment.json" file.
    - This imports the environment variables needed to execute the requests in the collection.

### Configuring the Environment Variables
- Once the environment is imported, select it from the top right environment dropdown in Postman.
- Click on the eye icon next to the environment dropdown and select 'Edit' to modify the environment variables.
- Update the `bearerToken`, `accountCode`, `client_id`, and `client_secret` variables with your specific Mimecast application details.
- These variables are crucial for authentication and making successful API requests.

### Using the Collection to Make API Requests
- With the environment selected and variables configured, you can now use the requests in the Mimecast 2.0 collection.
- Select an endpoint from the collection.
- Review the pre-configured request and modify it if necessary.
- Send the request to interact with the Mimecast API 2.0.
- The response will be displayed in Postman, allowing you to verify the results and debug if needed.

## Practical Use Cases

### Automated Threat Management
#### Scenario
A cybersecurity team aims to automate monitoring and response to email-based threats using Mimecast's API to quickly identify and take action against potential threats, even from 3rd party applications such as SIEM's or SOAR's.
#### Application
Utilizing "Threat Management" endpoints, such as `ttp/remediation/search-hash` for identifying threats and `ttp/remediation/create` for automated responses.

### Compliance and Audit Reporting
#### Scenario
An IT compliance officer needs to generate regular audit reports for adherence to email security policies and data protection regulations.
#### Application
Using "Audit Events" endpoints like `Get Archive Search Logs` and `Get Audit Events` to gather necessary audit information and ensure compliance.

## API Endpoint Reference

### Get Oauth Token

### Get Account

### Account Management
- Get Dashboard Notifications
- Get Support Info
- Get Packages
- Create Config Snapshot
- Export Config Snapshot
- List Config Snapshots
- Restore Config Snapshot

### Audit Events
- Get Archive Search Logs
- Get Search Logs
- Get View Logs
- Get Audit Events
- Get Audit Categories
- Get Held Release Logs
- Get Rejections

### Awareness Training
- Get Performance Details
- Get Performance Summary
- Get Safe Score Details
- Get Safe Score Summary
- Get Watchlist Details
- Get Watchlist Summary
- Get Campaign
- Get User Data
- Get Queue
- Get Training Details

### Data Retention
- Get File
- Get Message Detail
- Get Message List
- Get Message Part
- Search Archive

### Domain Management
- Create Domain
- Delete Pending Domain
- Get Internal Domain
- Get Pending Domain
- Get Provision Status
- Get Verification Code
- Verify Domain

### Email Security Cloud Gateway
- Get Email Queues
- Send Email
- File Upload
- Find Processing Messages
- Get Hold Message List
- Get Hold Summary List
- Hold Reject
- Hold Release
- message/get-file
- journaling/get-service
- managedsender/permit-or-block-sender
- message-finder/get-message-info
- message-finder/search
- ttp/url/decode-url

### Policy Management
- address-alteration/create-address-alteration-set
- address-alteration/create-definition
- address-alteration/create-policy
- address-alteration/delete-definition
- address-alteration/delete-policy
- address-alteration/get-address-alteration-set
- address-alteration/get-definition
- address-alteration/get-policy
- address-alteration/update-policy
- antispoofing-bypass/create-policy
- antispoofing-bypass/delete-policy
- antispoofing-bypass/get-policy
- antispoofing-bypass/update-policy
- blocked-senders/create-policy
- blockedsenders/get-policy
- webwhiteurl/create-policy-with-targets
- webwhiteurl/delete-policy-with-targets
- webwhiteurl/get-policy-with-targets
- webwhiteurl/update-policy-with-targets
- ttp/url/create-managed-url
- ttp/url/delete-managed-url
- ttp/url/get-all-managed-urls

### Security Events
- dlp/get-logs
- ttp/attachment/get-logs
- ttp/impersonation/get-logs
- ttp/url/get-logs

### Threat Management
- byo-threat-intelligence/create-batch
- byo-threat-intelligence/delete-batch
- byo-threat-intelligence/get-batches
- byo-threat-intelligence/get-quota
- ttp/remediation/create
- ttp/remediation/find-incidents
- ttp/remediation/get-incident
- ttp/remediation/search-hash
- ttp/remediation/v2/create

### Threats, Security Events, and Data
- siem/v1/batch/events/cg
- siem/v1/events/cg
- threats/v1/stats/attachment-scans
- threats/v1/stats/gateway-detections
- threats/v1/stats/impersonations
- threats/v1/stats/url-clicks

### User and Group Management
- directory/add-group-member
- directory/create-group
- directory/delete-group
- directory/execute-sync
- directory/find-groups
- directory/get-connection
- directory/get-group-members
- directory/remove-group-member
- directory/update-group
- user/add-delegate-user
- user/create-user
- user/find-delegate-users
- user/get-aliases
- user/get-attributes
- user/get-import-status
- user/get-internal-users
- user/get-most-used-contacts
- user/import-users
- user/remove-alias
- user/remove-delegate-user
- user/update-alias
- user/update-attributes
- user/update-user

## Additional Resources
For more detailed information and documentation on the Mimecast API 2.0, please visit:

- [Mimecast API Overview](https://developer.services.mimecast.com/api-overview)
- [Mimecast APIs](https://developer.services.mimecast.com/apis)
