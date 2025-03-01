---
title: Service management
linkTitle: Service management
weight: 20
---

An API Service represents an API, including all its versions and deployed endpoints, and additional information to represent your API. For example, description, environment scope, image encoded in base64.

Use the Service Registry WebUI to view all your API Services across all environments.

Use the Topology WebUI to select an environment and then manage your API Services, including view, create, update, and delete.

## Before you start

You must have credentials or a user account from your org Administrator to use the Service Registry WebUI.  Please follow the steps [here](https://docs.axway.com/bundle/platform-management/page/docs/management_guide/organizations/managing_organizations/index.html#managing-users).

## Objectives

Learn how to use the Service Registry WebUI to create and manage services, including:

* List all API Services in an environment
* View details for an API Service
* Create a new API Service
* Delete an API Service

## List API Services

To list API Services:

1. Navigate to *Catalog > Service Registry*.
2. View the following information for all services:

   * Environment
   * Assets
   * Owner
   * Version
   * Tags
   * Created/Updated date by User

You can also filter the services by the Service type, Environment and Team Ownership using the **Filter By** controls. Search by the Service Name with the search bar.

## View API Service details

To view service details:

1. Navigate to *Catalog > Service Registry*.
2. From the list view, select a service to open the service details.

View the following detailed information for a specific service in any state (Draft, Active, Deprecated, Active):

* Service Name, Logical Name, Description, Owning Team, Tags, Attributes, Endpoints, Active Version, Spec, Created on / Modified on date by User
* Per Service Version Tags and Attributes
* The API Specification and Methods
* Endpoints listening for requests to the service

## Create an API Service

1. Navigate to *Topology* and select an environment.
2. Click **+ Add API Service** to add a new service.
3. Upload an API Specification file.
4. Some information will be read from the API Specification file and pre-populated. Add / Edit information where applicable and then click **Next**:

    * Service Name - The display name for the service in the WebUI
    * Description - A short description of the service
    * Image - An icon or image to be associated with the service

5. Add / edit Endpoint information, if available, and then click **Next**.
6. Click **Save**.

## Delete an API Service

1. Navigate to *Catalog > Service Registry*.
2. From the list view, select a service to open the service details.
3. Click on the environment name breadcrumb at the top of the page (i.e., the name to the right of **ENVIRONMENTS / NAME**).
4. In the *Services* tab at the bottom of the page, click on the trash bin associated with the service you want to delete.
5. Type the name of the service and click on the confirmation button that “I understand this is a permanent and irreversible action. Delete.” **All versions of the service are deleted.**
