# Mimecast API 2.0 Integration Guide

## Table of Contents
1. [Overview](#overview)
2. [What's New in Mimecast API 2.0](#whats-new-in-mimecast-api-20)
3. [Choosing Between Mimecast API 2.0 and 1.0](#choosing-between-mimecast-api-20-and-10)
4. [Key API Endpoints](#key-api-endpoints)
5. [Postman Collection and Environment Configuration](#postman-collection-and-environment-configuration)
6. [Additional Resources](#additional-resources)

## Overview
This comprehensive guide is designed to assist developers with integrating and interacting with the Mimecast API 2.0. It includes detailed information on API endpoints, application registration, authentication processes, response code interpretations, API call restrictions, pagination handling, and delegate access, along with instructions for using the provided Postman collection and environment.

## What's New in Mimecast API 2.0
The latest version of Mimecast API introduces enhanced features and improvements over its predecessor. For the most recent updates and changes in API 2.0, users are encouraged to visit the 'What's new' section on the Mimecast documentation site.

## Choosing Between Mimecast API 2.0 and 1.0
Selecting the appropriate API version is crucial for optimal integration and performance:
- **API 2.0** is recommended for new Email Security Cloud Gateway customers, new Email Security Cloud Integrated customers (coming soon), and existing customers seeking access to new capabilities not available in API 1.0.
- **API 1.0** should continue to be used by existing Email Security Cloud Gateway customers with active integrations, but a migration plan to API 2.0 should be considered.

## Key API Endpoints
Mimecast API 2.0 encompasses a wide range of functionalities through its various endpoints. The primary endpoints available in the collection include:

1. **Account Management**: Handles all aspects of account settings and configurations.
2. **Audit Events**: Provides access to audit logs and event tracking.
3. **Awareness Training**: Manages user training modules and awareness programs.
4. **Data Retention**: Controls data retention policies and configurations.
5. **Domain Management**: Enables the management and configuration of email domains.
6. **Email Security Cloud Gateway**: Specialized endpoint for managing email security settings.
7. **Policy Management**: Facilitates the creation and management of security and handling policies.
8. **Security Events**: Tracks and reports on security-related events and incidents.
9. **Threat Management**: Offers tools for identifying, analyzing, and managing email threats.
10. **Threats, Security Events, and Data**: A comprehensive endpoint for all threat-related information and data analytics.
11. **User and Group Management**: Manages user accounts and group permissions.
12. **Get Oauth Token**: Endpoint for obtaining OAuth authentication tokens.
13. **Get Account**: Retrieves account-specific information and settings.

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

By following these steps, you can effectively utilize the provided JSON files to interact with the Mimecast API 2.0 using Postman. This setup simplifies the process of testing and developing your integrations with Mimecast services.

## Additional Resources
For more detailed information and documentation on the Mimecast API 2.0, please visit:

- [Mimecast API Overview](https://developer.services.mimecast.com/api-overview)
- [Mimecast APIs](https://developer.services.mimecast.com/apis)

This README aims to provide a thorough understanding of the Mimecast API 2.0, equipping developers with the knowledge and tools needed for successful integration and usage.
